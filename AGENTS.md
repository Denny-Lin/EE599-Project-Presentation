# Agent instructions

This repo is one Beamer deck assembled from one file per teammate (see README.md, "Who edits what").

- Edit only the section file and the `figures/<name>/` folder of the person you are working for. `main.tex`,
  `preamble.tex`, `sections/intro.tex`, `sections/conclusion.tex`, the `solo_*.tex` files and `.github/` belong to
  Renzhi: change them only when he asks.
- Personal macros go at the top of the owner's own file, with the owner's name as a prefix; never in `preamble.tex`.
- Build the owner's part with `latexmk -pdf solo_<name>.tex` and fix every error before committing. Commit no build
  files and no PDFs other than figures; CI writes `main.pdf`.
- Keep slides readable: no more than about 6 bullets a frame, figures at least half the frame wide.
