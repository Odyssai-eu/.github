<div align="center">

# OdyssAI

**European open-source local AI ecosystem.**
Infrastructure you control, frontier-grade experience.

[**odyssai.eu**](https://odyssai.eu) · Apache 2.0 · Built in Europe · Pre-release

</div>

---

## Local AI is not a downgrade.

Running models on your own hardware shouldn't cost you the quality, memory, speed and agentic capability expected from a frontier product. OdyssAI delivers that experience on sovereign infrastructure — local when it matters, cloud when you choose. No surrender required.

## The stack — three components, one experience

| Project | Role | Runs on |
|---|---|---|
| **OdyssAI-X** | Distributed **experience engine** (the *X* is for experience). Compute, routing and standard surfaces as one operational layer. *Runs the experience.* | Apple Silicon cluster · 1–5 nodes · TB5 RDMA |
| **Telemak** | Single-Mac runtime. One native app, a menu-bar, an HTTP daemon. No Docker, no Python, no cluster. *Holds the helm.* | One Apple Silicon Mac |
| **Companion** | Client and cognitive layer. Three-level knowledge base, semantic routing, local agents, Decision Log. *Gives the experience.* | Any host · Web · MCP · IDE |

Everything speaks standard **OpenAI** and **Anthropic** APIs. No proprietary SDK — any existing client works unchanged.

## Why it matters

- **Not capped at 35B.** OdyssAI-X distributes inference across Apple Silicon over Thunderbolt 5 RDMA — up to ~600B fp16 / ~1T Q8 on five nodes.
- **Within one point of the frontier.** Qwen 3.5 397B on a four-node cluster reached **94.4%** of Claude Opus on the TMB benchmark.
- **Built to run unattended.** A single Telemak node served **23,549 inferences over 96 h non-stop — zero failures**, two models in parallel.
- **On Apple's own stack.** Built directly on MLX and `mlx-distributed`. Not an exo fork, not a llama.cpp wrapper.

## Status

Pre-release, already running internally. Source opening progressively under **Apache 2.0**.

**→ [See the pitch](https://odyssai.eu/pitch/full/) · [Read the docs](https://odyssai.eu/docs) · [odyssai.eu](https://odyssai.eu)**

<div align="center">
<sub>OdyssAI by The Monocle Bear OÜ · Local AI infrastructure and experience, built in Europe.</sub>
</div>
