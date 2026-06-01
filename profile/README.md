<div align="center">

# ቆንጆ &nbsp;Konjo AI

### The open infrastructure layer for AI 🧱

![konjo banner](https://github.com/user-attachments/assets/fd55d13d-f747-447f-a979-34b3734c9d76)

<br/>

[![Website](https://img.shields.io/badge/🌐_konjotech.com-0A0A0A?style=for-the-badge)](https://konjotech.com)
[![X / Twitter](https://img.shields.io/badge/𝕏_@wesley__scholl-0A0A0A?style=for-the-badge)](https://x.com/wesley_scholl)
[![Followers](https://img.shields.io/github/followers/konjoai?style=for-the-badge&logo=github&label=Follow&labelColor=0A0A0A&color=4F46E5)](https://github.com/konjoai)
[![License](https://img.shields.io/badge/License-MIT-4F46E5?style=for-the-badge)](https://github.com/konjoai)

<br/>

**KONJO** — **K**now · **O**utline · **N**ail · **J**ustify · **O**ptimize

> 🇪🇹 **ቆንጆ** *Beautiful* &nbsp;·&nbsp; 🇯🇵 **根性** *Fighting spirit* &nbsp;·&nbsp; 🀄 **康宙** *Health of the universe* &nbsp;·&nbsp; 🇳🇵 **खोजो** *Search & discover*

***Make it Konjo — Plan, build, test, ship, rest, repeat.*** 🔁

</div>

---

<div align="center">

*Konjo is the word you reach for when a tool does exactly what it needs to do — nothing more, nothing less.*

</div>

We build the **open infrastructure layer for AI**. Not wrappers, not prompt chains — the deep systems that power them: compression, inference, vector engines, memory architectures, compliance, and the research that pushes the whole stack forward. **Vertically integrated, benchmark-driven, built in public.** 🛠️

<div align="center">

### ⚡ By the numbers

| 🚀 **12M+** vec/s | ⚡ **4.85×** faster than FAISS C++ | ❄️ **54×** faster cold starts | 🎯 **recall@10 = 0.920** |
|:---:|:---:|:---:|:---:|

</div>

---

## 🏗️ The Stack

```
┌──────────────────────────────────────────────────────────────┐
│  🧠  Orchestration                                            │
│        lopi (Agent Orchestrator)  ·  kyro (RAG)              │
├──────────────────────────────────────────────────────────────┤
│  ⚙️  Inference Layer                                          │
│        squish (Local LLMs)  ·  kairu (Speculative)          │
├──────────────────────────────────────────────────────────────┤
│  🔍  Retrieval Layer                                          │
│        vectro (Vectors)  ·  kohaku (Memory)                 │
├──────────────────────────────────────────────────────────────┤
│  🔬  Research & Compliance                                    │
│    drex (Architecture) · toki (Robustness) · miru (XAI)     │
│                    squash (EU AI Act)                        │
└──────────────────────────────────────────────────────────────┘
```

---

## 📦 Projects

### ⚙️ Inference & Compression

<table>
<tr><td width="50%" valign="top">

#### 🗜️ [squish](https://github.com/konjoai/squish)

**Compress local LLMs once. Run them forever.**

OpenAI + Ollama drop-in for Apple Silicon with statistically identical accuracy and **54× faster cold starts**. INT8/INT4/AQLM quantization, MLX-native, sub-second load times.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
[![Stars](https://img.shields.io/github/stars/konjoai/squish?style=flat-square&logo=github&label=%E2%98%85&labelColor=0A0A0A&color=4F46E5)](https://github.com/konjoai/squish)

`quantization` `apple-silicon` `mlx` `local-llm` `ollama`

</td><td width="50%" valign="top">

#### 🔮 [kairu](https://github.com/konjoai/kairu)

**Speculative decoding engine for HuggingFace models.**

EAGLE-style drafting, dynamic early exit, and token budget control with a live performance dashboard. Squeeze every token out of your inference budget.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
[![Stars](https://img.shields.io/github/stars/konjoai/kairu?style=flat-square&logo=github&label=%E2%98%85&labelColor=0A0A0A&color=4F46E5)](https://github.com/konjoai/kairu)

`speculative-decoding` `huggingface` `inference` `latency`

</td></tr>
</table>

### 🔍 Retrieval & Memory

<table>
<tr><td width="50%" valign="top">

#### ⚡ [vectro](https://github.com/konjoai/vectro)

**Lightning-fast embedding quantization & ANN indexing.**

**12M+ vec/s** — 4.85× faster than FAISS C++ — with a drastically smaller footprint. Sub-1ms encode, HNSW (recall@10 = 0.920), NF4/INT8/PQ, AutoQuantize, pipeline CLI, WASM.

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Mojo](https://img.shields.io/badge/Mojo-FF4F00?style=flat-square&logo=fireship&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
[![Stars](https://img.shields.io/github/stars/konjoai/vectro?style=flat-square&logo=github&label=%E2%98%85&labelColor=0A0A0A&color=4F46E5)](https://github.com/konjoai/vectro)

`rust` `mojo` `vector-search` `embeddings` `rag` `hnsw`

</td><td width="50%" valign="top">

#### 🧬 [kohaku](https://github.com/konjoai/kohaku)

**Neural episodic memory engine using HDC hypervectors.**

Stores long-term context and retrieves via associative recall — a persistent memory layer that goes *beyond* RAG. For LLMs that need to remember across sessions and tasks.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
[![Stars](https://img.shields.io/github/stars/konjoai/kohaku?style=flat-square&logo=github&label=%E2%98%85&labelColor=0A0A0A&color=4F46E5)](https://github.com/konjoai/kohaku)

`episodic-memory` `hdc` `hyperdimensional-computing` `llm`

</td></tr>
</table>

### 🧠 Orchestration & Pipelines

<table>
<tr><td width="50%" valign="top">

#### 🤖 [lopi](https://github.com/konjoai/lopi)

**High-performance orchestrator for Claude Code agents.**

Concurrent agents in git-isolated branches with retry loops, priority queuing, SQLite memory, pattern mining, scheduled tasks, and a live TUI + web dashboard. Remote control via Telegram.

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
[![Stars](https://img.shields.io/github/stars/konjoai/lopi?style=flat-square&logo=github&label=%E2%98%85&labelColor=0A0A0A&color=4F46E5)](https://github.com/konjoai/lopi)

`rust` `claude-code` `agent-orchestrator` `tokio` `tui`

</td><td width="50%" valign="top">

#### 🔗 [kyro](https://github.com/konjoai/kyro)

**Production RAG pipeline.**

Hybrid retrieval (dense + BM25 + RRF), reranking, and RAGAS evals baked in. Local-first with Squish + Vectro. Plugs into OpenAI, Anthropic, or runs fully offline.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
[![Stars](https://img.shields.io/github/stars/konjoai/kyro?style=flat-square&logo=github&label=%E2%98%85&labelColor=0A0A0A&color=4F46E5)](https://github.com/konjoai/kyro)

`rag` `hybrid-search` `bm25` `reranking` `ragas`

</td></tr>
</table>

### 🛡️ Compliance

<table>
<tr><td width="50%" valign="top">

#### ✅ [squash](https://github.com/konjoai/squash)

**Automated EU AI Act compliance for AI/ML teams.**

Annex IV docs, SBOMs (CycloneDX/SPDX), policy checks, and Sigstore-signed audit records inside your CI/CD. **Aug 2, 2026 enforcement deadline** — squash gets you there.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
[![Stars](https://img.shields.io/github/stars/konjoai/squash?style=flat-square&logo=github&label=%E2%98%85&labelColor=0A0A0A&color=4F46E5)](https://github.com/konjoai/squash)

`eu-ai-act` `sbom` `cyclonedx` `sigstore` `nist-ai-rmf`

</td><td width="50%" valign="top">

#### 🚦 [squash-action](https://github.com/konjoai/squash-action)

**AI Compliance Gate for GitHub Actions.**

EU AI Act · NIST AI RMF · ISO 42001 — one step in CI/CD. Pairs with squash.

[![Stars](https://img.shields.io/github/stars/konjoai/squash-action?style=flat-square&logo=github&label=%E2%98%85&labelColor=0A0A0A&color=4F46E5)](https://github.com/konjoai/squash-action)

🍺 Also: [**homebrew-squash**](https://github.com/konjoai/homebrew-squash) — `brew install konjoai/squash/squash-ai`

`github-actions` `compliance` `iso-42001`

</td></tr>
</table>

### 🔬 Research

<table>
<tr><td width="33%" valign="top">

#### 🧩 [drex](https://github.com/konjoai/drex)

**Next-gen neural architecture research.**

The transformer is a brilliant hack scaled past its limits. DREX is what comes next — tiered memory, sparse execution, and a learned controller that knows what to remember.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
[![Stars](https://img.shields.io/github/stars/konjoai/drex?style=flat-square&logo=github&label=%E2%98%85&labelColor=0A0A0A&color=4F46E5)](https://github.com/konjoai/drex)

`mamba` `tiered-memory` `cognitive-architecture`

</td><td width="33%" valign="top">

#### ⚔️ [toki](https://github.com/konjoai/toki)

**Adversarial fine-tuning lab for small models (1B–3B).**

Generate red-team attacks, harden via LoRA, ship datasets and robust weights. Does robustness truly generalize — or just overfit under pressure?

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
[![Stars](https://img.shields.io/github/stars/konjoai/toki?style=flat-square&logo=github&label=%E2%98%85&labelColor=0A0A0A&color=4F46E5)](https://github.com/konjoai/toki)

`red-teaming` `adversarial-ai` `lora` `alignment`

</td><td width="33%" valign="top">

#### 👁️ [miru](https://github.com/konjoai/miru)

**Multimodal reasoning tracer.**

Answers questions over images and documents while visualizing step-by-step attention and reasoning chains. See what the model sees — and why.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
[![Stars](https://img.shields.io/github/stars/konjoai/miru?style=flat-square&logo=github&label=%E2%98%85&labelColor=0A0A0A&color=4F46E5)](https://github.com/konjoai/miru)

`vlm` `multimodal` `xai` `attention`

</td></tr>
</table>

### 🎨 Design

#### 🖌️ [ui](https://github.com/konjoai/ui)

**Konjo AI design system + portfolio homepage monorepo.** &nbsp; ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) [![Stars](https://img.shields.io/github/stars/konjoai/ui?style=flat-square&logo=github&label=%E2%98%85&labelColor=0A0A0A&color=4F46E5)](https://github.com/konjoai/ui)

Packages: `ui` · Apps: `web`

---

## 🧭 Engineering Principles

We build primarily in **Rust** 🦀 and **Python** 🐍, reaching for **Mojo** 🔥 and **C++** when the metal demands it.

| | Principle | What it means |
|:---:|:---|:---|
| 🔧 | **CLI-first, pipe-friendly** | Every tool plays seamlessly with Unix workflows and CI/CD. |
| 📊 | **Show the math** | Real benchmark numbers over vibes. Latency (p50/p95/p99) + accuracy, measured constantly. |
| 🔓 | **Open specs, zero lock-in** | Built on open formats. Swap any Konjo layer for something else — the system allows it. |
| 🚀 | **Ship fast, iterate in public** | Ugly v1s beat perfect local branches every time. |

---

## 🤝 Get Involved

We're a small, focused team building in the open. If you've ever written a custom benchmark script because nothing composable existed, watched an agent forget everything between sessions, or spent more time on the README than the code — **you'll feel at home here.** 🏡

<table>
<tr><td valign="top" width="50%">

### 💛 Ways to contribute

- ⭐ **Star** a project you find useful
- 🐛 **Open an issue** — a bug, an idea, a frustration
- 🔨 Pick up a `good first issue` and send a **PR**
- 💬 Start or join a **Discussion** — we decide in public
- 📣 **Build something** with our tools and share it

</td><td valign="top" width="50%">

### 🔭 We're looking for

- 🦀 **Rust / C++ engineers** into inference optimization
- 🧠 **ML researchers** on memory systems & efficient architectures
- 🐍 **Python devs** building agent infrastructure
- ✨ **Anyone** who's felt the gaps we're filling

</td></tr>
</table>

<div align="center">

### 🌐 Stay Connected

[![Website](https://img.shields.io/badge/konjotech.com-4F46E5?style=for-the-badge&logo=googlechrome&logoColor=white)](https://konjotech.com)
[![X / Twitter](https://img.shields.io/badge/@wesley__scholl-0A0A0A?style=for-the-badge&logo=x&logoColor=white)](https://x.com/wesley_scholl)
[![Follow on GitHub](https://img.shields.io/github/followers/konjoai?style=for-the-badge&logo=github&label=Follow%20konjoai&labelColor=0A0A0A&color=4F46E5)](https://github.com/konjoai)

</div>

---

<div align="center">

## 📜 License

All Konjo AI projects are open source — most **MIT** licensed unless otherwise noted.
**Build on them, fork them, ship them.** 🚢

<br/>

***Make it Konjo — Plan, build, test, ship, rest, repeat.*** 🔁

🌟 *If any of this resonates,* [**give us a follow**](https://github.com/konjoai) *and watch the stack grow.* 🌟

</div>
