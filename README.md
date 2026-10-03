# awesome-techdou-skills

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

### 🤖 AI Models & Delegation | 模型调用与委派

| Skill | Description | Repo |
|---|---|---|
| **coze-ai-models** | Full Coze model suite adapter: LLM chat/streaming/vision, Seedream image generation, Seedance video (first/last frame, multimodal refs), TTS/ASR, embeddings. Sandbox SDK or local OpenAI-compatible calling. | [techdou/coze-ai-models](https://github.com/techdou/coze-ai-models) |
| **codex-delegate** | Delegate bounded work to the local OpenAI Codex CLI. Model discovery/selection, reasoning control, session continuity, cache-aware repeated review/writing. | [techdou/codex-delegate](https://github.com/techdou/codex-delegate) |
| **gemini-delegate** | Delegate bounded work to the local Google Gemini CLI (Antigravity-first, Gemini CLI fallback). Model probing, thinking control, session continuity, PDF/multimodal review. | [techdou/gemini-delegate](https://github.com/techdou/gemini-delegate) |

### 📚 Academic Research | 学术研究

| Skill | Description | Repo |
|---|---|---|
| **download-paper-collection** | Batch-download papers from heterogeneous Excel lists. Auto-detects schema, merges PDF/URL/DOI/arXiv, validates integrity, produces auditable manifests. | [techdou/download-paper-collection](https://github.com/techdou/download-paper-collection) |
| **paper-reading** | Purpose-first interpretation of a specific paper (or a named comparison set): two-pass reading, experiment-first review, structured HTML with KaTeX formulas, Mermaid diagrams, and annotation write-back. v1.1.0 — tightened agent routing with 7 reading modes. *Forked from Agentchengfeng/paper-reading-skills (Apache-2.0).* | [techdou/paper-reading](https://github.com/techdou/paper-reading) |
| **mono-diagram** | Pure black-on-white academic diagrams. Mermaid/SVG sources, lint for print safety, high-res PNG output for Word/PDF. | [techdou/mono-diagram](https://github.com/techdou/mono-diagram) |
| **omml-formula-skill** | Convert LaTeX formulas into editable Office Math (OMML) in Word/PowerPoint — not screenshots or garbled text. | [techdou/omml-formula-skill](https://github.com/techdou/omml-formula-skill) |
| **research-paper-hub** | Single front door for paper-research workflows. Routes 30 vendor-locked playbooks across CCF-A and Nature tracks — literature search, deep reading, idea review, experiment design, writing, review, rebuttal — with persistent `.research/` project state. | [techdou/research-paper-hub](https://github.com/techdou/research-paper-hub) |
| **visualization-innovation** | Mechanism-level research-visualization innovation: chart redesign, new chart families, interaction and coordinated-view innovation, evidence-based visual stories, prior-art-aware novelty claims. | [techdou/visualization-innovation](https://github.com/techdou/visualization-innovation) |
| **research-visual-analytics** | Design and audit scientific visual-analysis workspaces: task-to-view architecture, encoding correctness, coordination contracts, statistical integrity, reproducible interaction. | [techdou/research-visual-analytics](https://github.com/techdou/research-visual-analytics) |
| **nenu-computer-tech-proposal** | Plan, co-write, and audit NENU CS master's thesis proposals — six modes (guiding / co-writing / diagnosis / evidence / defense / final review), evidence-first verification, no fabricated citations or data. *Private, personal use.* | [techdou/nenu-computer-tech-proposal](https://github.com/techdou/nenu-computer-tech-proposal) |

### 🎓 Education & Teaching | 教育教学

| Skill | Description | Repo |
|---|---|---|
| **classroom-annotator** | Three-level annotation of classroom teaching videos — operation / behavior / activity — exported to xlsx. AI pre-annotation with human-in-the-loop correction. | [techdou/classroom-annotator](https://github.com/techdou/classroom-annotator) |

### 🎬 Video Generation | 视频生成

| Skill | Description | Repo |
|---|---|---|
| **remotion-video** | SRT → Remotion video pipeline. MCP server (17 tools), async queue, multi-provider TTS, React web console. *Adapted from YangAgent's B站 sharing.* | [techdou/remotion-video](https://github.com/techdou/remotion-video) |
| **whiteboard-video** | Whiteboard hand-drawn video generator. Three modes: SRT → full video, batch images, single image. *Adapted from YangAgent's B站 sharing.* | [techdou/whiteboard-video](https://github.com/techdou/whiteboard-video) |
| **ai-promo-video** | End-to-end AI promo video pipeline. Model research, marketing copy, voiceover scripts, shot-by-shot prompts for seedance/Sora/Kling/Runway/HeyGen. | [techdou/ai-promo-video](https://github.com/techdou/ai-promo-video) |
| **agnes-ai-generation-skill** | Call Agnes AI / Sapiens AI generation APIs for text, image, and video. | [techdou/agnes-ai-generation-skill](https://github.com/techdou/agnes-ai-generation-skill) |
| **boson-ai-skill** | Boson AI Higgs TTS 3 + Higgs Avatar. 102-language speech, voice cloning, talking-head avatar videos. | [techdou/boson-ai-skill](https://github.com/techdou/boson-ai-skill) |
| **dou-ai-course-video** | Course video editing template — full ChatCut workflow from raw lecture to polished cut. | [techdou/dou-ai-course-video](https://github.com/techdou/dou-ai-course-video) |
| **koubo-clean** | Talking-head video cleanup spec — trim only stumbles and fillers, never delete content. | [techdou/koubo-clean](https://github.com/techdou/koubo-clean) |
| **relay-studio-media** | AI image/video generation via Relay Studio reverse proxy (Seedream/Seedance). Capability-aware routing + deterministic stdlib wrapper. | [techdou/relay-studio-media](https://github.com/techdou/relay-studio-media) |

### 🎨 Image & Visual | 图像与视觉

| Skill | Description | Repo |
|---|---|---|
| **image2-api** | Generate and edit images through OpenAI-compatible Images API or GPT Image 2 relay. Multi-provider fallback, structured prompt compilation, reproducible metadata. | [techdou/image2-api](https://github.com/techdou/image2-api) |
| **edu-image-prompt** | Turn knowledge points into ready-to-paste AI image generation prompts. Education-optimized, reliable Chinese rendering. | [techdou/edu-image-prompt](https://github.com/techdou/edu-image-prompt) |
| **douip-illustrations** | DouKnowAI branded editorial illustrations. Orange coffee-bean IP for 公众号/小红书/博客/课程. *Adapted from helloianneo/ian-xiaohei-illustrations (MIT).* | [techdou/douip-illustrations](https://github.com/techdou/douip-illustrations) |
| **remove-checkerboard** | Remove fake checkerboard backgrounds (AI fake transparency) and solid/white backgrounds. Auto-detects, produces real transparent PNGs. | [techdou/remove-checkerboard](https://github.com/techdou/remove-checkerboard) |
| **pet-reskin** | Generate and install complete canvas-pet character skins. Supports single/multi-skin architectures, Gemini/image2-api providers. | [techdou/pet-reskin](https://github.com/techdou/pet-reskin) |

### 🔊 Audio & Speech | 音频语音

| Skill | Description | Repo |
|---|---|---|
| **mimo-audio-skill** | Convert lecture notes/scripts into MiMo voice broadcast audio. Modular: TTS core + optional HTML player, subtitles, ASR QA, packaging. | [techdou/mimo-audio-skill](https://github.com/techdou/mimo-audio-skill) |
| **media-transcribe** | Local audio/video transcription and timestamp workflow (Qwen3-ASR). Data never leaves your machine. | [techdou/media-transcribe](https://github.com/techdou/media-transcribe) |
| **poly-tts** | Local zero-shot voice-cloning TTS for macOS Apple Silicon — CosyVoice3 wrapper. Review-hardened: atomic output, single-instance lock, resumable install. | [techdou/poly-tts](https://github.com/techdou/poly-tts) |
| **qqmusic-decrypt** | Decrypt QQ Music exclusive encrypted audio (.mflac/.mgg/.qmc* families) to lossless FLAC/OGG or 320k MP3, for personal backups of owned music. | [techdou/qqmusic-decrypt](https://github.com/techdou/qqmusic-decrypt) |

### 📝 Document & Publishing | 文档与发布

| Skill | Description | Repo |
|---|---|---|
| **interactive-doc-builder** | Convert long technical content into interactive single-file HTML dashboards. Dark mode, search, dictionary popovers. | [techdou/interactive-doc-builder](https://github.com/techdou/interactive-doc-builder) |
| **html-asset-toolkit** | Package HTML and static frontend builds into one portable single-file HTML. Double-click to open, zero external files. | [techdou/html-asset-toolkit](https://github.com/techdou/html-asset-toolkit) |
| **typora-html-enhancer** | Inject modern UI enhancements into Typora/Markdown HTML exports. Sidebar TOC, multi-theme, reading progress bar, mobile responsive. | [techdou/typora-html-enhancer](https://github.com/techdou/typora-html-enhancer) |
| **md-image-uploader** | Batch-upload local images in Markdown/HTML to image hosts (R2/OSS/COS/Qiniu/MinIO/B2) and rewrite paths to CDN URLs. | [techdou/md-image-uploader](https://github.com/techdou/md-image-uploader) |
| **surge-publish** | Publish static web projects to surge.sh CDN. Pre-flight checks, non-interactive publishing, revisions/rollback, custom domains. | [techdou/surge-publish](https://github.com/techdou/surge-publish) |
| **dou-tone** | Personal Chinese writing, rewriting and polishing skill: proofreading, tone-preserving polish, rewriting, genre conversion, drafting from materials. L1–L5 edit levels with scene references for reports / academia / teaching / PPT / 公众号. | [techdou/dou-tone](https://github.com/techdou/dou-tone) |
| **ppt-studio** | Fully offline PPT / slides / poster creation for agents — python-pptx local engine, PPTD format, PowerPoint COM visual QA, zero-dependency viewer, OMML formula rendering (pairs with omml-formula-skill). | [techdou/ppt-studio](https://github.com/techdou/ppt-studio) |

### 🛠️ Development Tools | 开发工具

| Skill | Description | Repo |
|---|---|---|
| **developing-coze-apps** | Plan, build, review, and package Coze Coding (扣子编程) apps, incl. single-HTML/iframe delivery. | [techdou/developing-coze-apps](https://github.com/techdou/developing-coze-apps) |
| **cf-ops** | Cloudflare's next-gen `cf` CLI (wrangler successor) usage skill. Safe search → schema → dry-run workflow over the full Cloudflare API: DNS, zones, Workers, WAF, R2/D1/KV. Beta pitfalls documented (silent abort on exit 0, --force ambiguity). | [techdou/cf-ops](https://github.com/techdou/cf-ops) |
| **wsl-operations** | Operate WSL/WSL2 from Windows: distro lifecycle, `.wslconfig`/`wsl.conf`/systemd, repair, Windows↔Linux interop, Python/Node/Docker/CUDA environments, experiments, health checks. Doctor scripts included. | [techdou/wsl-operations](https://github.com/techdou/wsl-operations) |

### 🔌 Integrations | 集成接入

| Skill | Description | Repo |
|---|---|---|
| **feishu-bitable** | Wire forms/data into Feishu Bitable end-to-end: self-built app setup, two-layer permissions (app scope + bot collaborator), four-key `.env` config, TypeScript wiring reference, probe self-check. Same pattern fits GitHub/Notion/钉钉 integrations. | [techdou/feishu-bitable](https://github.com/techdou/feishu-bitable) |
| **github-workspace-bridge** | Safely attach local/sandbox/Coze projects to your GitHub identity: multi-account PAT registry, clone/bootstrap/sync, origin/upstream hygiene, ZIP-to-git init. *Private (douknowai), personal use.* | [douknowai/github-workspace-bridge](https://github.com/douknowai/github-workspace-bridge) |

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

- **共 42 个 skill**，覆盖模型调用与委派、学术研究、教育教学、视频生成、图像处理、音频语音、文档发布、开发工具、集成接入、存储基础设施 10 大领域
- 兼容 ZCode、Claude Code、OpenAI Codex、OpenCode 等 Agent 客户端
- README 统一风格：一句话定位 / 安装与更新 / 使用 / 场景参考 / 维护与来源
- 敏感信息（API 密钥、.env）严格通过 `.gitignore` 排除，已全部验证无泄露

---

## License | 协议

每个 skill 沿用各自仓库的协议（多数为 MIT，paper-reading 为 Apache-2.0）。本索引仓库本身采用 MIT。

## Author | 作者

**TechDou / 豆懂AI**
- GitHub: [@techdou](https://github.com/techdou)
- Brand: DouKnowAI / 豆懂AI
