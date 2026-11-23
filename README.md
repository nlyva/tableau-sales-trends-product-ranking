# tableau-sales-trends-product-ranking
Tableau analysis of monthly sales trends and the top five products by profit in each region.
# Monthly Sales Trends & Regional Product Profitability

For a Business Analytics assignment at ADA University, I used Tableau
to analyze monthly sales and rank products by profit within each region.

## Tableau Public Visualizations

| Analysis | What it shows | Tableau calculations |
| --- | --- | --- |
| [Monthly Sales for a Selected Year](https://public.tableau.com/app/profile/nazrin.aliyeva/viz/hw5_1_17625371574110/question1) | Shows monthly sales for the selected year and highlights its first and last months. | `LOOKUP(SUM([Sales]), FIRST())` retrieves the first month's sales. `LOOKUP(SUM([Sales]), LAST())` retrieves the last month's sales. |
| [First and Last Month Sales by Year](https://public.tableau.com/app/profile/nazrin.aliyeva/viz/hw5_2_17625371978040/question2) | Isolates sales for the first or last month of each year. | `INDEX()` numbers the months in each yearly pane. A Boolean filter selects `INDEX() = 1` or `INDEX() = 12`. |
| [Top Five Products by Profit in Each Region](https://public.tableau.com/app/profile/nazrin.aliyeva/viz/hw5_3/question3) | Identifies the five most profitable products within each region. | `RANK(SUM([Profit]))` ranks products by total profit within each region. |

## Data Source

[Orders-ReviewMidterm Excel dataset](https://github.com/ogut77/BA/blob/main/Orders-ReviewMidterm.xls)
