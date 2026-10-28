# EV Atlas — Electric Vehicle Market Insights

EV Atlas is a student project that presents electric vehicle dataset patterns through a Flask website, interactive Plotly charts, and a Tableau Public Story. This version uses a warm editorial visual theme with charcoal, burnt-orange, and olive accents.

## Features
- Flask-based web application
- Interactive Plotly visualizations and dataset filters
- Manufacturer, category, sales, regional, geographic, range/battery, and rating views (depending on available fields)
- Embedded Tableau Public Story
- Sample data for a quick local run

## Technology stack
Python, Flask, Pandas, Plotly, HTML, CSS, Tableau Public.

## Run locally
1. Install Python 3.10 or newer (or a version supported by the dependencies).
2. Download or clone this repository.
3. Open a terminal in the project folder.
4. Install dependencies:
   ```powershell
   python -m pip install -r requirements.txt
   ```
5. Run the application:
   ```powershell
   python app.py
   ```
6. Open the local address printed by Flask, usually `http://127.0.0.1:5000`.

## Dataset
The repository includes a small sample CSV for initial testing. To reproduce analysis using the full dataset, download the permitted source dataset and place the expected CSV in the `data/` folder. Check the filename and source instructions in `data/README.md` and `scripts/download_data.py`. Do not commit large data files or redistribute data unless its licence permits it.

## Tableau Story
The page currently embeds the shared Tableau Story configured in `templates/index.html`. Replace the temporary Story URL with the project owner's published Story URL before publishing or submitting this version. Tableau Public content and published data may be visible to anyone.

## Project structure
```text
app.py
requirements.txt
templates/
static/css/
src/
data/
scripts/
tests/
docs/
```

## Important interpretation note
The charts describe the available dataset. Record counts should not automatically be interpreted as real-world market share, and visual correlations do not establish causation.
