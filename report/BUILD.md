# Building the report

## Overleaf

1. Upload the complete project ZIP using New Project → Upload Project.
2. In project settings, select `report/main.tex` as the main document. If Overleaf retains the outer repository folder, select the file at that nested path.
3. Set the compiler to pdfLaTeX.
4. Recompile; a second pass resolves the table of contents and bookmarks.

The CAD folders are not needed for LaTeX compilation, but can remain in the uploaded project. To make a smaller Overleaf project, upload only `main.tex` and `figures/` from the report directory, preserving their relative paths, then select `main.tex`.

## Local compilation

From the repository root:

```bash
cd report
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
```

The result is `report/main.pdf`.

The report uses standard LaTeX packages: fontenc, inputenc, lmodern, geometry, amsmath, amssymb, graphicx, booktabs, array, microtype, float, placeins, caption, hyperref, and fancyhdr. No custom fonts, bibliography database, external CAD application, or shell escape are required.

The document was compiled with pdfLaTeX from TeX Live 2023. All figures required by the source are supplied as PNG files. The extra original EMF annotation is preserved for provenance but is not required to compile the report.
