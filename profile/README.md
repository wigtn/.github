<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wigtn/.github/main/profile/assets/wigtn-logo-white.png">
  <img src="https://raw.githubusercontent.com/wigtn/.github/main/profile/assets/wigtn-logo-navy.png" alt="WIGTN" width="320">
</picture>

**An independent AI team that builds for clients and publishes in the open.**

[WIGTN](https://wigtn.com) · [WIGTN Tech](https://tech.wigtn.com) · [Hugging Face](https://huggingface.co/Wigtn) · [LinkedIn](https://www.linkedin.com/company/wigtn) · [contact@wigtn.com](mailto:contact@wigtn.com)

</div>

---

### We learn, build, and share AI in the open.

WIGTN builds web products and AI systems for clients, and publishes what it learns in the open: peer-reviewed papers, released models, and reports that say what they do not show.

## Built on Qwen: from a 2B document parser to an EMNLP 2026 paper

One line of work in three repositories, read in order. Its training pipeline uses only openly released Qwen models. WIGTN is an independent team, not part of the Qwen project.

### 1. Distill Qwen3-VL into a document parser · [wigtnOCR-v1](https://github.com/wigtn/wigtnOCR-v1)

Qwen3-VL-30B-A3B-Thinking wrote Markdown for 4,501 pages of Korean government documents and arXiv papers. Qwen3.5-122B-A10B scored that Markdown on five criteria, and Qwen3-VL-2B-Instruct was fine-tuned with LoRA (ms-swift, r=8) on the 2,667 pages kept. The result, [WigtnOCR-2B](https://huggingface.co/Wigtn/Qwen3-VL-2B-WigtnOCR), matches or beats its 30B teacher on 3 of 5 OmniDocBench metrics, with Table TEDS 0.649 against 0.523. The repository holds the training config, the pipeline scripts and a step-by-step LoRA guide.

### 2. A result that did not fit

Against five other parsers, the one with the best chunk-boundary score (MinerU, BC 0.735) came fifth of six in retrieval. A score measured on a parser's output alone did not say which parser a retriever would work best with.

### 3. Test it as a paper: RCPS, EMNLP 2026 Industry Track · [WigtnOCR-RADP](https://github.com/wigtn/WigtnOCR-RADP)

The paper takes WigtnOCR-2B as its production parser and ranks parsers by retrieval on a frozen probe of 663 question–answer pairs.

- Table-enabled MinerU scores higher Boundary Clarity than WigtnOCR-2B (0.713 against 0.610), but its Hit@1 is 42.6 points lower (0.123 against 0.549).
- Choosing the parser moved Hit@1 by 42.6 points. Fine-tuning had moved it by 4.9.
- Retrieval-aware DPO training on top of WigtnOCR-2B added about one point of Hit@5, as did a matched edit-distance control. The nine adapters are in [RCPS-RADP-Adapters](https://github.com/wigtn/RCPS-RADP-Adapters).

Presentation: 25 October 2026, Virtual Session 1. [Paper (PDF)](https://github.com/wigtn/WigtnOCR-RADP/blob/main/output/pdf/EMNLP2026_Industry_384_camera_ready_final.pdf)

## Our Service

Three teams: Solutions builds AI into enterprise systems, Product ships our own, and Research publishes what we find, including what went nowhere, on [WIGTN Tech](https://tech.wigtn.com).

### Solutions: we build it

AX for enterprises, from consulting to the systems that run it.

- SK hynix: Global One ERP (i‑ERP) Platform development, with Braincrew. 2026.10
- Braincrew: AX project partnership. 2026.10
- Mind AI: closed beta test partner for MEGA Code. 2026.06

### Product: we ship it

Open-source tools we build and use ourselves.

- [WIGSS](https://github.com/wigtn/wigss): drag a component on your dev server and the source file rewrites itself. `npx wigss`
- [WIGTN Plugin for Claude Code](https://github.com/wigtn/wigtn-plugins): product workflows for Claude Code, with a gate on what leaves the machine.
- [WIGTN Plugin for Codex](https://github.com/wigtn/wigtn-plugins-codex): requirements, verification and release decisions, reusable in Codex.

### Research: we publish it

Peer-reviewed research on LLMs, their evaluation, and speech.

- ACL 2026 System Demonstrations: WIGVO, real-time speech translation over phone calls. [Paper](https://aclanthology.org/2026.acl-demo.33/) · [Code](https://github.com/wigtn/wigvo)
- EMNLP 2026 Industry Track: RCPS, choosing document parsers by retrieval. [Paper and code](https://github.com/wigtn/WigtnOCR-RADP)
- NeurIPS 2026 TAE Workshop: MDI, the minimum detectable improvement of an LLM judge. [Code and data](https://github.com/wigtn/mdi-artifact)

## Work with us

Have a problem AI hasn't solved for you yet? Tell us where it fails today. We measure it before we build anything, bring the fix into the systems you already run, and say where the fix stops. A report you think is wrong, or an issue on one of our tools, is just as welcome.

[contact@wigtn.com](mailto:contact@wigtn.com) · [About WIGTN](https://wigtn.com/team)

<div align="center">
<sub>Everything we learn, we share.</sub>
</div>
