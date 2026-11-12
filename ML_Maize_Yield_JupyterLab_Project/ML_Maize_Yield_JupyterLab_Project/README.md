# Q1 Maize Yield — JupyterLab project

## Important dataset compatibility note
The assignment PDF describes a different schema (`farm_id`, `yield_kg_per_ha`, etc.) and a filename `maize_yield_rwanda_raw.csv`. The uploaded CSV used here is `maize_yield_rwanda_rw.csv`, with 1,426 rows, 20 columns and target `yield_t_ha`. Confirm with your lecturer that this is the correct dataset before submission. These notebooks are written for the actual uploaded CSV, not the schema described in the PDF.

## Open in JupyterLab
1. Extract this ZIP file.
2. Open Anaconda Prompt or CMD and move into the extracted project folder.
3. Install dependencies: `python -m pip install -r requirements.txt`
4. Start JupyterLab: `jupyter lab`
5. Open `q1_maize_yield/notebooks/01_acquire.ipynb`.
6. Run notebooks in order: `01_acquire`, `02_eda`, `03_clean`, `04_features`.

If you start JupyterLab from the project root, the notebooks locate the CSV relative to the `notebooks` folder. Keep the raw CSV in `q1_maize_yield/data/raw/`.

## Project structure
- `q1_maize_yield/data/raw/`: original supplied CSV; do not edit.
- `data/interim/`: cleaned dataset.
- `data/processed/`: transformed and engineered train/validation/test datasets.
- `notebooks/`: executable stage notebooks.
- `docs/`: generated data dictionary, source log, quality report, cleaning log and feature justification.

## Assignment boundaries
This project prepares data; it does not train a prediction model. Fill in group number and both student names in the notebook cover cells. Take genuine screenshots of code and outputs for every stage, as required by the assignment. Review and justify all decisions with your partner; do not submit results you cannot explain.

## Compatibility
Use Python 3.10 or newer. The `OneHotEncoder(sparse_output=False)` option requires a recent scikit-learn version (1.2+).
