# Waterloo Beamer deck (fraud detection presentation)

A 16:9 Beamer deck in University of Waterloo colours, reusing Nafisat's thesis-talk theme
(`beamerthemeWaterloo.sty`), built for the same 18-slide structure as `presentation-draft.pptx`.
Everything in `main.tex` is placeholder content, replace it as Task 7 finishes, same as the PowerPoint draft.

This file was written without a local LaTeX install to compile-test it against, check that it compiles
cleanly the first time you open it in Overleaf and fix anything XeLaTeX flags.

## Files

| File | What it is |
| --- | --- |
| `main.tex` | The deck. 18 slides: title, problem, RQs, dataset, both methods, both results, comparison, strengths/weaknesses, limitations, takeaways, closing, references, 4 appendix slides. |
| `beamerthemeWaterloo.sty` | The theme, copied unmodified from the thesis-talk template. Do not edit it, everything project-specific lives in `main.tex`. |
| `fonts/` | Barlow and Barlow Condensed (SIL Open Font License, see `fonts/OFL.txt`). |
| `figures/` | University of Waterloo logo and seal, used by the title, sidebar, and closing slides. |

## Put it on Overleaf

1. New Project > Blank Project.
2. Delete the default `main.tex`. Upload `main.tex` and `beamerthemeWaterloo.sty`.
3. Create two folders, `fonts` and `figures`, and upload the files of each folder into it.
4. Menu > Settings > **Compiler: XeLaTeX** (the fonts need it). Recompile.
5. Share the Overleaf project link with the team, Overleaf edits collaboratively in real time like Google Docs,
   no local LaTeX install needed.

## Filling it in

- Every `[bracketed]` placeholder is something Task 7 (or your own notebook) needs to supply: numbers, table
  cells, the one-line takeaways, the `\imgplaceholder{...}{...}` boxes (replace with `\includegraphics` once
  you have a saved plot file in `figures/`).
- Section labels on the left sidebar come from `\Section{...}` in `main.tex`, matching the site's task
  categories (Introduction, Data, Methods, Results, Comparison, Conclusion).
- Backup slides are everything after `\appendix`, they get the pink BACKUP label automatically.
