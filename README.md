# HIDDEN GEM Workflow Explorer

A GitHub Pages-ready, interactive HTML dashboard for exploring the *published workflow and aggregate study-level facts* reported in Popov et al. (2024).

## Important scope
- This is a visualization and educational companion. It does **not** execute HIDDEN GEM, docking, model generation, similarity searching, or virtual screening.
- It contains no compound-level records, structures, identifiers, candidate rankings, or candidate selection tools.
- Target-level enrichment charts are blank until you provide a CSV of aggregate values transcribed from the paper/supplementary material. No missing values are fabricated.
- The published article describes computational nominations; computational enrichment is not experimental validation.

## Run locally
Open `index.html` in a modern browser. Internet access is required for Chart.js (loaded from jsDelivr CDN).

## Deploy with GitHub Pages
1. Create a new GitHub repository.
2. Upload the contents of this ZIP (the `index.html`, `README.md`, and `data/` folder).
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then save.
6. Wait for the Pages deployment to finish; GitHub will show the site URL in Settings → Pages.

## Aggregate CSV format
Use `data/target_enrichment_template.csv` as the header template:
- `target_id`: a short, neutral label such as `Target 01`
- `ef1000`: the published EF1000 numeric value for that target

Only enter aggregate target-level metrics. Do not add molecular structures, SMILES strings, compound IDs, or candidate-level records.

## What is included
- Interactive workflow stage explorer
- Chart of computational scale values stated in the article
- Upload control for target-level aggregate EF1000 values
- Source and interpretation notes

## Source
Popov et al. (2024), “Hit Discovery using Docking ENriched by GEnerative Modeling (HIDDEN GEM): A Novel Computational Workflow for Accelerated Virtual Screening of Ultra-large Chemical Libraries,” *Molecular Informatics*.
