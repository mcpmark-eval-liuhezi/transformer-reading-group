# Transformer — "Attention Is All You Need" (arXiv:1706.03762)

**arXiv ID:** 1706.03762
**Title:** Attention Is All You Need
**Authors:** Vaswani, Shazeer, Parmar, Uszkoreit, Jones, Gomez, Kaiser, Polosukhin

## Architecture one-liner

The Transformer is a new simple network architecture **based solely on attention mechanisms**, **dispensing with recurrence and convolutions entirely**.

## Headline WMT 2014 results

| Task | BLEU (as reported in the paper) |
|------|-------------------------------|
| English-to-German (en-de) | 28.4 |
| English-to-French (en-fr) | 41.8 |

### English-to-German (en-de) — 28.4 BLEU
Improves over the existing best results, **including ensembles, by over 2 BLEU** (the paper's text: "by more than 2.0 BLEU"), establishing a new state-of-the-art BLEU score of 28.4. Training took 3.5 days on 8 P100 GPUs.

### English-to-French (en-fr) — 41.8 BLEU
A new single-model state-of-the-art BLEU score of 41.8, achieved **after training for 3.5 days on eight GPUs** — a small fraction of the training costs of the best models from the literature. (The abstract and Table 1 report 41.8; the Results narrative text mentions 41.0, but 41.8 is the headline figure in both the abstract and Table 1.)

---
*All figures quoted verbatim from arXiv:1706.03762 ("Attention Is All You Need"), abstract and Table 1.*
