# FSE Risk-Guided ADS Manuscript

This archive is ready to upload as a new Overleaf project. `main.tex` is the root file and uses ACM's `acmart` review format.

## Project layout

```text
main.tex
references.bib
figures/
  scenario_taxonomy.png
  generation_workflow.png
sections/
  01_introduction.tex
  02_background.tex
  03_related_work.tex
  04_approach.tex
  05_experimental_design.tex
  06_results.tex
  07_discussion.tex
  08_conclusion.tex
legacy/
  ...original ASE sources, bibliography files, and images...
```

The files under `legacy/` are preserved for reference and are not included by `main.tex`. The clean manuscript removes the roundabout method, experiment, result, and conclusion material.

## Upload to Overleaf

1. In Overleaf, choose **New Project → Upload Project**.
2. Upload the ZIP file.
3. Confirm that `main.tex` is selected as the main document.
4. Use the standard pdfLaTeX compiler. Overleaf supplies `acmart` and `ACM-Reference-Format.bst`.

## Items that must be replaced

- **Venue metadata:** Replace the `FSE 'XX`, date, and location placeholders in `main.tex` with the exact metadata for the target FSE cycle.
- **Authors:** Keep the anonymous settings for review; restore names and affiliations only for the required submission stage.
- **Bibliography:** The root `references.bib` now uses the verified entries from the original ASE bibliography supplied as `references_ase.bib`. It covers every citation used by the clean FSE manuscript. The exact supplied file is preserved as `legacy/references_ase.bib`.
- **Figures:** `figures/scenario_taxonomy.png` and `figures/generation_workflow.png` are deliberately simple placeholders. Replace them with final images using the same filenames, or update the paths in `sections/04_approach.tex`. Original image candidates are preserved in `legacy/imgs/`.
- **Experimental reporting:** Add exact software versions, hardware, random seeds, search budgets, repetitions, statistical analyses, and artifact URL.
- **FSE revision experiments:** The checklist at the end of `sections/05_experimental_design.tex` records the recommended seed-selection, search, open/closed-loop, and diversity ablations.

## Bibliography comparison

The earlier root bibliography contained 41 compile-only placeholders. The supplied ASE bibliography contains 361 unique real citation keys and covers all 27 keys used by the clean FSE manuscript. The placeholder file was therefore replaced with the ASE bibliography. The supplied file contained two real records under the key `menzel_scenarios_2018`; the published conference record keeps that key, while the second arXiv record is named `menzel_scenarios_2018_arxiv` in the root bibliography to avoid a duplicate-key BibTeX error. No bibliographic fields were changed.

## Legacy material

`legacy/` contains exact copies of the recovered source files and original images. Edit the clean files at the project root and under `sections/`; treat `legacy/` as read-only backup material.
