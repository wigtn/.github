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

## Fine-tuning Qwen3-VL by distillation

We built our own document parser by distilling Qwen3-VL-30B into Qwen3-VL-2B.

```
Qwen3-VL-30B-A3B-Thinking  (teacher)  →  writes Markdown for 4,501 document pages
Qwen3.5-122B-A10B          (judge)    →  keeps the pages that score 3 or higher
Qwen3-VL-2B-Instruct       (student)  →  LoRA r=8 with ms-swift on 2,667 pages  →  WigtnOCR-2B
```

- WigtnOCR-2B matches or beats its 30B teacher on 3 of 5 OmniDocBench metrics, with Table TEDS 0.649 against 0.523. [Model](https://huggingface.co/Wigtn/Qwen3-VL-2B-WigtnOCR) · [Training and evaluation code](https://github.com/wigtn/wigtnOCR-v1)
- Evaluating it led to RCPS, an EMNLP 2026 Industry Track paper that uses WigtnOCR-2B as its production parser. [Paper and code](https://github.com/wigtn/WigtnOCR-RADP) · [Retrieval-aware LoRA adapters](https://github.com/wigtn/RCPS-RADP-Adapters)

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
