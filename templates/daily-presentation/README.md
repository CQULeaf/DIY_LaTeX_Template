# Daily Presentation Beamer Template

A minimal XeLaTeX Beamer template for group meetings, research updates, course presentations, and short project reports.

## Files

```text
daily-presentation/
├── main.tex
├── collegeBeamer.sty
├── src/
│   └── CQU/
│       ├── background.png
│       ├── color-logo.png
│       └── trans-logo.png
└── LICENSE.source
```

## Quick Start

Compile with XeLaTeX:

```bash
latexmk -xelatex main.tex
```

Edit the reusable metadata block at the top of `main.tex`:

```latex
\newcommand{\PresenterName}{Yexuhang Ye}
\newcommand{\PresenterSchool}{Chongqing University}
\newcommand{\PresentationTopic}{Robotics Learning\\and Control}
\newcommand{\PresentationSubtitle}{Progress, Open Questions, and Next Steps}
```

Use `\\` in a long title to control the line break on the cover slide. Keep the optional short title in `\title[...]` on one line for PDF metadata and navigation.

## Template Notes

- The template uses a 16:9 Beamer layout.
- The default visual theme is Chongqing University (`cqu`).
- The cover page uses a large watermark logo on the right.
- Frame titles are aligned next to the upper-left logo.
- The default language is English.

## Customize

To change the theme assets, replace the files under `src/CQU/`:

```text
background.png
color-logo.png
trans-logo.png
```

To rename or extend the theme, add a new option in `collegeBeamer.sty` following the existing `cqu` option.

## Source

This template is adapted from the Beamer presentation theme in `Gua927/Latex_Template`. Source license details are kept in `LICENSE.source`.
