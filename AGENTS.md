# Repository Guidelines

## Project Structure & Module Organization
This repository is a collection of Engineering Equation Solver (EES) problem solutions for the Stoecker & Jones text. Content is organized by chapter folders named `CH##_Topic`, each containing problem files like `P##_##.EES`. A few chapters include short notes such as `ch18_note.txt` or `Ch16_note.txt`, and one chapter includes a Mathematica notebook (`.nb`). There is no conventional source/test split; the chapter folders are the primary units of organization.

## Build, Test, and Development Commands
There is no automated build or test suite in this repo. Work is done directly in EES:
- Open a problem file in EES, e.g. `CH10_the_Vapor_Compression_Cycle/P10_1.EES`.
- Run the solver within EES to compute results and verify equations.

## Coding Style & Naming Conventions
- Use EES syntax and formatting; prefer clear variable names and consistent units.
- Keep filenames aligned with the existing pattern: `P<chapter>_<problem>.EES` inside the matching `CH##_*` folder.
- Notes or explanations should be short text files (e.g., `ch##_note.txt`) and stay with the chapter they describe.

## Testing Guidelines
There are no automated tests. Validation is manual:
- Recalculate in EES and confirm outputs match expected values or the textbook results.
- If you add a new solution, mention any assumptions or reference values in a comment or adjacent note file.

## Commit & Pull Request Guidelines
Recent history uses simple, imperative messages such as "Add files via upload" or "Update README.md". Keep commit messages short and action-oriented.
For pull requests:
- Describe the chapter/problem numbers added or changed.
- Note any assumptions, property tables, or reference sources used.
- Include before/after solver outputs if a solution was modified.

## Security & Configuration Tips
EES files may rely on local property databases. If results differ, confirm the EES version and fluid property settings before changing equations.
