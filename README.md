# RFM-Customer-Segmentation
RFM Customer Segmentation &amp; Excel Report Generator for business insights

Table of Contents

Overview

Problem

Solution

Tech Stack

Features

Installation

Usage

Sample Output

Folder Structure

Contributing

License

Overview

This project performs customer segmentation using the RFM (Recency, Frequency, Monetary) model. It classifies customers into Regular, Lost, VIP, and Loyal segments based on their purchase behavior.

It generates Excel reports with each segment on a separate sheet, providing actionable insights for businesses to target high-value customers, improve retention, and optimize marketing strategies.

Problem

Many businesses struggle with overstocking, low retention, and ineffective marketing because they treat all customers the same.

Solution

Analyze customer purchase behavior using RFM metrics.

Automatically classify customers into 4 segments.

Generate Excel reports with separate sheets per segment.

Provides actionable insights for marketing, loyalty programs, and business strategy.

Tech Stack

Python

Pandas (data manipulation)

Openpyxl (Excel report generation)

RFM Analysis

K-Means / Clustering (if clustering added in future)

Features

Accepts any customer dataset with Recency, Frequency, Monetary, and Cluster columns.

Adds segment names automatically.

Creates Excel file with 4 sheets, each representing a customer segment.

Easy to integrate into business workflows.

Installation

Clone the repository:

git clone https://github.com/<your-username>/RFM-Customer-Segmentation.git
cd RFM-Customer-Segmentation


Create a virtual environment (optional but recommended):

python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows


Install dependencies:

pip install -r requirements.txt


Make sure openpyxl is installed:

pip install openpyxl

Usage

Place your customer CSV file in the project folder.

Update file_path in the script or use input prompt:

file_path = input("Enter your CSV file path: ")
generate_rfm_report(file_path)


Run the script:

python rfm_segmentation.py


Check RFM_Customer_Segments.xlsx for segmented sheets.

Sample Output
Recency	Frequency	Monetary	Cluster	Segment
43.7	3.68	1359	0	Regular_Customers
248	1.55	480	1	Lost_Customers
7.38	82.53	127338	2	VIP_Whales
15.5	22.33	12709	3	Loyal_Customers

Excel file will have 4 sheets:

Regular_Customers

Lost_Customers

VIP_Whales

Loyal_Customers

Folder Structure
RFM-Customer-Segmentation/
│
├─ rfm_segmentation.py        # Main script
├─ sample_data.csv            # Example dataset
├─ RFM_Customer_Segments.xlsx # Output file
├─ requirements.txt           # Dependencies
└─ README.md                  # This file

Contributing

Fork the repository

Make your changes

Submit a pull request

License

This project is open-source. Feel free to use and modify.
