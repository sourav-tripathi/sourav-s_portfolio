# Retail Sales Data Analysis

![GitHub last commit](https://img.shields.io/github/last-commit/sourav-tripathi/sourav-s_portfloio)
![GitHub issues](https://img.shields.io/github/issues/sourav-tripathi/sourav-s_portfloio)
![GitHub](https://img.shields.io/github/license/sourav-tripathi/sourav-s_portfloio)

## Project Overview

This project examines and analyzes retail store sales data to uncover valuable insights into customer purchasing behavior, product performance, and broader business trends. The dataset includes details on various transactions, such as item categories, pricing, quantities sold, payment methods, and applied discounts. Through data cleaning, data analysis (EDA), and visualizing key trends, we seek to identify revenue driving factors and offer practical recommendations for enhancing business performance.

## Table of Contents

- [Data Description](#data-description)
- [Methodology](#methodology)
  - [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
  - [Exploratory Data Analysis](#exploratory-data-analysis-eda)
- [Key Findings](#key-findings)
  - [Revenue Contribution by Category](#revenue-contribution-by-category)
  - [Payment Method Preferences](#payment-method-preferences)
  - [Category-wise Spending Trends](#category-wise-spending-trends)
  - [Monthly Sales Trends](#monthly-sales-trends)
  - [Relationship Between Quantity and Total Spend](#relationship-between-quantity-and-total-spend)
- [Setup and Installation](#setup-and-installation)
- [License](#license)

## Data Description

The dataset contains detailed retail transaction records with the following attributes:
* Transaction information (dates, IDs)
* Product details (item category, price per unit)
* Purchase information (quantity, total spent)
* Payment methods
* Discount applications

## Methodology

### Data Cleaning and Preprocessing

1. **Handling Missing Values**
   * Identified and addressed missing values in key columns including "Item," "Price Per Unit," "Quantity," and "Total Spent"
   * Set "Discount Applied" to "False" for records with missing discount information

2. **Data Type Conversion**
   * Converted "Transaction Date" to datetime format to enable time-series analysis
   * Ensured numeric fields had appropriate data types for accurate calculations

### Exploratory Data Analysis (EDA)

The analysis explored various dimensions of the retail data:
* Distribution of prices across product categories
* Purchase quantity patterns
* Revenue distribution by category
* Payment method preferences
* Seasonal sales trends

## Key Findings

### Revenue Contribution by Category

The top five revenue-generating categories are:
1. **Butchers**: $218,153
2. **Electric Household Essentials**: $215,297
3. **Beverages**: Significant contribution
4. **Furniture**: Strong sales figures
5. **Food**: Strong sales figures

### Payment Method Preferences

Analysis revealed that most customers prefer Credit Cards and Cash for purchases, while Online Payment methods also showed significant popularity.

### Category-wise Spending Trends

* **Furniture** and **Butchers** categories showed the highest median spending
* Several categories demonstrated high variability in pricing, indicating diverse product ranges with both premium and budget options
* Outliers were identified and addressed to improve analytical clarity

### Monthly Sales Trends

Time-series analysis identified specific months with significant sales spikes, potentially attributable to:
* Seasonal purchasing patterns
* Promotional campaigns
* Shifts in consumer behavior

### Relationship Between Quantity and Total Spend

The analysis revealed several interesting purchase patterns:
* High-value, low-quantity transactions (premium item purchases)
* Moderate-spend bulk purchases (volume discount seeking)
* Diverse purchasing behaviors across customer segments

## Setup and Installation

```bash
# Clone the repository
git clone https://github.com/sourav-tripathi/sourav-s_portfloio.git

# Navigate to the project directory
cd sourav-s_portfloio

# Create and activate a virtual environment (recommended)
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate

# Install required packages
pip install -r requirements.txt
```

## Usage

```bash
# Run the main analysis script
python src/analysis.py

# Or explore the Jupyter notebook
jupyter notebook notebooks/retai_sales_analysis.ipynb
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- Data sourced from retail operations records
- Analysis conducted as part of data science portfolio development

## Contact

For questions or feedback, please [open an issue](https://github.com/sourav-tripathi/sourav-s_portfloio/issues) on this repository.