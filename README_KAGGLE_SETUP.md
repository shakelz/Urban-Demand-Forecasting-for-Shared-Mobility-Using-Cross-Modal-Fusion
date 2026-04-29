# Abdul Thesis Kaggle Code Package

Seven standalone notebooks are included, one for each research question. Each notebook loads UCI Bike Sharing `hour.csv`, engineers temporal/weather/calendar/neighborhood features, trains models, and saves outputs under `/kaggle/working/outputs/`.

## How to run on Kaggle

1. Open Kaggle → Code → New Notebook.
2. Upload one `.ipynb` file from this package.
3. In the right sidebar, click **Add Input**.
4. Add any Kaggle dataset containing the UCI Bike Sharing Dataset file `hour.csv`, or upload the original UCI `hour.csv` manually.
5. Run all cells.
6. Download generated PDFs from `/kaggle/working/outputs/figures/` and CSV tables from `/kaggle/working/outputs/tables/`.

## Dataset note

The proposal mentions UCI Bike Sharing and NYC TLC data. These notebooks use UCI Bike Sharing as the primary reproducible dataset because it already contains hourly demand, weather, season, holiday, weekday, and working-day fields. Since UCI is system-level rather than station-level, the notebooks create deterministic synthetic station/neighborhood descriptors to implement the neighborhood-aware methodology. For final thesis results, replace these synthetic descriptors with real station metadata, POI density, land-use, census, and transit-access features.

## Outputs

- Figures: PDF format.
- Tables: CSV format.
- All paths are printed during execution.

## Practical recommendation

Start with RQ1 to verify the dataset path and output generation. Then run RQ2–RQ7 independently.
