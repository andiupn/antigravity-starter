---
name: wiki-lint
description: |
  Cek konsistensi `.gemini/wiki/`: broken [[refs]], orphan files (tidak ada inbound link),
  dan missing front pages (README.md per subfolder jika ada).
  Trigger when: user minta "lint wiki", "cek wiki", "wiki-lint", "cek broken links di wiki".
  Do NOT trigger when: project tidak punya `.gemini/wiki/` directory.
tools: [Read, Grep, Glob]
agent: false
model: flash
color: blue
---

# Wiki Lint Skill

**Bahasa output:** Indonesia. File paths dan ref names dalam English.

## Proses

1. **Check wiki exists** — Glob `.gemini/wiki/**/*.md`. Jika empty: output "Wiki kosong atau belum dibuat. Buat `.gemini/wiki/` terlebih dahulu." Stop.

2. **Build file inventory** — List semua `.md` files di `.gemini/wiki/`. Simpan sebagai set.

3. **Extract refs** — Untuk setiap file, extract semua `[[double-bracket]]` refs:
   - Pattern: `\[\[([^\]]+)\]\]`
   - Resolve relative ke `.gemini/wiki/` → expected path `<ref>.md`
   - Jika ref tidak mengandung `/`, cek di root wiki
   - Jika ref mengandung `/`, cek di subfolder

4. **Check broken refs** — Setiap ref yang di-extract: apakah file-nya ada di inventory? Jika tidak: tambahkan ke broken list.

5. **Find orphans** — File yang tidak punya inbound link (tidak ada file lain yang `[[ref]]` ke file ini). Kecuali: `README.md` — tidak perlu inbound link.

6. **Check front pages** — Pastikan ada `README.md` di subfolder yang ada.

7. **Output report**

## Output Format

```
## Wiki Lint Report — <project_name>

### Summary
- Files scanned: N
- Broken refs: N
- Orphan files: N
- Missing front pages: N

### Broken Refs
| File | Line | Broken Ref |
|---|---|---|

### Orphan Files

### Status: PASS / WARN / FAIL
- PASS: 0 broken refs, 0 missing pages (orphans acceptable)
- WARN: orphans only
- FAIL: broken refs or missing pages
```

## Aturan

- **Read-only** — tidak modify apapun
- Hanya treat `[[double-bracket]]` sebagai wiki refs; skip `[regular](markdown)` links
- `README.md` exempt dari orphan check
- Flash cukup (read + regex, no reasoning needed)
- Jika `.gemini/wiki/` tidak ada: exit cleanly dengan message, bukan error
