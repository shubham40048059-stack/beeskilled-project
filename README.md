# Beeskilled Sales Analysis

This project explores a sales dataset and prepares cleaned data and summary tables for analysis in Power BI. The notebook also includes a linear-regression example for estimating sales.

## Project files

| File | Description |
| --- | --- |
| `eda _project.ipynb` | Exploratory analysis, grouped summaries, visualizations, and a sales-regression example |
| `Sample data (1).xlsx - Sheet1.csv` | Source dataset exported as CSV |
| `PowerBI_Cleaned_Data.csv` | Cleaned dataset exported by the notebook |
| `Sales_by_Country.csv` | Sales totals grouped by country |
| `Sales_by_Product.csv` | Sales totals grouped by product |
| `Sales_by_Segment.csv` | Sales totals grouped by segment |
| `Sales_by_Year.csv` | Sales totals grouped by year |
| `Profit_by_Country.csv` | Profit totals grouped by country |
| `Profit_by_Product.csv` | Profit totals grouped by product |
| `requirements.txt` | Python packages used by the notebook |

## Getting started

1. Clone this repository and open the project directory.
2. Install Python 3 and Jupyter Notebook or JupyterLab.
3. Install the project dependencies:

   ```powershell
   python -m pip install -r requirements.txt
   ```

4. Open `eda _project.ipynb` and run it from the project directory so its relative CSV paths resolve.

The notebook reads `Sample data (1).xlsx - Sheet1.csv`, trims whitespace from column names, explores the data, generates visualizations and summary tables, and writes the cleaned dataset and summary CSV files listed above.

## Dataset fields

The source data includes sales segment, country, product, discount band, units sold, manufacturing and sale prices, gross sales, discounts, sales, cost of goods sold (COGS), profit, date, month, and year. The source CSV has whitespace before the `Sales` column name; the notebook strips column-name whitespace before analysis.

## Modeling note

The notebook's regression example predicts `Sales` using `Units Sold`, `Sale Price`, `Gross Sales`, `Discounts`, and `COGS`. Since `Sales` is closely determined by some of those accounting fields, treat this as an instructional example rather than evidence of independent predictive performance.
