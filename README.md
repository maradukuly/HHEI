# Heller Hurwicz Economics Institute (HHEI)

**Fall 2026 research project**

**The Costs of Capital: How War Diminishes Human Capital and Skill Formation Over Time**

**Advisor:** Dr. Joseph Mullins

**Research assistants:** Mara Dukuly and Advaith Suresh

## Research overview

This project studies how conflict disrupts human-capital formation and whether those disruptions persist after conflict ends. The empirical work focuses on applying growth accounting to measure conflict exposure and potential spillovers across borders. The theoretical work examines how interruptions to education, parental investment, and learning-by-doing may affect skill accumulation and longer-run economic outcomes.

**Status:** In progress. Analyses and models are under development.

## Methodology

The empirical data work combines individual-level Demographic and Health Survey (DHS) data with georeferenced conflict events. Current analyses build measures of school-age and geographic conflict exposure; the broader empirical approach is developing.

The modeling work develops a dynamic human-capital framework in which individuals invest in skills over time. Conflict can disrupt that investment and contribute to persistent or intergenerational effects.

## Repository guide

- **`data/`** — Local, ignored data grouped by source: DHS, UCDP, Correlates of War, IPUMS DHS, and geographic files.
- **`empirical/`** — Quarto documents for data exploration and conflict-data analysis.
- **`modeling/`** — Theoretical model notes, papers, and notebooks on household optimization and shooting methods.
- **`supplement/`** — Supplementary programming material.
- **`outputs/`** — Generated conflict maps and figures; new files are ignored by Git.

## Replication

The repository does not yet have a single end-to-end replication script. To run an analysis:

1. Use Python 3.11 or later and install the listed packages:

   ```bash
   python -m pip install -r requirements.txt
   ```

   Dependency declarations are also listed in `pyproject.toml`.

2. Install [Quarto](https://quarto.org/) to render `.qmd` documents.
3. Obtain the required input data and place it in the corresponding subfolder under `data/`. This directory is intentionally ignored by Git and is not included in repository checkouts. Some source microdata may require provider access or approval.
4. Run the notebook or render the Quarto document from its source, following its cells or sections in order. Check each document for its specific inputs and sample definitions.

Some analyses remain exploratory, and the country-year UCDP input used by the screening analysis is not currently included in the local data directory. Reproduction may depend on the exact data release and processing choices. Cite original data providers and check their terms before reusing or redistributing source data.

## References

The project's working reference library is available in the [HHEI Zotero group](https://www.zotero.org/groups/6476302/thebeesfromthehive/library).
