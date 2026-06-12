#反重力スターター 🛰️

<div align="center">
  <a href="README.md">English</a> | <a href="README.id.md">Bahasa Indonesia</a> | <a href="README.zh.md">简体中文</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.fr-ca.md">Français (CA)</a> | <a href="README.de.md">Deutsch</a> | <a href="README.fr.md">Français</a> | <a href="README.pt-br.md">Português (BR)</a> | <a href="README.vi.md">Tiếng Việt</a> | <a href="README.pl.md">Polski</a> | <strong>日本語</strong> | <a href="README.ko.md">한국어</a> | <a href="README.es.md">Español</a> | <a href="README.tr.md">Türkçe</a> | <a href="README.it.md">Italiano</a> | <a href="README.ru.md">Русский</a> | <a href="README.uk.md">Українська</a> | <a href="README.nl.md">Nederlands</a>
</div>

<br />

<div align="center">
  <h3><strong>AI エージェントは非常に賢いです。しかし、乱雑な作業スペースでは目が見えません。</strong></h3>
  <p><strong>Antigravity Starter は、AI エディターに完璧なビジョンを提供する、純粋な AI ファーストの Next.js 16 サンドボックスです。</strong></p>

  <p>トークンを無駄にしたり、AI の幻覚に悩まされたり、乱雑なフォルダー構造に悩まされたりするのはもうやめましょう。 AI を使用したコーディングは魔法のように感じられるはずですが、今では魔法のように感じられます。</p>
</div>

> 📦 **andiupn** による無料テンプレート ([kuncimu.com](https://kuncimu.com)) · [MIT ライセンス](LICENSE) に基づいてライセンスされています  
> ☕ 役に立ったら、[コーヒーを買ってきてください](https://ko-fi.com/andiupn) · 🚀 ステータス優先のマルチプロジェクトのモノリポジトリが必要ですか? [PRO バージョン](https://github.com/sponsors/andiupn?frequency=monthly) をお試しください

__バッジ_0__
__バッジ_1__
__バッジ_2__
__バッジ_3__
__バッジ_4__
__バッジ_5__

---

## 💡 問題: 従来のワークスペースが AI に失敗する理由
AI エージェント (カーソル、ジェミニ、クロード) は驚異的な能力を持っています。しかし、標準の乱雑なディレクトリにドロップすると、紛失してしまいます。明確な境界がないため、無関係なフォルダーを読み取り、トークンの予算を使い果たし、幻覚を起こし、ファイルを間違ったディレクトリに配置します。

---

## ⚡ ソリューション: プレミアム AI 足場の 3 つの柱

### 1. 🛰️ AI に最適なビジョン (AI ファーストのレイアウト)
すべてのフォルダー、構成、`.gitignore` ルールは、AI のロードマップとして機能するように設計されています。ワークスペースは非常にクリーンなので、Cursor または Gemini は **Next.js 16 + React 19 + Tailwind v4** アーキテクチャ全体を 3 秒以内に理解できます。無駄なトークンはゼロ、最高の精度。

### 2. 🤖 一般的なチャットボットではなく専門チーム
空の AI ボックスに話しかけることはできません。事前に構成された 2 つの高度に専門化された自律型 AI エージェントのチームが得られます。
- **`@code-reviewer`** — コミット前にコードの品質、リント、構造をレビューする厳密かつ厳密な QA チーム。
- **`@research-assistant`** — 新しい API ドキュメントとライブラリを安全に探索できるように調整された、高速でコスト効率の高いリサーチ エージェント。

### 3. ⚡ ワンクリックスキル (ワークフロー)
複雑な開発ワークフローを簡単なコマンドで実行します。手動のスキャフォールディング、環境チェック、テスト作成を 1 秒のタスクに変える 8 つの再利用可能な自動化ワークフロー (`/skills`) が装備されています。

---

## 📊 LITE vs PRO: プレミアムアップグレード

|あなたにできること | 🆓 ライト (無料) | 💎PRO (有料) |
|---|:---:|:---:|
| **専門エージェント** | 2 | 5 (+ プランナー、アーキテクチャ、セキュリティ) |
| **ワークフロー スキル** | 8 | 23 (+ Drizzle 同期、Docker、ルール監査など) |
| **ワークスペースの構造** |シンプル (`src/`、`docs/`) |ステータス優先のモノリポジトリ (`active/`、`staging/` など) |
| **運用準備完了構成** | ❌ | ✅ (Docker Compose、Caddyfile) |
| **プロジェクトのプリセット** | 1 (Next.js) | 4 (次のアプリ、SPA、Laravel、Flutter) |

👉 **[全機能の比較とアップグレード ガイドを表示](COMPARISON.md)**

---

## 📂 ワークスペースのブループリント

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

## 🚀 3 ステップで始めましょう

### 1. 構成をコピーします。

```bash
cp .env.example .env
```

*(リポジトリ統合を有効にするには、`GITHUB_TOKEN` を挿入します)。*

### 2. AI 権限をセットアップします。

```bash
cp .gemini/settings.local.example.json .gemini/settings.local.json
```

*(コメントを解除し、OS に応じて `permissions` を設定します)。*

### 3. コーディングを開始します。
お気に入りの AI 対応エディターでこのワークスペースを開いて、そのスピードを体験してください。

---

## 💖 このプロジェクトをサポートする (寄付)

このテンプレートによりコーディング ワークフローが高速化された場合は、以下のサポートを検討してください。
- **Ko-fi:** [ko-fi.com/andiupn](https://ko-fi.com/andiupn)
- **Patreon:** [patreon.com/AndiUpn](https://patreon.com/AndiUpn)
- **Trakteer:** [trakteer.id/andi_upn/gift](https://trakteer.id/andi_upn/gift)
- **サウェリア:** [saweria.co/andiupn](https://saweria.co/andiupn)

---

## 📄 ライセンス

このプロジェクトは **MIT ライセンス** に基づいてライセンスされています。 See the [LICENSE](LICENSE) file for more information.