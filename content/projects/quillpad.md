---
title: "QuillPad: A Local-First Markdown Editor"
kind: project
year: 2023
status: "Released"
venue: "open source (v1.2.0)"
authors:
  - Christina Adams
summary: "A desktop Markdown editor that stores notes as plain files and merges edits without a server."
topics:
  - local-first
  - markdown
---

# QuillPad: A Local-First Markdown Editor

QuillPad keeps notes as plain Markdown files and treats the filesystem as the
source of truth. Concurrent edits are merged with a small operation log that
lives next to the notes, so no server is required.

## Features

- Direct file editing with atomic saves.
- Offline-first conflict resolution.
- Optional sync through any file-sync provider.
- Export to static HTML.

## Status

Version 1.2.0 is released and is the recommended build.
