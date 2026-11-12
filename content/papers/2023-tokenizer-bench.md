---
title: "Tokenizer Bench: A Reproducible Evaluation Harness"
kind: paper
year: 2023
status: "Published"
venue: "EMNLP 2023 Demo Track"
authors:
  - Christina Adams
  - Marcus Feld
summary: "A harness and leaderboard for tokenizer quality across domains, with reproducible splits and sanity checks."
topics:
  - evaluation
  - tokenization
---

# Tokenizer Bench: A Reproducible Evaluation Harness

Christina Adams, Marcus Feld

## Abstract

Tokenizer Bench packages domain-specific corpora, frozen splits and a set of
sanity checks so that tokenizer comparisons are reproducible across research
groups. The demo shows the harness running on five languages and three
domains.

## Demonstration outline

1. Freeze a corpus and a split.
2. Train or download candidate tokenizers.
3. Run the quality suite and export a leaderboard entry.

## Appendix A — sanity checks

The harness refuses to score a tokenizer that fails any of the following:
round-trip losslessness, stable whitespace handling, or deterministic merges on
a fixed seed. These checks exist because early leaderboard submissions were
silently comparing different preprocessing pipelines.

## Appendix B — corpora

The public corpora cover legal, medical and conversational text. Private
corpora used in the paper are not redistributable; the harness accepts
user-supplied corpora through the same manifest format.

## Reproducibility notes

Every reported number is accompanied by a hash of the corpus manifest and the
tokenizer artifact. The demo prints both hashes next to the score so that a
reader can confirm they are comparing the same inputs.
