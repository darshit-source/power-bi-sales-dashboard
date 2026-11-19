# Sales Insights Dashboard | Power BI

An interactive Power BI project for exploring sales performance across products, customers, geography, payment methods, and time. The report is built from two related tables and packaged with the source CSV files and a custom background image.

> **Portfolio project** · Power BI · Data modeling · Business intelligence

<!-- Add a screenshot of the finished report to the repository (for example, assets/dashboard-preview.png), then uncomment and update this line:
![Sales dashboard preview](assets/dashboard-preview.png)
-->

## Project overview

This project turns order-level and sales-detail data into a report that can support questions such as:

- How do sales and profit change over the year?
- Which product categories and sub-categories contribute most to sales and profit?
- How do results vary by state and city?
- Which payment methods are used most often?
- How do order volume, quantity, sales, and profit compare?

The supplied dataset covers **1 January–31 December 2018** and contains **500 order records** and **1,500 sales-detail records**. The totals below are calculated from `Details.csv`; the source does not specify a currency, so `Amount` is shown in the dataset's original units.

| Dataset measure | Value |
| --- | ---: |
| Sales amount | 437,771 |
| Profit | 36,963 |
| Quantity | 5,615 |
| Profit as a share of sales amount | 8.44% |

These figures describe the supplied data, not independently verified business results.

## Files

| File | Description |
| --- | --- |
| `Power Bi Sales DashBoard.pbix` | Power BI report file. Download and open with Power BI Desktop. |
| `Orders.csv` | Order date, customer name, state, and city. |
| `Details.csv` | Amount, profit, quantity, category, sub-category, and payment mode for each order line. |
| `dark-gradient.jpg` | Background image supplied with the project. |

## Data model

The two CSV files share the `Order ID` field, which can be used to relate order information to sales details in Power BI.

- **Orders**: 500 rows; includes order date and customer/location attributes.
- **Details**: 1,500 rows; includes sales and product/payment attributes.
- **Categories**: Clothing, Electronics, Furniture.
- **Payment methods**: COD, Credit Card, Debit Card, EMI, UPI.
- **Coverage**: 2018 calendar year; 19 distinct state labels in the order file.

## Tools and skills

- Microsoft Power BI Desktop
- Data modeling and table relationships
- KPI and measure design
- Time, product, payment, and geographic analysis
- Report layout and visual design

## Open the report

1. Download or clone this repository.
2. Open `Power Bi Sales DashBoard.pbix` in Microsoft Power BI Desktop.
3. If Power BI asks for data sources, point the queries to the included CSV files.
4. Refresh the report to load the data.

GitHub stores the `.pbix` file but does not render an interactive Power BI report in the repository page. Add a screenshot of the report above so visitors can preview it without downloading the file.

## Data notes

The CSV files include customer names and location information. If you publish this repository publicly, confirm that you have permission to share the data. Otherwise, remove the CSV files and replace them with anonymized or synthetic sample data, then update this README accordingly.

The CSV date values use the `DD-MM-YYYY` format. The amount field has no currency label in the source files; avoid assigning a currency symbol unless you have confirmed the intended currency.

## About

Created as a portfolio project to demonstrate a Power BI sales analysis workflow. Replace this line with your name and add links to your portfolio or LinkedIn profile if you want to make the repository easier to associate with your resume.

