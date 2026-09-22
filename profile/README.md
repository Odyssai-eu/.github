<div align="center">

# OdyssAI

**European sovereign local AI ecosystem.**
Infrastructure you control, frontier-grade experience.

[**odyssai.eu**](https://odyssai.eu) · Built in Europe · Pre-release

</div>

---

## Local AI is not a downgrade.

Running models on your own hardware shouldn't cost you the quality, memory, speed and agentic capability expected from a frontier product. OdyssAI is two pieces that together give you exactly that — on Apple Silicon you own, with the cloud only where *you* decide.

## The stack — an engine and a client, one experience

OdyssAI is two pieces: **OdyssAI-X**, the engine that runs the models, and **CoeOS**, the client you use every day. CoeOS itself ships as two repositories: **Nemo**, the app on your Mac, and the **CoeOS box**, the smart router behind it.

| Project | Role | Runs on |
|---|---|---|
| [**OdyssAI-X**](https://github.com/Odyssai-eu/OdyssAI-X) | The **engine**. Distributed MLX inference across Apple Silicon (pipeline / tensor parallel over Thunderbolt 5 RDMA or TCP), **replica mode** for many users at once, vision models, one control plane for many models. OpenAI and Anthropic APIs. AGPL-3.0. | One Mac to a rack of Mac Studios |
| [**Nemo**](https://github.com/Odyssai-eu/coeos) | The **CoeOS client**: a desktop AI operating system for one person. Chat with visible reasoning and personal memory, cowork on documents with the model, code with a panel of agents. Every turn shows which model served it and why. Signed, notarized macOS app: [releases](https://github.com/Odyssai-eu/coeos/releases). MIT. | Your Mac (Apple Silicon) |
| [**CoeOS box**](https://github.com/Odyssai-eu/coeos-box) | The **smart router**. Every request goes to the model proven best at that skill (from benchmarks, not marketing): local on OdyssAI-X, or cloud with your own keys. Users, tokens, quotas, the *Theseus* console. MIT. | A container on your LAN or your VPS |

Everything speaks standard **OpenAI** and **Anthropic** APIs. No proprietary SDK — Claude Code, IDE agents and any existing client work unchanged.

Also in this organisation: [**Guardian**](https://github.com/Odyssai-eu/odyssai-guardian) (confidential-content detection before anything leaves for a cloud provider), [**odyssai-services**](https://github.com/Odyssai-eu/odyssai-services) (bench and sidecar tooling), [**mlx-swift-lm**](https://github.com/Odyssai-eu/mlx-swift-lm).

## Why it matters

- **Not capped at 35B.** OdyssAI-X distributes inference across Apple Silicon over Thunderbolt 5 RDMA — up to ~600B fp16 / ~1T Q8 on five nodes.
- **Within one point of the frontier.** Qwen 3.5 397B on a four-node cluster reached **94.4%** of Claude Opus on the TMB benchmark.
- **Serves a crowd, not a demo.** Replica mode: one full copy per Mac, continuous batching, session affinity — throughput scales with the machines you add.
- **Sovereign by construction.** CoeOS ships with tested guarantees: no telemetry, no kill-switch, no mandatory call home. If you stop paying, it keeps running.
- **On Apple's own stack.** Built directly on MLX and `mlx-distributed`. Not an exo fork, not a llama.cpp wrapper.

## Status

Pre-release, running in production internally. **Available on-premise — get in touch.**

**→ [See the pitch](https://odyssai.eu/pitch/full/) · [Read the docs](https://odyssai.eu/docs) · [odyssai.eu](https://odyssai.eu)**

<div align="center">
<sub>OdyssAI by The Monocle Bear OÜ · Local AI infrastructure and experience, built in Europe.</sub>
</div>

OdyssAI-X is AGPL-3.0; Nemo, the CoeOS box, Guardian, CodeOS and mlx-swift-lm are MIT. Commercial licensing for the engine is available — see the website.
