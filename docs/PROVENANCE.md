# Provenance

## Supplied source

The user supplied `Proj1.rar`, containing a Persian Word report and these seven CAD-related files:

- `CFTurbo/Proj1.cft`
- `CFTurbo/Proj1.stp`
- `CFTurbo/Proj1.swb`
- `Solidworks/Part1.SLDPRT`
- `Solidworks/Part2.SLDPRT`
- `Solidworks/Junk/Part1.SLDPRT`
- `Solidworks/Junk/Part2.SLDPRT`

They are copied into the repository under `cad/`, with the same relative paths and identical bytes. See `SHA256SUMS.txt`. No native project settings, CAD topology, or macro logic were changed.

## English report

The Persian Word report was translated and typeset as `report/main.tex`, with its two phases, calculations, tables, construction steps, and substantive figures retained. The English report is not a new independent design study. Editorial qualifications and a separate appendix distinguish documented evidence from broader statements in the source.

The source credits Pouya Asghari and نیلوفر فتاحی. The latter is transliterated as Niloufar Fattahi; the preferred Latin spelling should be confirmed. Student numbers are omitted from the English edition. The original Word report is not included in this public-facing package.

The source contains 52 image relationships: 51 substantive images including the two cover logos, plus a small repeated EMF annotation of the letter K. Original raster images and the EMF are retained in `report/figures/`; a PNG rendering of the K annotation is also supplied. The main figure captions identify point K without treating its tiny overlay as a separate figure. Repeated occurrences of the same edge-design screenshot are retained in the translated report.

Figures include author-created CAD screenshots and embedded Pumpiran catalog extracts. No figures were regenerated with AI. The translation, LaTeX typesetting, repository documentation, and editorial review were prepared with AI assistance.

## Validation performed

- Extracted the archive and inventoried all contained files.
- Read the complete report text, equations, tables, and images.
- Parsed the native CFturbo XML and inspected the STEP and macro text.
- Checked selected hand calculations and compared the preliminary and stored design parameters.
- Compiled the English report with pdfLaTeX and inspected its rendered pages.
- Checked original CAD copy hashes and the repository archive integrity.

No CFturbo recomputation, SolidWorks rebuild, macro execution, downstream CFD simulation, manufacturing check, or experimental validation was performed.
