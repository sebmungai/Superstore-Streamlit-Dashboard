# Superstore Sales Dashboard

An interactive sales analytics dashboard built with **Python, Streamlit, Pandas, and Plotly** to explore retail sales performance, profitability, and regional trends.

The dashboard transforms raw Superstore sales data into actionable business insights through interactive filters, KPI metrics, and visualizations.

## Project Overview

Retail businesses generate large amounts of sales data, but raw datasets can make it difficult to identify trends, evaluate profitability, and compare performance across product categories and regions.

This project addresses that challenge by providing an interactive dashboard where users can filter sales data and explore key business performance indicators.

## Dashboard Features

### 1. Key Performance Indicators (KPIs)

The dashboard provides an overview of business performance through:

- **Total Sales:** Total revenue generated from orders.
- **Total Profit:** Overall profit from sales.
- **Quantity Sold:** Total units sold.
- **Profit Margin:** Profit expressed as a percentage of sales.

### 2. Interactive Filters

Users can filter the dashboard using sidebar controls:

- Order date range
- Product category
- Sales region
- Customer segment

The charts and KPI metrics update according to the selected filters.

### 3. Data Visualizations

The dashboard contains four main visualizations arranged in a two-column layout:

- **Monthly Sales Trend:** Tracks sales performance over time to identify growth patterns and fluctuations.
- **Sales by Category:** Compares revenue across product categories.
- **Profit by Sub-Category:** Identifies product sub-categories contributing the most or least profit.
- **Sales Distribution by Region:** Compares sales performance across geographical regions.

The charts are interactive and provide additional details when users hover over data points.

### 4. Data Preparation

The application uses Pandas to prepare the dataset for analysis, including:

- Converting order dates into datetime format.
- Cleaning and converting numerical columns.
- Handling invalid date and numerical values.
- Grouping sales data for monthly and categorical analysis.
- Applying filters before calculating metrics and rendering charts.

## Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Streamlit | Interactive dashboard and web application |
| Pandas | Data cleaning, transformation, and analysis |
| Plotly Express | Interactive data visualizations |

## Project Structure

```text
superstore-sales-dashboard/
│
├── app.py
├── Superstore.csv
├── requirements.txt
└── README.md
```

- `app.py` — Contains the Streamlit application and dashboard logic.
- `Superstore.csv` — Dataset used for the analysis.
- `requirements.txt` — Lists the Python dependencies.
- `README.md` — Project documentation.

## Installation and Setup

### Prerequisites

Ensure that Python 3.9 or later is installed on your computer.

### Step 1: Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd superstore-sales-dashboard
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your actual repository URL.

### Step 2: Create a virtual environment (recommended)

```bash
python -m venv venv
```

Activate the environment.

**Windows:**

```bash
venv\Scripts\activate
```

**macOS/Linux:**

```bash
source venv/bin/activate
```

### Step 3: Install dependencies

```bash
pip install -r requirements.txt
```

If you do not have a `requirements.txt` file yet, create one containing:

```text
streamlit
pandas
plotly
```

### Step 4: Add the dataset

Place `Superstore.csv` in the project root directory, alongside `app.py`.

The application reads the CSV using Latin-1 encoding.

### Step 5: Run the application

```bash
streamlit run app.py
```

Open the local URL displayed in your terminal, usually:

`http://localhost:8501`

## Business Questions Explored

This dashboard helps users investigate questions such as:

1. How do monthly sales change over time?
2. Which product categories generate the highest revenue?
3. Which sub-categories contribute the most to profitability?
4. How does sales performance differ across regions?
5. How do customer segments and date ranges affect overall performance?
6. What happens to key business metrics when different filters are applied?

## Skills Demonstrated

This project demonstrates practical skills in:

- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- Business KPI calculation
- Time-series analysis
- Data aggregation and grouping
- Interactive dashboard development
- Data visualization using Plotly
- Building Python applications with Streamlit

## Future Improvements

Potential extensions include:

- Adding sales and profit comparisons against previous periods.
- Introducing monthly growth and year-over-year performance metrics.
- Identifying loss-making products and categories.
- Adding downloadable filtered reports.
- Deploying the dashboard online for public access.
- Integrating a database to support larger datasets.

## Conclusion

The Superstore Sales Dashboard demonstrates how Python-based analytics can turn raw retail data into an interactive business intelligence tool.

By combining data preparation, KPI reporting, and interactive visualizations, the project provides a foundation for exploring business performance and making data-informed decisions.

**Author:** Sebastian Mungai  
**Organization:** KeDataLab  
**Focus:** Data Analytics | Python | Business Intelligence | Dashboard Development
