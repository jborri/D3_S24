# Bestseller Trends with D3

Interactive D3 visualizations exploring how books on *Publishers Weekly* annual bestseller lists changed from the 1990s through the 2020s.

## Project overview

The final project combines book metadata gathered from *Publishers Weekly* lists, Goodreads, and Wikipedia to explore three questions:

1. How does the distribution of bestselling genres change by decade?
2. Which authors appear most frequently across the collected lists?
3. Is book length associated with reader rating in the assembled dataset?

The interface includes decade controls for the genre view, a ranked author bar chart, and a scatterplot comparing page count with rating.

## Featured files

- [`FinalProject/Final_LitAnalysis.html`](FinalProject/Final_LitAnalysis.html): combined interactive analysis
- [`FinalProject/Yearly_Best_Sellers12.csv`](FinalProject/Yearly_Best_Sellers12.csv): cleaned project dataset
- [`FinalProject/Final: Single Charts/`](FinalProject/Final%3A%20Single%20Charts/): individual chart experiments

The `Homework1` through `Homework5` directories preserve earlier D3 exercises that led to the final project.

## Technology

- D3.js 7
- JavaScript
- HTML and CSS
- CSV data preparation
- SVG charts and event-driven interaction

## Run locally

Because the visualizations load CSV files in the browser, serve the repository through a local web server instead of opening the HTML file directly:

```bash
git clone https://github.com/jborri/D3_S24.git
cd D3_S24
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000/FinalProject/Final_LitAnalysis.html
```

## Data notes

The dataset was assembled for an academic visualization project from public bestseller lists and book metadata. Counts describe the collected records and should not be interpreted as a complete history of the publishing market. Goodreads ratings reflect platform users rather than a representative sample of all readers.

## Repository organization

```text
D3_S24/
├── FinalProject/       Final analysis, data, and chart variants
├── Homework1/          Introductory HTML and D3 work
├── Homework2/          Data binding and SVG charts
├── Homework3/          Additional chart practice
├── Homework4/          Additional chart practice
├── Homework5/          Additional chart practice
└── README.md
```

## Possible extensions

- normalize author and genre labels;
- add accessible tooltips and chart descriptions;
- make the combined page responsive;
- document the data-cleaning workflow; and
- deploy the final analysis as a standalone GitHub Pages project.
