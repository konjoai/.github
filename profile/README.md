# ቆንጆ Konjo AI

**KONJO — Know, Outline, Nail, Justify, Optimize.**

**The Konjo Way: Know the problem, outline the solution, nail the build, justify the claims, optimize the output.**

![image (42)](https://github.com/user-attachments/assets/fd55d13d-f747-447f-a979-34b3734c9d76)

> **Konjo** - **ቆንጆ** — Beautiful. **根性** — Fighting spirit. **康宙** — Health of the universe. **खोजो** — Search and discover.
> *Make it Konjo — Plan, build, test, ship, rest, repeat.*

Konjo is the kind of word you use when a tool does exactly what it needs to do, nothing more, and nothing less.

We build the open infrastructure layer for AI. Not wrappers, not prompt chains, but the deep systems that power them: compression, inference optimization, vector engines, and compliance layers. We are building a vertically integrated LLM stack from scratch.

---

## 🏗️ The Architecture

We approach AI infrastructure as a layered operating system. Everything is modular, benchmark-driven, and designed to plug into the core orchestration runtime.

  * **Orchestration:** `konjo-runtime`
  * **Components:** `vectro` (Retrieval) + `squish` (Inference)
  * **Compliance:** `squash` (Policy & Audit)
  * **Research Foundation:** `drex` (Architecture)

-----

## 📦 Active Projects

### [KonjoOS](https://www.google.com/search?q=https://github.com/konjoai/KonjoOS)

**The AI Orchestration Runtime**
The central spine of the Konjo AI stack. It is not just a RAG application; it is a modular AI system runtime capable of hybrid retrieval, query routing, execution, and telemetry.

  * **Capabilities:** Dense + BM25 + RRF hybrid retrieval, HyDE, ColBERT late interaction, and real-time RAGAS evaluation.
  * **Stack:** Python, FastAPI, Docker, Qdrant.

### [vectro](https://www.google.com/search?q=https://github.com/konjoai/vectro)

**High-Performance Embedding Compression & ANN Index**
A blazingly fast vector system that absorbs the complexity of advanced quantization. It currently outperforms FAISS by 4.85× in local benchmarks.

  * **Capabilities:** Sub-1ms encode, HNSW (recall@10=0.920), NF4/INT8/PQ quantization, AutoQuantize, pipeline CLI.
  * **Stack:** Rust CLI, Mojo hot-path, Python API, WASM bindings.

### [drex](https://www.google.com/search?q=https://github.com/konjoai/drex)

**Hybrid Neural Architecture Research**
The research foundation of Konjo AI. DREX is an exploration into building highly efficient, next-generation language models without relying solely on standard Transformers.

  * **Architecture:** Mamba SSM + ESN reservoir + HDC encoding + NoProp memory + RL controller + KAN readout.
  * **Status:** Phase 1 complete (125M config ready), Sprint 5 active.

### [squish](https://github.com/squishai/squish) & squash

**Inference, Quantization, and Compliance Layer**
*(Maintained under our partner org, Squish AI)*
Squish handles local model serving, INT3/INT4/AQLM quantization, semantic caching, and speculative decoding. It is tightly coupled with **Squash**, our enterprise AI compliance layer.

  * **Squash Capabilities:** CycloneDX/SPDX generation, EU AI Act policy engine, VEX feed multi-tenant SaaS, and CI/CD integration (Argo, Jenkins, GitHub Actions).

-----

## 🔮 The Roadmap (Q3/Q4 2026)

These supporting components are currently being built inside `konjo-runtime` and will be extracted into standalone infrastructure primitives once their APIs are stabilized:

  * **`membank`**: A multi-tiered memory architecture (L1 context, L2 vector, L3 semantic/episodic) directly inspired by DREX research.
  * **`evalkit`**: A central evaluation framework for tracking inference latency, retrieval accuracy, and generation faithfulness.
  * **`nanotune`**: A localized fine-tuning loop designed to optimize small models specifically for the `konjo-runtime` orchestration layer.

-----

## 🛠️ Our Engineering Principles

We build primarily in **Rust** and **Python**, integrating **Mojo** and **C++** where the metal demands it.

1.  **CLI-first, pipe-friendly:** Tools must play seamlessly with existing Unix workflows and CI/CD pipelines.
2.  **Show the math:** Real benchmark numbers over vibes. Latency (p50/p95/p99) and accuracy are measured constantly.
3.  **Open specs, zero lock-in:** We build on open formats. If you want to swap out a Konjo layer for a different tool, the system allows it.
4.  **Ship fast, iterate in public:** Ugly v1s are better than perfect local branches.

---

## Get Involved

We're a small, focused team building in the open. If you've ever written a custom benchmark script because nothing composable existed, had an agent forget everything between sessions, or shipped a local AI app and spent more time on the README than the code — you'll feel at home here.

**Ways to contribute:**

- ⭐ Star a project you find useful
- 🐛 Open an issue with a bug, idea, or frustration
- 🔨 Pick up a [`good first issue`](#) and send a PR
- 💬 Start or join a [Discussion](#) — we make decisions in public
- 📣 Build something with our tools and share it

**We're actively looking for:**
- Rust and C++ engineers interested in inference optimization
- ML researchers working on memory systems or efficient inference
- Python developers building agent infrastructure
- Anyone who's felt the gaps we're filling

---

## Stay Connected

- 🌐 [konjotech.com](https://konjotech.com)
- 𝕏 [@wesley_scholl](https://x.com/wesley_scholl)
- 💬 Discord — coming soon
- 📬 Newsletter — coming soon

---

## License

All Konjo AI projects are open source. Most are MIT licensed unless otherwise noted. Build on them, fork them, ship them. Just make it konjo.

---

*Konjo AI — Make it Konjo. Plan, build, test, ship, rest, repeat.*
