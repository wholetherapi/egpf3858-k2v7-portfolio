---
title: "Neural Signatures for Program Semantics (Extended)"
kind: paper
year: 2025
status: "Accepted"
venue: "TMLR"
authors:
  - Christina Adams
  - Priya Raman
  - Hana Okafor
summary: "Learned signatures that summarise program semantics across compiler transformations, extended with cross-language transfer experiments."
topics:
  - program semantics
  - representation learning
---

# Neural Signatures for Program Semantics (Extended)

Christina Adams, Priya Raman, Hana Okafor

## Abstract

This extended version of the neural-signatures work adds cross-language
transfer experiments and a larger benchmark of compiler transformation pairs.
We show that a compact learned signature is sufficient to retrieve
semantically equivalent functions across optimisation levels and source
languages.

## Contributions

- A training objective that is invariant to declaration order within a module.
- A retrieval benchmark covering three languages and four optimisation levels.
- Ablations over signature width, training data size and tokenisation.

## Appendix

The appendix in the journal version contains the full hyper-parameter sweep
and the per-language error analysis. Those tables are not reproduced here.
