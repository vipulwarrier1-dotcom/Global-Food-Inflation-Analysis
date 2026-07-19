# Global Food Prices, Inflation & Nutrition: An Exploratory Data Analysis

An exploratory data analysis connecting global food price shocks (COVID-19, the Russia–Ukraine war) to
country-level inflation, undernourishment, and hunger outcomes across 30 countries, 2015–2024.

## Project Overview

Rising food prices don't hit every country the same way. This project explores how food price shocks,
inflation, and malnutrition indicators (stunting, wasting, undernourishment, Global Hunger Index) are
connected — and how global commodity/food-price shocks line up with spikes in hunger, and why some
countries prove far more resilient than others.

**Key questions explored:**
- How has the global FAO Food Price Index moved since 2015, and does it align with known crisis events?
- How do food inflation and price shocks relate to nutrition outcomes like stunting and undernourishment?
- Which countries are most vulnerable and which are most resilient when a global shock hits?

## Repository Structure

```
├── food_price_nutrition_analysis.ipynb   # Main analysis notebook
├── data/                                  # Source datasets (CSV)
│   ├── food_price_vs_nutrition.csv        # Main panel: country-year inflation & nutrition indicators
│   ├── fao_food_price_index.csv           # Global monthly/annual FAO Food Price Index
│   ├── food_crises_events.csv             # Documented global/regional food crisis events
│   ├── global_hunger_index.csv            # GHI scores by country/year
│   └── regional_summary.csv               # Pre-aggregated regional averages
├── Food_Price_Nutrition_Analysis_Report.docx  # Summary report (Word)
├── requirements.txt                       # Python dependencies
├── CITATION.cff                           # Machine-readable citation metadata
├── LICENSE                                # Project license
└── README.md                              # You are here
```

## Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/vipulwarrier1-dotcom/Global-Food-Inflation-Analysis.git
   cd Global-Food-Inflation-Analysis
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Launch the notebook**
   ```bash
   jupyter notebook food_price_nutrition_analysis.ipynb
   ```

   > The notebook loads data using a relative path (`DATA_DIR = "./"`), so as long as the `./`
   > required files stays next to the notebook, it will run correctly on any machine.

## Analysis Workflow

The notebook follows the standard data analysis pipeline:

1. **Data Loading & Inspection** — shape, types, and summary statistics
2. **Data Cleaning** — missing value, duplicate, and type checks
3. **Exploratory Data Analysis** — group comparisons by income, region, and correlation analysis
4. **Data Visualization** — 9 charts covering trends, relationships, and country rankings
5. **Crisis Impact Analysis** — before/during/after comparisons for all countries simultaneously showing the impact of Food Import Dependency and GDP per capita
6. **Insights & Conclusions** — key findings, limitations, and suggested next steps

## Key Findings

- Global food prices spiked sharply from 2020–2022, coinciding with COVID-19 and the Russia–Ukraine war.
- GDP per capita is the strongest single predictor of nutrition outcomes in this dataset.
- The 2022–2023 global shock hit countries very unevenly — Turkey's food inflation rose 60+ percentage
  points, while other countries barely moved.
- Global Hunger Index changes did not move in lockstep with price shocks, reflecting the GHI's composite,
  lagged construction and the role of domestic resilience factors (governance, social protection, conflict).

See the full [analysis report](Food_Price_Nutrition_Analysis_Report.docx) or the notebook itself for
details, charts, and interpretation.

## Data Sources

This project uses illustrative/curated datasets assembled for analysis practice. See [CITATION.cff](CITATION.cff)
for citation details, and consult original sources (FAO, Global Hunger Index / Welthungerhilfe & Concern
Worldwide, World Bank) for authoritative, up-to-date figures.

## License

This project is licensed under the terms in [LICENSE](LICENSE).

## Contributing

This is a personal learning/portfolio project, but suggestions and issues are welcome — feel free to open
an issue or pull request.
