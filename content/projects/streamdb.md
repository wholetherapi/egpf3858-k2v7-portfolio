---
title: "StreamDB: Append-Only Event Store"
kind: project
year: 2024
status: "Released"
venue: "open source (v0.9.2)"
authors:
  - Christina Adams
  - Marc Oyelaran
summary: "An embedded append-only event store with time-indexed scans and deterministic compaction."
topics:
  - storage
  - event sourcing
code: "https://github.com/wholetherapi/egpf3858-k2v7-streamdb-archive"
---

# StreamDB: Append-Only Event Store

StreamDB stores events as immutable segments and answers time-range scans from a
compact index. Compaction is deterministic: replaying the same segment set in
the same order always produces the same output files.

## Features

- Append-only writes with group commit.
- Time-indexed scans without loading the whole segment.
- Deterministic compaction for reproducible snapshots.
- Single-file embedded deployment.

## Status

Version 0.9.2 is the current public release. The pre-1.0 prototype is no longer maintained
and is not part of the current release.
