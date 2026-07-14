<samp>**English** · [한국어](README.ko.md)</samp>

# 🏆 1st Place at [Ralphthon @ICML "Auto Research"](https://luma.com/hjuo7auc) — won $10,000 OpenAI credits

## Depth-AR — a research paper written end-to-end by an AI scientist

[![Harness: writing-driven-autoresearch](https://img.shields.io/badge/harness-writing--driven--autoresearch-181717?logo=github)](https://github.com/happyhappy-jun/writing-driven-autoresearch)
[![Blog: how we built it](https://img.shields.io/badge/blog-how_we_built_it-4a76c9)](https://byungjunyoon.ai/writing-driven-autoresearch/)

**Co-authored by [Byungjun Yoon](https://github.com/happyhappy-jun), [Woomin Song](https://github.com/woominsong) & our AI Scientist** 🙏

> 🔬 **Fully AI-written, with only light high-level human guidance, then judged by human experts.** The AI scientist wrote the paper end to end; humans stepped in only for occasional high-level direction, never to revise the text. It was then evaluated in ICML format by a panel of **11 expert judges**: professors and researchers across ML, AI safety, robotics, and biotech.

<div align="center">

### ✍️ We believe there's far more to learn from *how* an agent writes than from the paper itself.

**So we're fully open-sourcing the `git log`** — every step of how our AI scientist reasoned, revised, and drove Overleaf to write the LaTeX.

</div>

## Full `git log` of Our AI-Scientist

```bash
# track whole AI Scientist's writing history
git clone https://github.com/happyhappy-jun/depth-ar.git
git log
```

<div align="center">
  <img src="assets/commit-history.svg" alt="Commit-history timeline: 45 commits in one ~4-hour session, 39 by the AI, with self-corrections highlighted — a pre-registered test, an honest non-replication, a figure fix flagged not faked, and a retraction." width="880">
</div>

## Left alone, it wrote itself a rulebook

The AI kept setting itself hard rules and quoting them back — banning its own weasel-words, refusing to ship a figure it hadn't looked at, and publishing a result that argued *against* its own paper. Then it got bitten by the exact bug one of those rules was written to prevent. All verbatim from the commit messages:

<div align="center">
  <img src="assets/agent-rules.svg" alt="Rules the AI wrote for itself, verbatim from its commits: a number I cannot account for is a number I do not print; a figure I have not looked at does not go in the paper; a warn is a non-check; 'matches or beats' is a banned construction; and it goes in anyway." width="880">
</div>

## The paper, in one line

**Depth-AR** — instead of zeroing a skipped Transformer layer's update, *predict* it from the layers before it. 📄 [`paper.pdf`](paper.pdf)

## How it was built

This repo is the *paper* — the harness that wrote it lives in **[happyhappy-jun/writing-driven-autoresearch](https://github.com/happyhappy-jun/writing-driven-autoresearch)**: the three agent personas, the decision ledger (136 timestamped decisions), and the integrity tooling that kept the paper honest. The full story of how and why we built it: **[the blog post](https://byungjunyoon.ai/writing-driven-autoresearch/)**.

---

## The event

Built at **[Ralphthon @ICML — "Auto Research"](https://luma.com/hjuo7auc)**: once the "Ralph Loop" starts, you're not allowed to touch your agent. (To touch your laptop at all, you wear a lobster costume — which is why every commit is authored by `lobster`. 🦞)

**How it was judged.** In the AI Scientist track, each team builds an agent that writes a research paper (this repo). The paper was peer-reviewed in ICML format by a panel of **11 expert human judges** — university professors and researchers, startup founders and engineers - who scored both the paper and the agent workflow behind it. We took 1st place.
