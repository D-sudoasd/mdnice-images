<p align="center">
  <img src="assets/readme/hero.png" width="100%" alt="mdnice-images — Stable image assets for Markdown articles / 用于 Markdown 文章的稳定图片资源. Conceptual illustration / 概念插图。">
</p>

# mdnice-images

**Stable image assets for Markdown articles**

**用于 Markdown 文章的稳定图片资源**

[Overview / 项目概览](#overview--项目概览) · [Start / 开始使用](#start--开始使用) · [Reference / 详细说明](#reference--详细说明)

## Overview / 项目概览

Keep article covers, figure panels and source cards in a public asset tree that can be linked from mdnice and other Markdown publishing workflows.

在公开资源目录中保存文章封面、图版与来源卡片，供 mdnice 和其他 Markdown 发布流程引用。

- **Article organization** — 按文章整理图片与关联素材。
- **Stable links** — 使用明确文件名并保留已发布路径。
- **Source-aware reuse** — 按各图件来源与许可决定复用方式。

## Start / 开始使用

Browse [synchrotron-column/](synchrotron-column/) and copy the raw URL of the selected image.

浏览 `synchrotron-column/`，复制所选图片的原始文件链接并插入 Markdown。

```markdown
![Image description / 图片说明](https://raw.githubusercontent.com/D-sudoasd/mdnice-images/main/assets/readme/hero.png)
```

This repository hosts assets; it does not run an application. Keep published image paths stable.

本仓库保存图片资源，无需运行应用；已发表文章引用的图片路径应保持稳定。

*Cover: AI-generated conceptual illustration. 封面为 AI 生成的概念插图。*

## Reference / 详细说明

**Public image host for mdnice / WeChat copy-ready Markdown columns.**

Not an application — a public asset tree so column posts can reference **stable GitHub raw URLs** when pasting into [mdnice](https://mdnice.com/) or WeChat editors.

## Layout

| Path | Role |
|------|------|
| `synchrotron-column/` | Synchrotron / diffraction column figures, covers, and source cards |
| `synchrotron-column/<article>/` | Nested per-article figure packs (example: `barriobero_vila_2017_ti662_hexrd_column/`) |
| `assets/readme/` | README cover and section illustrations |

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
