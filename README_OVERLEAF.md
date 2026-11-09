# Paper A -- Overleaf / journal submission package

Upload this whole zip to Overleaf (New Project -> Upload Project).  Set `main.tex` as main document.
Compiler: pdfLaTeX (TeX Live 2023 or newer).  Needs only packages found in standard TeX Live
(amsmath, mathtools, siunitx, booktabs, cleveref, subcaption, hyperref).

| File | What it is | Compile |
|---|---|---|
| `main.tex` + `sections/` + `references.bib` | the manuscript (48 pages, 12 pt) | set as main; pdflatex, bibtex, pdflatex x2 (Overleaf does this automatically) |
| `abstract.tex` | abstract only | compile alone -> `abstract.pdf` |
| `highlights.tex` | five highlight bullets (each <= 85 characters) | compile alone |
| `cover_letter.tex` | cover letter | compile alone |
| `figures/` | the ten figures, all vector PDF (fig01..fig10) | included by `main.tex` |

To compile a standalone file in Overleaf: Menu -> Main document -> choose that file.

## You must fill in (left as placeholders on purpose)
* `main.tex`: `\author{...}` (name, affiliation), and add acknowledgement, funding, CRediT, competing
  interests sections if the journal asks.
* `cover_letter.tex`: everything in [square brackets] (author, journal, editor, date); confirm the
  originality statement.
* Change `\documentclass`/layout to the target journal's template if required (all content is in
  `sections/`, so only `main.tex` needs changing).

The `.bib` has 61 entries, each with a DOI.  The manuscript contains no reference to code or data files.  `main.tex` has a data-availability line ("included in this article; further detail on reasonable request"); change it to the journal's wording if needed.
