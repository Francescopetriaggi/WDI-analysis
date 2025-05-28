# Environmental Footprint vs Human Development (1990-2023)

### *Who pays the highest price?*

Notebook-based study that measures how **CO₂ emissions** and **Material Footprint** reduce the Human Development Index (HDI) in 193 countries over 34 years.

---

## Preview

<p align="center">
  <img src="assets/heatmap.png"  width="45%" alt="Correlation heatmap">
  <img src="assets/improvement.png" width="45%" alt="Top improvements vs setbacks">
</p>

---

## Repository layout

| Path | Description |
|------|-------------|
| `WDI_analysis_EN.ipynb` | English notebook – data-prep, EDA, maps, trends, quadrants, conclusions. |
| `WDI_analysis_IT.ipynb` | Italian notebook – same code, Italian commentary. |
| `assets/` | PNG previews used in this README (`heatmap.png`, `improvement.png`, `top10_penalized_countries.png`). |
| `requirements.txt` | Tested Python package versions. |
| `LICENSE` | MIT license for code & notebooks. |

---

## Quick start (local)

```bash
git clone https://github.com/Francescopetriaggi/WDI-analysis.git
cd WDI-analysis

python -m venv .venv && source .venv/bin/activate    # optional
pip install -r requirements.txt

# ---- 1-minute manual step ----
# Download the World Bank WDI CSV (~178 MB) from
# https://datacatalog.worldbank.org/search/dataset/0037712/World-Development-Indicators
# unzip it and copy the largest *_Data.csv file to:
#   data/wdi.csv
# --------------------------------

jupyter lab WDI_analysis_EN.ipynb
