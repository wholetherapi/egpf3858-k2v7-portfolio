---
title: "Confidence-Gated Speculative Decoding for Long-Context Serving"
kind: paper
year: 2026
status: "Under Review"
venue: "ICML 2026 (submitted)"
authors:
  - Christina Adams
  - Priya Raman
  - Tobias Ling
summary: "A draft-and-verify decoding scheme that gates speculation on calibrated confidence to keep long-context serving latency predictable."
topics:
  - efficient inference
  - decoding
  - long context
---

# Confidence-Gated Speculative Decoding for Long-Context Serving

Christina Adams, Priya Raman, Tobias Ling

## Abstract

Speculative decoding accelerates generation by letting a small draft model
propose tokens that a larger verifier checks in parallel. On long-context
workloads the acceptance rate drifts as the draft model loses track of far
context, so a fixed speculation length wastes verifier capacity. We gate
speculation on a calibrated confidence score and shorten the draft window when
the score falls outside a tolerance band.

## Approach

1. Score each draft token with a calibrated head.
2. Accept only the longest prefix whose aggregate score stays inside the band.
3. Re-estimate the band online from a rolling window of acceptance statistics.

## Notes

The evaluation harness is described in the draft; links will be added when the
artifact is public.
