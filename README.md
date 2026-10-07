<p align="center">
  <img src="assets/readme/hero.png" width="100%" alt="mdnice-images — Stable image assets for Markdown articles / 用于 Markdown 文章的稳定图片资源. Conceptual illustration / 概念插图。">
</p>

# mdnice-images

**为 Markdown 与 mdnice 文章保存可直接引用的公开图片。**

A public image repository for the maintainer’s synchrotron and diffraction columns. Browse the figures, copy a raw GitHub URL, and embed it in your article; there is no application to install.

[图片目录](synchrotron-column/) · [Ti-662 原位衍射文章图包](synchrotron-column/barriobero_vila_2017_ti662_hexrd_column/) · [引用方法](#embed) · [复用范围](#scope-and-reuse)

## 从一张真实资源开始

![文章图件：衍射环数据整理示意](synchrotron-column/01-diffraction-ring-data-sorting.png)

*这是仓库中的文章配图，作为资源示例展示；科学含义及来源以对应文章和图包记录为准。*

```markdown
![衍射环数据整理示意](https://raw.githubusercontent.com/D-sudoasd/mdnice-images/main/synchrotron-column/01-diffraction-ring-data-sorting.png)
```

添加新资源时使用明确文件名；已被文章引用的路径应保持稳定。`main` 链接反映当前文件；需要固定历史版本时，用提交 SHA 替换 URL 中的 `main`。

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
