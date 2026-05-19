# ቆንጆ Konjo AI

**KONJO — Know, Outline, Nail, Justify, Optimize.**

![konjo banner](https://github.com/user-attachments/assets/fd55d13d-f747-447f-a979-34b3734c9d76)

> **Konjo** · **ቆንጆ** — Beautiful. · **根性** — Fighting spirit. · **康宙** — Health of the universe. · **खोजो** — Search and discover.
>
> *Make it Konjo — Plan, build, test, ship, rest, repeat.*

Konjo is the word you reach for when a tool does exactly what it needs to do — nothing more, nothing less.

We build the open infrastructure layer for AI. Not wrappers, not prompt chains — the deep systems that power them: compression, inference, vector engines, memory architectures, compliance, and the research that pushes the whole stack forward. Vertically integrated, benchmark-driven, built in public.

---

## The Stack

```
┌──────────────────────────────────────────────────────────────┐
│                        Orchestration                          │
│              lopi (Agent Orchestrator) · kyro (RAG)          │
├──────────────────────────────────────────────────────────────┤
│                       Inference Layer                         │
│            squish (Local LLMs) · kairu (Speculative)         │
├──────────────────────────────────────────────────────────────┤
│                       Retrieval Layer                         │
│             vectro (Vectors) · kohaku (Memory)               │
├──────────────────────────────────────────────────────────────┤
│                  Research & Compliance                        │
│    drex (Architecture) · toki (Robustness) · miru (XAI)     │
│                    squash (EU AI Act)                         │
└──────────────────────────────────────────────────────────────┘
```

---

## Projects

### Inference & Compression

#### [squish](https://github.com/konjoai/squish) · Python

**Compress local LLMs once. Run them forever.**

OpenAI + Ollama drop-in for Apple Silicon with statistically identical accuracy and 54× faster cold starts. INT8/INT4/AQLM quantization, MLX-native, sub-second load times.

`quantization` `apple-silicon` `mlx` `local-llm` `openai-api` `ollama`

#### [kairu](https://github.com/konjoai/kairu) · Python

**Speculative decoding engine for HuggingFace models.**

EAGLE-style drafting, dynamic early exit, and token budget control with a live performance dashboard. Designed to squeeze every token out of your inference budget.

`speculative-decoding` `huggingface` `inference` `latency` `throughput`

---

### Retrieval & Memory

#### [vectro](https://github.com/konjoai/vectro) · Rust · Mojo · Python

**Lightning-fast embedding quantization and ANN indexing.**

12M+ vec/s throughput — 4.85× faster than FAISS C++ — with drastically reduced memory footprint. Sub-1ms encode, HNSW (recall@10=0.920), NF4/INT8/PQ quantization, AutoQuantize, pipeline CLI, WASM bindings.

`rust` `mojo` `quantization` `vector-search` `embeddings` `rag` `hnsw`

#### [kohaku](https://github.com/konjoai/kohaku) · Python

**Neural episodic memory engine using HDC hypervectors.**

Stores long-term context and retrieves via associative recall. A persistent memory layer that goes beyond RAG — designed for LLMs that need to remember across sessions and tasks.

`episodic-memory` `hdc` `hyperdimensional-computing` `rag-alternative` `llm`

---

### Orchestration & Pipelines

#### [lopi](https://github.com/konjoai/lopi) · Rust

**High-performance orchestrator for Claude Code agents.**

Concurrent agents in git-isolated branches with retry loops, priority queuing, SQLite memory, pattern mining, scheduled tasks, and a live TUI + web dashboard. Remote control via Telegram.

`rust` `claude-code` `agent-orchestrator` `async-rust` `tokio` `tui` `telegram-bot`

#### [kyro](https://github.com/konjoai/kyro) · Python

**Production RAG pipeline.**

Hybrid retrieval (dense + BM25 + RRF), reranking, and RAGAS evals baked in. Local-first with Squish + Vectro. Plugs into OpenAI, Anthropic, or runs fully offline.

`rag` `hybrid-search` `bm25` `reranking` `ragas` `qdrant` `local-llm`

---

### Compliance

#### [squash](https://github.com/konjoai/squash) · Python

**Automated EU AI Act compliance for AI/ML teams.**

Annex IV documentation, SBOMs (CycloneDX/SPDX), policy checks, and Sigstore-signed audit records inside your CI/CD pipeline. August 2, 2026 enforcement deadline — squash gets you there.

`eu-ai-act` `compliance-automation` `sbom` `cyclonedx` `sigstore` `cicd` `nist-ai-rmf`

#### [squash-action](https://github.com/konjoai/squash-action)

**AI Compliance Gate for GitHub Actions.**

EU AI Act · NIST AI RMF · ISO 42001. One step in CI/CD. Pairs with squash.

#### [homebrew-squash](https://github.com/konjoai/homebrew-squash) · Ruby

**Homebrew tap for squash.**

`brew install konjoai/squash/squash-ai` — the fastest path to EU AI Act compliance on macOS.

`homebrew` `macos` `squash` `tap`

---

### Research

#### [drex](https://github.com/konjoai/drex) · Python

**Next-generation neural architecture research.**

The transformer is a brilliant hack scaled past its limits. DREX is what comes next — tiered memory, sparse execution, and a learned controller that knows what to remember. Mamba SSM + ESN reservoir + HDC encoding + NoProp memory + RL controller + KAN readout.

`transformer-alternative` `mamba` `tiered-memory` `sparse-attention` `cognitive-architecture`

#### [toki](https://github.com/konjoai/toki) · Python

**Adversarial fine-tuning lab for small models (1B–3B).**

Generate red-team attacks, harden via LoRA, ship datasets and robust weights. Investigates whether robustness truly generalizes or just overfits under pressure.

`red-teaming` `adversarial-ai` `lora` `fine-tuning` `alignment` `model-robustness`

#### [miru](https://github.com/konjoai/miru) · Python

**Multimodal reasoning tracer.**

Answers questions over images and documents while visualizing step-by-step attention and reasoning chains. Built for explainable vision-language AI — see what the model sees and why.

`vlm` `multimodal` `xai` `attention` `vision-language-models` `explainability`

---

### Design

#### [ui](https://github.com/konjoai/ui) · TypeScript

**Konjo AI design system + portfolio homepage monorepo.**

Packages: `ui` · Apps: `web`

---

## Engineering Principles

We build primarily in **Rust** and **Python**, integrating **Mojo** and **C++** where the metal demands it.

1. **CLI-first, pipe-friendly** — Every tool must play seamlessly with Unix workflows and CI/CD pipelines.
2. **Show the math** — Real benchmark numbers over vibes. Latency (p50/p95/p99) and accuracy are measured constantly.
3. **Open specs, zero lock-in** — Built on open formats. Swap any Konjo layer for something else; the system allows it.
4. **Ship fast, iterate in public** — Ugly v1s beat perfect local branches every time.

---

## Get Involved

We're a small, focused team building in the open. If you've written a custom benchmark script because nothing composable existed, had an agent forget everything between sessions, or spent more time on the README than the code — you'll feel at home here.

**Ways to contribute:**

- ⭐ Star a project you find useful
- 🐛 Open an issue with a bug, idea, or frustration
- 🔨 Pick up a `good first issue` and send a PR
- 💬 Start or join a Discussion — we make decisions in public
- 📣 Build something with our tools and share it

**We're actively looking for:**

- Rust and C++ engineers interested in inference optimization
- ML researchers working on memory systems or efficient architectures
- Python developers building agent infrastructure
- Anyone who's felt the gaps we're filling

---

## Stay Connected

- 🌐 [konjotech.com](https://konjotech.com)
- 𝕏 [@wesley_scholl](https://x.com/wesley_scholl)

---

## License

All Konjo AI projects are open source — most are MIT licensed unless otherwise noted. Build on them, fork them, ship them.

*Make it Konjo — Plan, build, test, ship, rest, repeat.*
