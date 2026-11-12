---
title: "HexGrid: Realtime Hexbin Map Rendering"
kind: project
year: 2023
status: "Released"
venue: "open source (v0.4.1)"
authors:
  - Christina Adams
  - Lena Vogt
summary: "A rendering layer for large hexbin maps with incremental aggregation and smooth zooming."
topics:
  - visualization
  - rendering
code: "https://github.com/pmcxs/hexgrid"
---

# HexGrid: Realtime Hexbin Map Rendering

HexGrid aggregates points into hexagonal bins on the fly and updates only the
bins that changed when the viewport moves. The result is smooth zooming on
datasets that would otherwise require a full re-bin at every frame.

## Features

- Incremental aggregation per viewport change.
- GPU-friendly bin buffers.
- Stable bin identifiers across zoom levels.
- Optional clustering overlay.

## Status

Version 0.4.1 was the last release published from this account. A similarly
named project upstream is maintained by other people and is not the
implementation described here.
