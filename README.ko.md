# 반중력 스타터 🛰️

<div align="center">
  <a href="README.md">English</a> | <a href="README.id.md">Bahasa Indonesia</a> | <a href="README.zh.md">简体中文</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.fr-ca.md">Français (CA)</a> | <a href="README.de.md">Deutsch</a> | <a href="README.fr.md">Français</a> | <a href="README.pt-br.md">Português (BR)</a> | <a href="README.vi.md">Tiếng Việt</a> | <a href="README.pl.md">Polski</a> | <a href="README.ja.md">日本語</a> | <strong>한국어</strong> | <a href="README.es.md">Español</a> | <a href="README.tr.md">Türkçe</a> | <a href="README.it.md">Italiano</a> | <a href="README.ru.md">Русский</a> | <a href="README.uk.md">Українська</a> | <a href="README.nl.md">Nederlands</a>
</div>

<br />

<div align="center">
  <h3><strong>AI 에이전트는 놀라울 정도로 똑똑합니다. 하지만 그들은 지저분한 작업 공간에서 눈이 멀었습니다.</strong></h3>
  <p><strong>Antgravity Starter는 AI 편집자에게 완벽한 비전을 제공하는 깨끗한 AI 우선 Next.js 16 샌드박스입니다.</strong></p>

  <p>토큰 낭비, AI 환각, 지저분한 폴더 구조로 인한 어려움을 중지하세요. AI를 사용한 코딩은 마치 마법처럼 느껴져야 합니다. 이제 실제로 그렇습니다.</p>
</div>

> 📦 **andiupn**([kuncimu.com](https://kuncimu.com))의 무료 템플릿 · [MIT 라이선스](LICENSE)에 따라 라이선스가 부여됨  
> 😄 도움이 되셨다면 [커피 사주세요](https://ko-fi.com/andiupn) · 🚀 상태 우선 다중 프로젝트 모노레포가 필요하신가요? [PRO 버전](https://github.com/sponsors/andiupn?frequency=monthly)을 사용해 보세요.

__배지_0__
__배지_1__
__배지_2__
__배지_3__
__배지_4__
__배지_5__

---

## 💡 문제: 기존 작업 공간이 AI에 실패하는 이유
AI 에이전트(Cursor, Gemini, Claude)는 놀라울 정도로 능력이 뛰어납니다. 그러나 표준적이고 어수선한 디렉토리에 넣으면 길을 잃습니다. 그들은 관련 없는 폴더를 읽고, 토큰 예산을 날려버리고, 환각을 느끼고, 명확한 경계가 없기 때문에 잘못된 디렉터리에 파일을 배치합니다.

---

## ⚡ 솔루션: 프리미엄 AI 비계의 세 가지 기둥

### 1. 🛰️ AI를 위한 완벽한 비전(AI-First 레이아웃)
우리는 AI의 로드맵 역할을 하도록 모든 폴더, 구성 및 `.gitignore` 규칙을 설계했습니다. 작업 공간은 매우 깔끔하여 Cursor 또는 Gemini가 전체 **Next.js 16 + React 19 + Tailwind v4** 아키텍처를 3초 이내에 이해할 수 있습니다. 낭비되는 토큰이 없고 정확도가 극대화됩니다.

### 2. 🤖 일반 챗봇이 아닌 전문팀
빈 AI 상자와 대화하지 마세요. 사전 구성되고 고도로 전문화된 자율 AI 에이전트 2개로 구성된 팀이 구성됩니다.
- **`@code-reviewer`** — 커밋 전에 코드 품질, 린트 및 구조를 검토하는 엄격하고 엄격한 QA 팀입니다.
- **`@research-assistant`** — 새로운 API 문서와 라이브러리를 안전하게 탐색하도록 맞춤화된 고속의 비용 효율적인 연구 에이전트입니다.

### 3. ⚡ 원클릭 기술(워크플로)
간단한 명령으로 복잡한 개발 워크플로를 실행하세요. 수동 스캐폴딩, 환경 확인, 테스트 작성을 1초 작업으로 전환하는 재사용 가능한 자동화 워크플로(`/skills`) 8개를 갖추고 있습니다.

---

## 📊 LITE 대 PRO: 프리미엄 업그레이드

| 당신이 할 수 있는 일 | 🆓 LITE(무료) | 💎 PRO(유료) |
|---|:---:|:---:|
| **전문 에이전트** | 2 | 5 (+ 플래너, 아키텍처, 보안) |
| **워크플로 기술** | 8 | 23(+ Drizzle 동기화, Docker, 규칙 감사 등) |
| **작업공간 구조** | 단순(`src/`, `docs/`) | 상태 우선 모노레포(`active/`, `staging/` 등) |
| **운영 준비 구성** | ❌ | ✅ (Docker Compose, Caddyfile) |
| **프로젝트 사전 설정** | 1(Next.js) | 4(다음 앱, SPA, Laravel, Flutter) |

👉 **[전체 기능 비교 및 업그레이드 가이드 보기](COMPARISON.md)**

---

## 📂 작업 공간 청사진

```
your-workspace/
  .gemini/             # AI agent configs, automation skills, and wiki
  docs/                # Pristine research and implementation plans
  src/                 # Main directory for your application source code
  .env.example         # Template for environment variables
  .gitignore           # Standard Git ignore file
  .mcp.json            # Model Context Protocol (MCP) configuration
  GEMINI.md            # AI coding rules & workspace guidelines
  LICENSE              # Project license (MIT License)
```

---

## 🚀 3단계로 시작하기

### 1. 구성 복사:

```bash
cp .env.example .env
```

*(저장소 통합을 활성화하려면 `GITHUB_TOKEN`을 삽입하세요).*

### 2. AI 권한 설정:

```bash
cp .gemini/settings.local.example.json .gemini/settings.local.json
```

*(주석을 해제하고 OS에 따라 `permissions`을 설정하세요).*

### 3. 코딩 시작:
선호하는 AI 친화적인 편집기에서 이 작업 공간을 열고 속도를 경험해 보세요.

---

## 💖 이 프로젝트를 후원하세요(기부)

이 템플릿으로 코딩 작업 흐름이 가속화된 경우 다음 지원을 고려해보세요.
- **Ko-fi:** [ko-fi.com/andiupn](https://ko-fi.com/andiupn)
- **Patreon:** [patreon.com/AndiUpn](https://patreon.com/AndiUpn)
- **트랙티어:** [trakteer.id/andi_upn/gift](https://trakteer.id/andi_upn/gift)
- **사웨리아:** [saweria.co/andiupn](https://saweria.co/andiupn)

---

## 📄 라이선스

이 프로젝트는 **MIT 라이선스**에 따라 라이선스가 부여됩니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.