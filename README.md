# awesome-techdou-skills

> A curated index of portable Agent Skills built by [@techdou](https://github.com/techdou) (DouKnowAI / 豆懂AI).
>
> 由 [@techdou](https://github.com/techdou)（DouKnowAI / 豆懂AI）打造的可移植 Agent Skill 索引合集。

[English](#english) | [中文](#中文)

---

<a id="english"></a>
## English

Each skill lives in its **own independent repository** (linked below). This repo is an index only — it does not duplicate code. Skills are portable and work with ZCode, Claude Code, OpenAI Codex, OpenCode, and compatible Agent clients.

### Why an index repo?

- One place to discover all skills, organized by domain
- Each skill remains independently versioned in its own repo
- No code duplication, no submodule sync headaches

### Install a skill

```bash
# Clone the skill you need into your Agent's skills directory
git clone https://github.com/techdou/<skill-name>.git ~/.agents/skills/<skill-name>
```

Refer to each skill's own README for dependencies and configuration.

---

## Skill Catalog | Skill 目录

### 📚 Academic Research | 学术研究

| Skill | Description | Repo |
|---|---|---|
| **download-paper-collection** | Batch-download papers from heterogeneous Excel lists. Auto-detects schema, merges PDF/URL/DOI/arXiv, validates integrity, produces auditable manifests. | [techdou/download-paper-collection](https://github.com/techdou/download-paper-collection) |
| **paper-reading** | Purpose-first paper interpretation into structured long-form HTML with KaTeX formulas, Mermaid diagrams, and annotation write-back. *Forked from Agentchengfeng/paper-reading-skills (Apache-2.0).* | [techdou/paper-reading](https://github.com/techdou/paper-reading) |
| **mono-diagram** | Pure black-on-white academic diagrams. Mermaid/SVG sources, lint for print safety, high-res PNG output for Word/PDF. | [techdou/mono-diagram](https://github.com/techdou/mono-diagram) |
| **omml-formula-skill** | Convert LaTeX formulas into editable Office Math (OMML) in Word/PowerPoint — not screenshots or garbled text. | [techdou/omml-formula-skill](https://github.com/techdou/omml-formula-skill) |

### 🎬 Video Generation | 视频生成

| Skill | Description | Repo |
|---|---|---|
| **remotion-video** | SRT → Remotion video pipeline. MCP server (17 tools), async queue, multi-provider TTS, React web console. *Adapted from YangAgent's B站 sharing.* | [techdou/remotion-video](https://github.com/techdou/remotion-video) |
| **whiteboard-video** | Whiteboard hand-drawn video generator. Three modes: SRT → full video, batch images, single image. *Adapted from YangAgent's B站 sharing.* | [techdou/whiteboard-video](https://github.com/techdou/whiteboard-video) |
| **ai-promo-video** | End-to-end AI promo video pipeline. Model research, marketing copy, voiceover scripts, shot-by-shot prompts for seedance/Sora/Kling/Runway/HeyGen. | [techdou/ai-promo-video](https://github.com/techdou/ai-promo-video) |
| **agnes-ai-generation-skill** | Call Agnes AI / Sapiens AI generation APIs for text, image, and video. | [techdou/agnes-ai-generation-skill](https://github.com/techdou/agnes-ai-generation-skill) |
| **boson-ai-skill** | Boson AI Higgs TTS 3 + Higgs Avatar. 102-language speech, voice cloning, talking-head avatar videos. | [techdou/boson-ai-skill](https://github.com/techdou/boson-ai-skill) |

### 🎨 Image & Visual | 图像与视觉

| Skill | Description | Repo |
|---|---|---|
| **image2-api** | Generate and edit images through OpenAI-compatible Images API or GPT Image 2 relay. | [techdou/image2-api](https://github.com/techdou/image2-api) |
| **edu-image-prompt** | Turn knowledge points into ready-to-paste AI image generation prompts. Education-optimized, reliable Chinese rendering. | [techdou/edu-image-prompt](https://github.com/techdou/edu-image-prompt) |
| **douip-illustrations** | DouKnowAI branded editorial illustrations. Orange coffee-bean IP for 公众号/小红书/博客/课程. *Adapted from helloianneo/ian-xiaohei-illustrations (MIT).* | [techdou/douip-illustrations](https://github.com/techdou/douip-illustrations) |
| **remove-checkerboard** | Remove fake checkerboard backgrounds (AI fake transparency) and solid/white backgrounds. Auto-detects, produces real transparent PNGs. | [techdou/remove-checkerboard](https://github.com/techdou/remove-checkerboard) |
| **pet-reskin** | Generate and install complete canvas-pet character skins. Supports single/multi-skin architectures, Gemini/image2-api providers. | [techdou/pet-reskin](https://github.com/techdou/pet-reskin) |

### 🔊 Audio & Speech | 音频语音

| Skill | Description | Repo |
|---|---|---|
| **mimo-lecture-audio-skill** | Convert lecture notes/scripts into MiMo voice broadcast audio. Modular: TTS core + optional HTML player, subtitles, ASR QA, packaging. | [techdou/mimo-lecture-audio-skill](https://github.com/techdou/mimo-lecture-audio-skill) |

### 📝 Document & Publishing | 文档与发布

| Skill | Description | Repo |
|---|---|---|
| **interactive-doc-builder** | Convert long technical content into interactive single-file HTML dashboards. Dark mode, search, dictionary popovers. | [techdou/interactive-doc-builder](https://github.com/techdou/interactive-doc-builder) |
| **html-asset-toolkit** | Package HTML and static frontend builds into one portable single-file HTML. Double-click to open, zero external files. | [techdou/html-asset-toolkit](https://github.com/techdou/html-asset-toolkit) |
| **typora-html-enhancer** | Inject modern UI enhancements into Typora/Markdown HTML exports. Sidebar TOC, multi-theme, reading progress bar, mobile responsive. | [techdou/typora-html-enhancer](https://github.com/techdou/typora-html-enhancer) |
| **md-image-uploader** | Batch-upload local images in Markdown/HTML to image hosts (R2/OSS/COS/Qiniu/MinIO/B2) and rewrite paths to CDN URLs. | [techdou/md-image-uploader](https://github.com/techdou/md-image-uploader) |
| **surge-publish** | Publish static web projects to surge.sh CDN. Pre-flight checks, non-interactive publishing, revisions/rollback, custom domains. | [techdou/surge-publish](https://github.com/techdou/surge-publish) |

### 🗄️ Storage & Infrastructure | 存储与基础设施

| Skill | Description | Repo |
|---|---|---|
| **objstore** | S3-compatible object store client. AWS S3 / R2 / OSS / COS / MinIO / B2 / Wasabi. Bucket CRUD, sync, pre-signed URLs, multi-profile credentials. | [techdou/objstore](https://github.com/techdou/objstore) |

---

<a id="中文"></a>
## 中文

每个 skill 都有**独立仓库**（见下方链接），本仓库仅做索引——不重复代码。所有 skill 可移植，兼容 ZCode、Claude Code、OpenAI Codex、OpenCode 等 Agent 客户端。

### 为什么用索引型仓库？

- 一个地方发现所有 skill，按领域分类
- 每个 skill 在自己的仓库里独立版本管理
- 无代码重复，无 submodule 同步麻烦

### 安装某个 skill

```bash
# 把需要的 skill 克隆到 Agent 的 skills 目录
git clone https://github.com/techdou/<skill-name>.git ~/.agents/skills/<skill-name>
```

具体依赖和配置见各 skill 自己的 README。

---

## 统计

- **共 21 个 skill**，覆盖学术研究、视频生成、图像处理、音频语音、文档发布、存储基础设施 6 大领域
- 全部支持中英双语 README
- 敏感信息（API 密钥、.env）严格通过 `.gitignore` 排除，已全部验证无泄露

---

## License | 协议

每个 skill 沿用各自仓库的协议（多数为 MIT，paper-reading 为 Apache-2.0）。本索引仓库本身采用 MIT。

## Author | 作者

**TechDou / 豆懂AI**
- GitHub: [@techdou](https://github.com/techdou)
- Brand: DouKnowAI / 豆懂AI
