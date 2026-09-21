# Transformer Reading Notes

Paper: **"Attention Is All You Need"** — Vaswani et al., arXiv 1706.03762
All figures and section names below were verified against the live paper on arXiv.

Note: the draft numbers on the prep sheet (26.4 BLEU En-De, 39.2 BLEU En-Fr) trace back to an old preprint and do not match the published paper's test-set results; the verified figures are below.

## Q1 — WMT 2014 English-to-German BLEU (big model)

The big Transformer model reports **28.4 BLEU** on the WMT 2014 English-to-German translation task, outperforming the best previously reported models, **ensembles included, by more than 2.0 BLEU**. (The strongest prior result was the ConvS2S ensemble at 26.36 BLEU; the Transformer base model already reaches 27.3.)

## Q2 — WMT 2014 English-to-French BLEU, training time and hardware

The big model establishes a new **single-model state-of-the-art BLEU score of 41.8** on WMT 2014 English-to-French, after training for **3.5 days on 8 P100 GPUs** — a small fraction of the training cost of the best models in the literature. (The abstract and Table 2 both state 41.8; the body text of the Results section quotes 41.0, so 41.8 is the headline figure. The En-Fr big model used dropout 0.1 rather than 0.3.)

## Q3 — Top-level section headings, in order

1. Introduction
2. Background
3. Model Architecture
4. Why Self-Attention
5. Training
6. Results
7. Conclusion
8. Attention Visualizations (appendix)

## Q4 — What the architecture dispenses with, and what it uses instead

The Transformer dispenses with **recurrence and convolutions entirely** and is based **solely on attention mechanisms**.
