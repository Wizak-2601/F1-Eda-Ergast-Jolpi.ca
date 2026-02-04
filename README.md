# Pit Stop Paradox — F1 Strategy Analytics

## What This Project Is
This project explores the **Pit Stop Paradox** in Formula 1: why pitting during Safety Car periods can *gain* positions instead of losing them.  
It includes:
- A Jupyter notebook (`Analysis.ipynb`) for exploratory data analysis.
- An interactive, story‑driven blog page (`pit_stop_paradox.html`) with embedded Plotly/Bokeh visuals.
- Exported interactive charts in `plots/` for iframe embedding.

## Repo Setup
### 1) Create and activate a virtual environment
```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 2) Install dependencies
If you have a `requirements.txt`, install from it:
```bash
pip install -r requirements.txt
```
If not, install the common packages used in the notebook:
```bash
pip install pandas numpy plotly bokeh ipywidgets
```

### 3) Run the notebook
```bash
jupyter notebook
```
Open `Analysis.ipynb` and run the cells top‑to‑bottom.

## Viewing the Blog Page
The blog (`pit_stop_paradox.html`) embeds Plotly charts via iframe files in `plots/`.  
To ensure everything loads, serve the folder locally:
```bash
python3 -m http.server
```
Then open:
```
http://localhost:8000/pit_stop_paradox.html
```

## Notes
- Exported charts live in `plots/` (e.g., `positions_gained.html`).
- Data files are stored under `data/`.

