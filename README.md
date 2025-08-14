# India CPI Inflation Case Study

## Overview

In India, the **Consumer Price Index (CPI)** is a key measure of inflation, representing a **fixed basket of goods and services** consumed by an average Indian household.
This basket is comprehensive, covering categories like:

* Food & Beverages
* Clothing & Apparel
* Housing
* Transportation
* Medical Care
* Electricity
* Education
* Recreation
  and more.

The CPI is calculated by **comparing market price levels** in a given period to a **base year**.
Each category has a weight based on its share of average consumer expenditure.
For this analysis, **equal weights** across categories are assumed.

---

## Dataset Details

* **Source:** CPI inflation index data (extracted from GOI website).
* **Data Points:** Monthly index values per category.
* **Missing Values:** Use suitable imputation techniques (e.g., moving averages).
* **CPI Nature:** An **index**, not a direct price measure — reflects average price changes over time.
* **Sub-Indexes:**

  * **CPI-U (Urban):** Urban consumer spending patterns.
  * **CPI-R (Rural):** Rural consumer spending patterns.
  * **General Index:** Overall inflation for all categories combined.

---

## Problem Statement

You are working as an **analyst** at the **National Statistical Office**.
You are tasked with identifying **key trends and insights** from CPI data, answering the following:

---

### **1. Contribution of Categories to CPI (Latest Month)**

* Group categories into **broader buckets** (e.g., *Meals, Beverages, Cereals → Food*).
* Calculate **percentage contribution** of each broader category to total CPI (sum to 100%).
* Identify **category with highest contribution**.

---

### **2. Year-on-Year CPI Trend (2017 onwards)**

* Plot **YoY growth rate** for CPI (Urban + Rural combined).
* Identify **year with highest inflation rate**.
* Provide **research-based reasons** for the peak year.

---

### **3. Food Inflation Analysis (Jun’22 – May’23)**

* Investigate **month-on-month changes** in the **broader Food category**.
* Identify **highest and lowest food inflation months**.
* Find **biggest individual category contributor** (within Food) to inflation over the period.

---

### **4. COVID-19 Impact on Inflation**

* Consider **March 2020** as pandemic onset.
* Compare **inflation trends before & after Mar’20**.
* Focus on **healthcare, food, and essential services** categories.
* Analyze effect of first lockdown.

---

### **5. Global Events Impact — Oil Prices (2021–2023)**

* Focus on **imported crude oil price fluctuations**.
* Analyze correlation between **oil prices** and **inflation rates** across categories.
* Identify category most **sensitive** to oil price changes (use correlation function).

---

## Additional Information

* **Percentage Change Formula:**

  * **Monthly Inflation Rate:**

    ```
    ((CPI_current - CPI_previous) / CPI_previous) × 100
    ```
  * **Annual Inflation Rate:**

    ```
    ((CPI_end - CPI_start) / CPI_start) × 100
    ```
  * Start month can be any; end month = 12 months later.
