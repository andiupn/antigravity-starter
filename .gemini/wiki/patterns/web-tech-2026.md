# Web Technology Standard 2026 (Mid-Year)

Dokumen ini mendefinisikan standar teknis utama untuk pengembangan aplikasi web di workspace ini, divalidasi sebagai stack paling optimal untuk kolaborasi dengan AI Agent.

## Core Tech Stack

- **Framework:** Next.js 16.x (App Router)
- **Library Utama:** React 19.x
- **Bahasa:** TypeScript 5.x (Strict Mode: ON)
- **Styling:** Tailwind CSS v4 (Oxide engine)
- **Database ORM:** Drizzle ORM (SQL-transparent)
- **Runtime Validation:** Zod
- **AI Integration:** Vercel AI SDK
- **Deployment:** Vercel (Primary)

## Prinsip Pengembangan (AI-Friendly)

1. **End-to-End Type Safety:** Data dari database hingga UI harus ter-typing secara ketat. Dilarang menggunakan `any`.
2. **Predictable Execution:** Gunakan Server Components (RSC) secara default. Batasan Client/Server harus eksplisit.
3. **Explicit Data Boundaries:** Validasi semua input (props, API, DB) menggunakan Zod schema.
4. **Transparency:** Gunakan Drizzle untuk memastikan query database dapat dibaca dan dipahami oleh AI Agent tanpa abstraksi berlebih (seperti Prisma).
5. **Native Streaming:** Manfaatkan streaming response untuk fitur AI agar memberikan feedback instan.

## Struktur File Standar

- `app/`: Next.js App Router.
- `src/db/`: Skema Drizzle dan konfigurasi database.
- `src/components/`: UI components (preferensi: shadcn/ui).
- `src/lib/`: Utilities dan Zod schemas.
- `src/app/actions.ts`: Server Actions untuk mutasi data.

## Performance Targets

- **LCP:** < 1.0s
- **Build Time:** < 100ms (incremental)
- **Bundle Size:** < 50KB (base JS)
- **Type Safety:** 99%+ coverage

---
*Diadopsi pada: 29 Mei 2026*
*Sumber: Research Artifacts Mid-2026*
