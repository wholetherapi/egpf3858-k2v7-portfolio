---
title: "ShardCraft: Deterministic Sharding for Time-Series Stores"
kind: paper
year: 2022
status: "Published"
venue: "USENIX ATC 2022"
authors:
  - Christina Adams
  - Marc Oyelaran
summary: "A sharding planner that makes range placement reproducible across cluster restarts."
topics:
  - storage
  - distributed systems
---

# ShardCraft: Deterministic Sharding for Time-Series Stores

Christina Adams, Marc Oyelaran

## Abstract

ShardCraft computes a deterministic placement plan for time-series ranges so
that a restarted cluster converges to the same layout without a central
coordinator. The planner combines a hash of the time range with the cluster
topology fingerprint and reconciles only the shards whose owners changed.

## Results

- Replanning a 64-node cluster takes under two seconds.
- Restart convergence uses 6x less data movement than the baseline.
- The plan is reproducible from the same inputs and seed.

## Appendix

The full evaluation traces and the planner's configuration grammar are
included in the paper's artifact. The page is kept in the archive because the
project concluded in 2022.
