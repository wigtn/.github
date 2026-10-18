<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wigtn/.github/main/profile/assets/wigtn-logo-white.png">
  <img src="https://raw.githubusercontent.com/wigtn/.github/main/profile/assets/wigtn-logo-navy.png" alt="WIGTN" width="320">
</picture>

**An independent AI team in Korea that builds for clients and publishes in the open.**

[WIGTN](https://wigtn.com) · [WIGTN Tech](https://tech.wigtn.com) · [Hugging Face](https://huggingface.co/Wigtn) · [contact@wigtn.com](mailto:contact@wigtn.com)

</div>

---

WIGTN builds web products and AI systems for clients, and publishes what it learns: peer-reviewed papers, released models, and technical reports that say what they do not show.

## What we do

### Web Agency: we build it

Websites and web products, assembled from modules we own and keep under test: a UI kit, a back office, an AI pipeline, and notifications.

### AX Agency: we measure it

We map where AI has leverage in your workflows and where it does not. The metric is agreed before anything is built and measured on your own data. After launch we measure again against that baseline, and whatever did not move the number gets cut.

## Selected work

| Project | What it is | Evidence | Links |
| --- | --- | --- | --- |
| WIGVO | Real-time Korean–English translation over ordinary phone calls. The person on the other end needs no app. | ACL 2026 System Demonstrations. 555 ms median caller-to-callee latency over 814 turns. | [Paper](https://aclanthology.org/2026.acl-demo.33/) · [Report](https://tech.wigtn.com/wigvo/) · [Code](https://github.com/wigtn/wigvo) |
| WigtnOCR | A 2B LoRA adapter that parses Korean government documents into structured Markdown, distilled from a 30B teacher. | Hit@1 0.739 on KoGovDoc-Bench, first of six parsers on three of four retrieval metrics. | [Model](https://huggingface.co/Wigtn/Qwen3-VL-2B-WigtnOCR) · [Benchmark](https://huggingface.co/datasets/Wigtn/KoGovDoc-Bench) · [Report](https://tech.wigtn.com/wigtnocr/) · [Code](https://github.com/wigtn/wigtnOCR-v1) |
| WIGSS | A CLI that wraps your dev server. Drag a component on the live page and the change is written back into the source file behind it. | Published on npm under Apache-2.0. Run with `npx wigss`. | [npm](https://www.npmjs.com/package/wigss) · [Report](https://tech.wigtn.com/wigss/) · [Code](https://github.com/wigtn/wigss) |
| WIGTN plugins | A plugin set for multi-agent software workflows in Claude Code and Codex. | Redesigned after our own evaluation found the old harness added 151.7% median wall time with no better task outcomes. | [Claude Code](https://github.com/wigtn/wigtn-plugins) · [Codex](https://github.com/wigtn/wigtn-plugins-codex) · [Report](https://tech.wigtn.com/codex-selective-harness/) |

Other public projects are in [our repositories](https://github.com/wigtn?tab=repositories&type=source).

## Track record

### Papers

- ![ACL 2026](https://img.shields.io/badge/ACL%202026-5A2E97?style=flat-square) System Demonstrations: *WIGVO: Real-Time Bidirectional Speech Translation over Legacy PSTN Calls via Dual-Session Echo Gating*, pp. 336–344. Demonstrated live at the conference, followed by an invited talk and poster at IWSLT 2026.
- ![EMNLP 2026](https://img.shields.io/badge/EMNLP%202026-5A2E97?style=flat-square) Industry Track: *Retrieval-Conditional Parsing Score (RCPS): Choosing Document Parsers by Retrieval, Not by Appearance.* [Code](https://github.com/wigtn/WigtnOCR-RADP)
- ![NeurIPS 2026](https://img.shields.io/badge/NeurIPS%202026-5A2E97?style=flat-square) TAE workshop: *MDI: The Minimum Detectable Improvement of an LLM Judge.* [Code and data](https://github.com/wigtn/mdi-artifact)

### Competitions

- Build with TRAE Seoul (ByteDance): Grand Prize
- Snowflake AI & Data Hackathon Korea 2026: 2nd place, Tech Track
- OBA Weekendthon: Top 6

We list only published work. Papers under review are left out until they are accepted.

## Work with us

Bring us a site to build or a workflow that needs AI. You can also read one of our reports and tell us where it is wrong, try one of the models, or open an issue in any repository.

Email us at [contact@wigtn.com](mailto:contact@wigtn.com).

<div align="center">
<sub>Everything we learn, we share.</sub>
</div>
