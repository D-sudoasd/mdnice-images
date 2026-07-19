<p align="center">
  <img src="assets/readme/hero.svg" width="100%" alt="mdnice-images: public image hosting for mdnice and WeChat Markdown columns.">
</p>

# mdnice-images

**Image hosting for mdnice and WeChat copy-ready Markdown.**

This repository is **not an application**. It stores figure and cover assets used by Markdown columns (for example under `synchrotron-column/`) so posts can reference **stable GitHub raw/CDN URLs** when pasting into [mdnice](https://mdnice.com/) or WeChat editors.

## What lives here

| Path | Role |
|------|------|
| `synchrotron-column/` | Synchrotron / diffraction technical-column figures and covers |
| Nested paper folders | Per-article figure sets (workflow, mechanism, covers) |

Treat folders as **named asset packs**. Prefer descriptive filenames; avoid overwriting files that are already linked from published posts.

## How to use an image in Markdown

1. Browse to the file on GitHub.  
2. Open the raw file URL (or use a CDN front if you prefer).  
3. Embed in Markdown:

```markdown
![Short description of the figure](https://raw.githubusercontent.com/D-sudoasd/mdnice-images/main/path/to/figure.png)
```

4. Paste into mdnice / WeChat workflow as usual.

## Conventions

- Prefer PNG/WebP for diagrams; keep file sizes reasonable for mobile readers.  
- Covers may include Chinese/English text baked into the image for platform requirements.  
- Do not commit secrets, unpublished lab data, or personal QR codes unless intentional and reviewed.  

## Contributing

New assets: add under a clear topic folder, use unique names, and open a PR if you maintain this repo collaboratively. Update this README only when the top-level layout changes.

## License

Unless a file states otherwise, check repository settings / file provenance before reuse outside personal columns.
