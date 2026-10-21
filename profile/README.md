<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wigtn/.github/main/profile/assets/wigtn-logo-white.png">
  <img src="https://raw.githubusercontent.com/wigtn/.github/main/profile/assets/wigtn-logo-navy.png" alt="WIGTN" width="320">
</picture>

**An independent AI team that builds for clients and publishes in the open.**

[wigtn.com](https://wigtn.com) · [WIGTN Tech](https://tech.wigtn.com) · [Hugging Face](https://huggingface.co/Wigtn) · [contact@wigtn.com](mailto:contact@wigtn.com)

</div>

---

### We learn, build, and share AI in the open.

WIGTN builds web products and AI systems for clients, and publishes what it learns in the open: peer-reviewed papers, released models, and reports that say what they do not show.

## Modeling

| Project | What it does | Built with |
|---|---|---|
| [WigtnOCR](https://github.com/wigtn/wigtnOCR-v1) | Document parser distilled from a 30B into a 2B vision-language model. The teacher writes Markdown for 4,501 pages, the judge keeps the pages that score 3 or higher, and the student is LoRA fine-tuned on 2,667 of them. [WigtnOCR-2B](https://huggingface.co/Wigtn/Qwen3-VL-2B-WigtnOCR) matches or beats its teacher on 3 of 5 OmniDocBench metrics, with Table TEDS 0.649 against 0.523 | Qwen3-VL-30B-A3B-Thinking (teacher), Qwen3.5-122B-A10B (judge), Qwen3-VL-2B-Instruct (student), ms-swift |
| [RCPS-RADP-Adapters](https://github.com/wigtn/RCPS-RADP-Adapters) | Nine LoRA adapters for retrieval-aware parser training: auxiliary loss, DPO, distillation and a SimPO control | PEFT LoRA on Qwen3-VL-2B-Instruct and WigtnOCR-2B |

## Real-Time Speech-to-Speech Translation

| Project | What it does | Built with |
|---|---|---|
| [WIGVO](https://github.com/wigtn/wigvo) | Real-time Korean–English speech translation over ordinary phone calls (ACL 2026 System Demonstrations). 555 ms median caller-to-callee latency at USD 0.28/min, 430+ tests | OpenAI Realtime API, Twilio Media Streams, FastAPI, Next.js, Cloud Run |

## Evaluation Research

| Project | What it does | Venue |
|---|---|---|
| [RCPS](https://github.com/wigtn/WigtnOCR-RADP) | Chooses document parsers by retrieval on a fixed question–answer probe, and separates parser-side from chunker-side loss | EMNLP 2026 Industry Track |
| [MDI](https://github.com/wigtn/mdi-artifact) | The minimum detectable improvement of an LLM judge. All 97,752 judge calls are logged, and every number in the paper resolves to a file | NeurIPS 2026 TAE Workshop |

## Developer Tools & Agent Harness

| Project | What it does | Built with |
|---|---|---|
| [WIGTN Plugins](https://github.com/wigtn/wigtn-plugins) | Claude Code plugin with 11 agents, from requirements to a verified commit | Claude Code |
| [WIGTN Plugins for Codex](https://github.com/wigtn/wigtn-plugins-codex) | The same requirements, verification and release workflow for Codex | Codex |
| [WIGSS](https://github.com/wigtn/wigss) | Drag a component on your running dev server and an AI agent rewrites the source. `npx wigss` | Next.js, WebSocket, OpenAI API |

Other public projects are in [our repositories](https://github.com/wigtn?tab=repositories&type=source).

<div align="center">
<sub>Everything we learn, we share.</sub>
</div>
