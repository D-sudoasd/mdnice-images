# mdnice-images

**Public image host for mdnice / WeChat copy-ready Markdown columns.**

Not an application — a public asset tree so column posts can reference **stable GitHub raw URLs** when pasting into [mdnice](https://mdnice.com/) or WeChat editors.

<p align="center">
  <img src="assets/readme/hero.svg" width="100%" alt="mdnice-images: public asset host for Markdown columns.">
</p>

## Layout

| Path | Role |
|------|------|
| `synchrotron-column/` | Synchrotron / diffraction column figures, covers, and source cards |
| `synchrotron-column/<article>/` | Nested per-article figure packs (example: `barriobero_vila_2017_ti662_hexrd_column/`) |
| `assets/readme/` | README hero / section SVGs only |

Filenames are descriptive (covers, fig panels, source cards, DESY visit guides, etc.). Prefer adding new files over renaming ones already linked from published posts.

## Embed

```markdown
![Short description](https://raw.githubusercontent.com/D-sudoasd/mdnice-images/main/path/to/figure.png)
```

Example (adjust path to a real file):

```markdown
![In-situ SXRD geometry](https://raw.githubusercontent.com/D-sudoasd/mdnice-images/main/synchrotron-column/fig1-in-situ-sxrd-geometry.png)
```

Tips:

- Prefer descriptive filenames and keep mobile-friendly file sizes.
- Avoid overwriting assets already linked from published posts.
- `main` branch raw URLs are the intended stable form; pin a commit SHA in the URL only if you need an immutable historical snapshot.

## Scope and reuse

| Intended | Not intended |
| --- | --- |
| Hosting figures for the maintainer’s Markdown / WeChat columns | A general CDN or upload API |
| Stable raw.githubusercontent.com links | Guaranteed long-term mirror outside GitHub |
| Personal / column illustration packs | Redistribution of third-party figures without checking provenance |

**Check provenance before reuse outside personal columns.** Some images illustrate published papers or facility visits; embedding here does not transfer journal or photographer rights. When in doubt, do not reuse.

## Contributing

This repository is primarily an asset dump for column publishing. Open an issue if a linked path 404s after a rename, or if a license / attribution note should sit next to a specific pack.

No install, no runtime, no tests — clone or browse on GitHub only.
