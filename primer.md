# Sequence Models Reading Group — Session 1 Primer

**Paper:** *Attention Is All You Need* (Vaswani et al., arXiv:1706.03762)

Welcome to the first session of our reading group! This short primer distills the paper's headline results, its structure, and the logistics for our kickoff call, so everyone can come prepared.

## What the paper claims

The dominant sequence transduction models of the time were built on complex recurrent or convolutional networks with an encoder and a decoder, the best of which also connected the two with attention. The Transformer instead uses **attention mechanisms alone** — dispensing with recurrence and convolutions entirely — which makes it both simpler and far more parallelizable to train.

## Headline numbers — WMT 2014 machine translation

| Task | Result | Notes |
|------|--------|-------|
| English → German | **28.4 BLEU** | Improves over the existing best results, **including ensembles, by more than 2 BLEU** |
| English → French | **41.8 BLEU** | New **single-model** state-of-the-art |

## Training cost

The big model trained for **3.5 days on eight GPUs** (P100s) for the English → French result — a **small fraction** of the training cost of the best models from the literature, while still being more parallelizable in design.

Beyond translation, the paper shows the Transformer **generalizes well to other tasks**, applying it successfully to English constituency parsing with both large and limited training data.

## How the paper is organized

One line: the paper moves from motivation to mechanism to evidence — *Introduction* and *Background* set up the problem, *Model Architecture* and *Why Self-Attention* explain the design, and *Training*, *Results*, and *Conclusion* deliver the empirical payoff (with an *Attention Visualizations* appendix for intuition).

Suggested reading order for the session: skim §1–2, spend most of our time on §3 (Model Architecture) and §4 (Why Self-Attention), then walk through §5–6 (Training, Results).

## Logistics — kickoff call

The kickoff call is at **19:00 Beijing time**, which works out to:

| City | Local time |
|------|------------|
| Beijing | 19:00 (Friday) |
| New York | 07:00 (Friday) |
| London | 12:00 (Friday) |

*(Times reflect current daylight-saving offsets: Beijing is UTC+8, New York is 12 hours behind, and London is 7 hours behind Beijing.)*

---

*All figures quoted from the abstract of arXiv:1706.03762.*
