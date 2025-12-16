# Grocery Sales ETL Pipeline with PySpark

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![PySpark](https://img.shields.io/badge/PySpark-3.0+-red.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

A robust and scalable ETL pipeline for processing grocery sales data using PySpark. This project demonstrates how to handle real-world data challenges including data cleaning, validation, and transformation at scale.

## 🚀 Features

- **Multi-source Data Integration**: Combine data from online, mobile, and in-store sales channels
- **Data Quality Checks**: Built-in validation and error handling
- **Scalable Processing**: Leverages PySpark for distributed computing
- **Comprehensive Logging**: Detailed logging for monitoring and debugging
- **Production-ready**: Follows best practices for ETL pipeline development

## 📦 Project Structure
PYSPARK_ETL_GROCERY_PIPELINE/ ├── DATA/ # Data directories │ ├── RAW/ # Raw input files │ │ ├── online_orders.csv │ │ ├── mobile_orders.csv │ │ └── store_orders.csv │ └── PROCESSED/ # Processed output │ └── orders/ # Final output directory ├── src/ # Source code │ ├── init.py │ └── etl_pipeline.py # Core ETL logic ├── main.py # Entry point ├── requirements.txt # Dependencies └── logs/ # Log files └── etl_run_*.log # Log files with timestamps


## 🛠️ Setup

### Prerequisites

- Python 3.8+
- Java 8 or later (required for PySpark)
- pip (Python package manager)

## 🛠️ Setup
 
### Prerequisites
 
- Python 3.8+
- Java 8 or later (required for PySpark)
- pip (Python package manager)

### Installation

1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/grocery-sales-etl.git](https://github.com/yourusername/grocery-sales-etl.git)
   cd grocery-sales-etl

   Create and activate a virtual environment (recommended):
bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies:
bash
pip install -r requirements.txt
🚦 Running the Pipeline
Run the ETL pipeline:
bash
spark-submit main.py
Check the logs in the logs/ directory for processing details.
🔍 Data Processing
Input Data Format
The pipeline expects CSV files in the DATA/RAW/ directory with the following columns:

order_id: Unique order identifier
customer_id: Customer identifier
product_name: Name of the product
price: Price of the product
quantity: Quantity ordered
order_date: Date of the order
region: Sales region
Processing Steps
Extraction: Reads data from multiple CSV sources
Transformation:
Standardizes customer IDs
Cleans and validates prices
Handles date formats
Removes test data and duplicates
Adds calculated fields
Loading: Saves processed data to DATA/PROCESSED/orders/
📊 Output
The processed data includes:

Cleaned and standardized fields
Additional calculated fields (total amount, processing date, etc.)
Quality flags for data validation
📝 Logging
The pipeline generates detailed logs in the logs/ directory, including:

Processing statistics
Data quality issues
Error messages
Performance metrics
🤝 Contributing
Contributions are welcome! Please follow these steps:

Fork the repository
Create a feature branch
Commit your changes
Push to the branch
Submit a pull request


