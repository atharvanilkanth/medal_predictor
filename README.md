# Medal Predictor

Predicts Olympic medals for a team using features derived from `teams.csv` and exploratory analysis in `medal_predictor.ipynb`.

## Files
- `teams.csv` — team-level Olympic features and medal counts
- `medal_predictor.ipynb` — analysis notebook (loading, feature selection, correlations, plots)

## Dataset columns
- `team`, `country`, `year`
- `events`, `athletes`
- `age`, `height`, `weight`
- `medals`
- `prev_medals`, `prev_3_medals`

## How to run
1. Install dependencies:
   - Python 3
   - pandas
   - seaborn
   - matplotlib
   - jupyter
2. Put `teams.csv` in the project root (same folder as the notebook).
3. In the notebook, make sure the CSV path is relative, e.g.:
   - `pd.read_csv("./teams.csv")`
4. Run all cells in `medal_predictor.ipynb`.

## Notes
Some rows may have missing values in `prev_medals` / `prev_3_medals`; handle NaNs as needed.
