# Technical review notes

These notes were added during translation. The body of the English report retains the original report's numerical statements; its editorial appendix gives fuller explanations.

## Scope of the supplied work

The archive supports an analytical design and CAD project. It contains no separately saved CFD mesh, solver setup, residual history, pressure or velocity field, experimental pump curve, or cavitation validation. Describe it as “analytical impeller design and CFturbo modeling” in a portfolio. The empirical NPSHr screenshot is not evidence of a resolved cavitation simulation.

## Different design stages

The source's preliminary design uses an outlet diameter of 209 mm and width of 32 mm. The supplied CFturbo file stores 225.8 mm and 34.55 mm. Its suction-diameter field is 132.5 mm; the initial report assumes an eye diameter of 125 mm. These are stored parameters, not independently measured geometry.

The stored blade angle and thickness arrays also differ from the preliminary prose. The report later describes automatic angle calculation, so preserve the distinction between manually proposed values and the saved state.

## Terminology and calculations

- **DN 125:** the nominal suction connection, not the shaft diameter. The report separately gives a 32 mm coupling shaft and 45 mm hub.
- **Intermediate radius:** `sqrt((R1² + R2²)/2)` is a root mean square, not a geometric mean. It gives approximately 86.10 mm for the stated radii.
- **Single arc:** the stated formula and numbers give approximately 121.11 mm, compared with 120.9 mm in the source.
- **Continuation radius:** the later tangent-based blade construction gives 568.39 mm using the source's stated 82.30 mm intermediate radius and 5.26° intermediate angle. It should not be conflated with the earlier two-arc estimate using 97.7 and 159.1 mm radii.
- **Specific speed:** the value near 38.36 uses rpm, m³/s, and meters. State the unit convention.
- **Efficiency:** catalog efficiency, an assumed hydraulic efficiency, and software estimates are distinct. No measured efficiency for the new impeller is supplied.
- **Design heuristics:** the source's comments on shrouds, splitters, span count, edge profiles, and the Cordier diagram describe its design rationale. They are not universal design rules or substitutes for validation.

## File status

The native files are unchanged copies. The SolidWorks parts and generated macro have not been executed or checked in their native application. The generic part names do not identify which construction method they represent. The STEP export contains solids as well as surfaces and curves; inspect the import before claiming a finished single solid.

The report has two credited authors. Keep both credits and avoid describing the complete project as individual work unless the contributions are clarified.
