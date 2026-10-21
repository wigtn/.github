<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wigtn/.github/main/profile/assets/wigtn-logo-white.png">
  <img src="https://raw.githubusercontent.com/wigtn/.github/main/profile/assets/wigtn-logo-navy.png" alt="WIGTN" width="320">
</picture>

**An independent AI team that builds for clients and publishes in the open.**

[wigtn.com](https://wigtn.com) · [WIGTN Tech](https://tech.wigtn.com) · [Hugging Face](https://huggingface.co/Wigtn) · [contact@wigtn.com](mailto:contact@wigtn.com)

</div>

---

This is where our code lives. For who we are and what we offer, see [wigtn.com](https://wigtn.com).

## WigtnOCR → RCPS: from a fine-tuned parser to an EMNLP 2026 paper

One project in three repositories, in the order it happened:

1. **Fine-tune.** [wigtnOCR-v1](https://github.com/wigtn/wigtnOCR-v1) distills a 30B vision-language model into a 2B document parser. Qwen3-VL-30B writes Markdown for 4,501 pages, Qwen3.5-122B filters it, and Qwen3-VL-2B is fine-tuned on the rest with LoRA. The result, [WigtnOCR-2B](https://huggingface.co/Wigtn/Qwen3-VL-2B-WigtnOCR), matches or beats its teacher on 3 of 5 OmniDocBench metrics.
2. **Find.** Evaluating it against five other parsers, the one with the best chunk-boundary score ranked fifth of six in retrieval.
3. **Research.** [WigtnOCR-RADP](https://github.com/wigtn/WigtnOCR-RADP) studies that mismatch with WigtnOCR-2B as the production parser: RCPS, accepted to the EMNLP 2026 Industry Track. [RCPS-RADP-Adapters](https://github.com/wigtn/RCPS-RADP-Adapters) holds the nine LoRA adapters from its parser-training study.

## Real-time AI systems

| Project | What it does | Built with |
|---|---|---|
| [WIGVO](https://github.com/wigtn/wigvo) | Real-time Korean–English speech translation over ordinary phone calls (ACL 2026 System Demonstrations). 555 ms median caller-to-callee latency at USD 0.28/min, 430+ tests | OpenAI Realtime API, Twilio Media Streams, FastAPI, Next.js, Cloud Run |
| [TimeLens](https://github.com/wigtn/wigtn-timelens) | Museum curator that recognises artifacts through the camera and talks about them in real time | Gemini Live API, Next.js, Cloud Run |

## Evaluation research

| Project | What it does | Venue |
|---|---|---|
| [RCPS](https://github.com/wigtn/WigtnOCR-RADP) | Chooses document parsers by retrieval on a fixed question–answer probe, and separates parser-side from chunker-side loss | EMNLP 2026 Industry Track |
| [MDI](https://github.com/wigtn/mdi-artifact) | The minimum detectable improvement of an LLM judge. All 97,752 judge calls are logged, and every number in the paper resolves to a file | NeurIPS 2026 TAE Workshop |

## Developer tools and agents

| Project | What it does | Built with |
|---|---|---|
| [WIGTN Plugins](https://github.com/wigtn/wigtn-plugins) | Claude Code plugin with 11 agents, from requirements to a verified commit | Claude Code |
| [WIGTN Plugins for Codex](https://github.com/wigtn/wigtn-plugins-codex) | The same requirements, verification and release workflow for Codex | Codex |
| [WIGSS](https://github.com/wigtn/wigss) | Drag a component on your running dev server and an AI agent rewrites the source. `npx wigss` | Next.js, WebSocket, OpenAI API |
| [wigtoken](https://github.com/wigtn/wigtoken) | Self-hosted Claude Code usage aggregator with a live SSE counter and Prometheus metrics | Node.js, SQLite |
| [SPEAR](https://github.com/wigtn/wigtn-spear) | Attack verification for products and AI agents you are authorized to test: signed authorization, causal HTTP attack checks, replayable evidence | TypeScript |
| [wigtn-hermes](https://github.com/wigtn/wigtn-hermes-agent) | Installs Hermes Agent on a bare Mac mini and keeps it running: restarts, cleanup, automatic PR review | Python, shell |

## Hackathons

| Project | What it does | Built with |
|---|---|---|
| [OpenSlot](https://github.com/wigtn/aws-hackathon-dsql) | On-sale infrastructure for high-demand drops, with no oversell across regions (H0: Hack the Zero Stack) | Aurora DSQL, Aurora PostgreSQL with PostGIS and pgvector, Next.js, Vercel |

- Build with TRAE Seoul (ByteDance): Grand Prize
- Snowflake AI & Data Hackathon Korea 2026: 2nd place, Tech Track
- OBA Weekendthon: Top 6

Other public projects are in [our repositories](https://github.com/wigtn?tab=repositories&type=source).

<div align="center">
<sub>Everything we learn, we share.</sub>
</div>
