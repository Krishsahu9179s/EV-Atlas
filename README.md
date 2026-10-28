# EV Atlas — Electric Vehicle Market Insights

EV Atlas is a student data-analytics project that explores patterns in an electric-vehicle dataset through a responsive Flask website, interactive Plotly charts, and a Tableau Public Story. It uses a warm editorial interface with cream backgrounds, charcoal text, burnt-orange highlights, and olive accents to give the project a distinct visual identity.

## Project objectives

- Explore the electric-vehicle dataset and summarize its available fields.
- Compare manufacturers and vehicle categories in the supplied data.
- Review annual sales-related measures where those fields are available.
- Explore geographic distribution, customer ratings, and battery-related measures where supported by the dataset.
- Present key charts and findings in a web interface and a Tableau Story.
- Provide a reproducible starting point for further data analysis.

## Features

- Flask web application for presenting the analysis.
- Interactive Plotly charts and dataset filters.
- Views for manufacturer, category, sales, geography, ratings, and battery/range-related fields, depending on the fields present in the dataset.
- Embedded Tableau Public Story.
- Sample CSV included for a quick local run.
- Separate data-loading and analytics modules.
- Documentation, a data-download helper, and basic analytics tests.

## Technology stack

- **Language:** Python
- **Web framework:** Flask
- **Data analysis:** Pandas
- **Interactive charts:** Plotly
- **Frontend:** HTML and CSS
- **Dashboard/storytelling:** Tableau Public

## Getting started

### Requirements

- Python 3.10 or a newer version supported by the dependencies.
- Internet access if downloading the full dataset or viewing the published Tableau Story.

### Installation

1. Download or clone this repository and open the project folder in a terminal.
2. Install the dependencies:

   ```bash
   python -m pip install -r requirements.txt
   ```

3. Start the Flask application:

   ```bash
   python app.py
   ```

4. Open the local URL printed in the terminal. It is usually `http://127.0.0.1:5000`.

## Dataset setup

A small sample CSV is included in `data/` so the application can be tried without downloading the full dataset. For a fuller analysis:

1. Read `data/README.md` and review `scripts/download_data.py`.
2. Obtain the dataset from its permitted source.
3. Place the CSV at the expected location and use the expected filename described by the project scripts.
4. Check the column names and missing values before interpreting the charts.

The full dataset is not bundled with this repository. Do not upload or redistribute data unless its licence and source terms permit it.

## Tableau Public Story

The website contains an embedded Tableau Story. Before publishing or submitting this project, replace the temporary Tableau URL in `templates/index.html` with the project owner's own published Story URL. Tableau Public workbooks and their published data may be visible to the public, so only publish data that is permitted to be shared.

## Repository structure

```text
app.py                         Flask application entry point
requirements.txt               Python dependencies
templates/index.html           Main web page
static/css/                    Website styles and EV Atlas theme
src/analytics.py               Analytics and chart-support logic
src/data_loader.py              Dataset loading and preparation
data/ev_market_sample.csv       Small sample dataset
data/README.md                  Dataset setup notes
scripts/download_data.py        Dataset download helper
tests/test_analytics.py         Basic analytics tests
docs/tableau_guide.md           Tableau dashboard/story guidance
docs/project_report.md          Project report draft
assets/dashboard_screenshots/   Location for dashboard screenshots
```

## Interpretation and limitations

- Results describe the dataset supplied to the application; they do not automatically represent the entire electric-vehicle market.
- A count of dataset records is not the same as market share unless the dataset and calculation explicitly support that interpretation.
- Missing values and differences in data coverage can affect comparisons.
- Correlation between two fields does not prove that one causes the other.
- Verify chart values and document the dataset source, cleaning decisions, and limitations before presenting final conclusions.

## Suggested next steps

- Add screenshots of the final website and Tableau Story.
- Record the actual dataset source and licence.
- Replace the temporary Tableau embed URL.
- Run the tests and record the results you actually observe.
- Personalize the analysis and conclusions based on your own review of the data.

## License

See the `LICENSE` file for the repository's license. Dataset licensing may be separate from the code license.
