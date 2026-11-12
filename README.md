# Field Notes — Christina Adams

Source for the personal research portfolio at `fieldnotes.example`. The site is
plain Markdown rendered by a very small static generator; every entry is a page
under `content/` with a YAML front-matter block.

## Repository layout

```
content/
  papers/      paper entries
  projects/    software and tool entries
  talks/       talks and seminar entries
  archive/     older entries, grouped by year
changelog/     short monthly notes about site maintenance
layouts/       one HTML template
assets/        stylesheet and images
```

## Selected work

- **Confidence-Gated Speculative Decoding for Long-Context Serving** — ICML 2026
  submission. Draft-and-verify decoding with a calibrated acceptance gate.
- **Neural Signatures for Program Semantics** — TMLR 2025 journal version;
  the earlier NeurIPS 2024 workshop version is kept for reference.
- **StreamDB** — an embedded append-only event store with deterministic
  compaction (open source).
- **QuillPad** — a local-first Markdown editor (open source).
- **HexGrid** — realtime hexbin map rendering for large datasets.
- **What Scaling Laws Actually Tell Us** — invited seminar, MLSys Community
  Seminar 2025.

Older material is kept under `content/archive/`; see the changelog notes for
when pages were moved.

## Front matter

```yaml
title:    display title
kind:     paper | project | talk
year:     integer
status:   Under Review | Accepted | Published | Superseded | Released | Invited
venue:    free-form venue or release line
authors:  list of names
summary:  one-sentence description
topics:   list of topic tags
code:     optional public repository URL with a released implementation
```

The template renders `code` as a "Code" link only when the field is present.
The field is deliberately left out when an implementation is not available.

## Local preview

```bash
python -m fieldnotes.build --serve
```

The build copies `content/` into the output tree and renders each page with
`layouts/default.html`.

## Housekeeping

- Keep author lists unchanged unless a correction is explicitly recorded.
- Do not rewrite prose in existing entries during maintenance passes; only the
  metadata that is demonstrably out of date should change.
- Monthly notes live in `changelog/` and are not part of the public site.

## License

Text is CC-BY-4.0; code samples are MIT.
