# CUSTOMER-SEGMENTATION

**Customer Segmentation using RFM & K-Means Clustering with Excel Reports**

---

## Table of Contents

* [Overview](#overview)
* [Problem](#problem)
* [Solution](#solution)
* [Tech Stack](#tech-stack)
* [Project Structure](#project-structure)
* [Installation](#installation)
* [Usage](#usage)
* [Sample Output](#sample-output)
* [Contributing](#contributing)
* [License](#license)

---

## Overview

This project performs **customer segmentation using the RFM (Recency, Frequency, Monetary) model** and **K-Means clustering**. Customers are classified into **Regular, Lost, VIP, and Loyal** groups based on their purchase behavior.

It also generates **Excel reports** with each segment on a separate sheet and provides actionable insights for **marketing strategies, retention programs, and identifying high-value customers**.

---

## Problem

Businesses often treat all customers the same, resulting in **lost revenue opportunities, overstocking, and low retention**.

---

## Solution

* Calculate **RFM metrics** for each customer.
* Determine optimal number of clusters using the **Elbow Method**.
* Segment customers using **K-Means clustering**.
* Generate an **Excel report** with **4 sheets**, one for each segment.
* Visualize **cluster distributions** using charts and graphs.

---

## Tech Stack

* **Python**
* **Pandas** (data manipulation)
* **NumPy** (numerical computations)
* **Matplotlib & Seaborn** (visualizations)
* **Scikit-learn** (K-Means clustering, Elbow method)
* **Openpyxl** (Excel report generation)
* **Jupyter Notebook** for analysis

---

## Project Structure

```
CUSTOMER-SEGMENTATION/
│
├─ data/
│   └─ online_retail.csv        # Input dataset
│
├─ notebooks/
│   └─ 01_rfm_analysis.ipynb   # Notebook with RFM analysis and clustering
│   └─ RFM_Customer_Segments.xlsx  # Generated output report
│
├─ venv/                        # Python virtual environment
│   ├─ Include/
│   ├─ Lib/
│   ├─ Scripts/
│   └─ etc/
│
├─ README.md
```

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/<your-username>/CUSTOMER-SEGMENTATION.git
cd CUSTOMER-SEGMENTATION
```

2. Activate the virtual environment:

```bash
# Windows
venv\Scripts\activate

# Linux / Mac
source venv/bin/activate
```

3. Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl
```

---

## Usage

1. Place your customer CSV file in the `data/` folder.
2. Open the notebook `01_rfm_analysis.ipynb` in Jupyter or VS Code.
3. Run all cells to perform:

   * RFM analysis
   * K-Means clustering with the Elbow method
   * Segment labeling
   * Excel report generation
4. Output: **`RFM_Customer_Segments.xlsx`** in `notebooks/` folder with **4 sheets**.

---

## Sample Output

| Recency | Frequency | Monetary | Cluster | Segment           |
| ------- | --------- | -------- | ------- | ----------------- |
| 43.7    | 3.68      | 1359     | 0       | Regular_Customers |
| 248     | 1.55      | 480      | 1       | Lost_Customers    |
| 7.38    | 82.53     | 127338   | 2       | VIP_Whales        |
| 15.5    | 22.33     | 12709    | 3       | Loyal_Customers   |

**Excel file sheets:**

* `Regular_Customers`
* `Lost_Customers`
* `VIP_Whales`
* `Loyal_Customers`

**Visualizations:**

* Elbow Method plot to find optimal clusters
* Cluster distribution plots with Seaborn/Matplotlib

---

## Contributing

* Fork the repository
* Make your changes
* Submit a pull request

---

## License

Open-source project. Free to use and modify.

---

