# Zomato Global Dining Trends Analytics Pipeline

An end-to-end data analytics pipeline that extracts, processes, and visualizes global restaurant data to uncover international culinary market trends. This system couples a programmatic Python data engine with an interactive, brand-aligned executive Power BI reporting layer.

<img width="1172" height="662" alt="image" src="https://github.com/user-attachments/assets/03bd78f8-8768-44a4-983e-2a0967c6a684" />


## 🚀 Project Overview
The core objective of this project was to take a raw, multi-format global restaurant footprint and convert it into a clean, actionable data core. By bypassing manual spreadsheets and handling character encoding and structural missingness anomalies programmatically in Python, the final dashboard remains optimized, accurate, and completely scannable for corporate review.

## 🛠️ Technical Architecture & Tech Stack
- **Data Engineering & Analysis:** Python, Pandas, Matplotlib, Seaborn
- **Business Intelligence Front-End:** Power BI Desktop
- **Environment:** Jupyter Notebook

---

## 📈 Pipeline Workflow

### 1. Extraction & Relational Data Merging
* **Encoding Optimization:** Handled initial file IO character exceptions by applying targeted `latin-1` codecs to preserve international transaction logs.
* **Automated Extraction:** Implemented native `zipfile` hooks to extract uncompressed archival raw schemas at runtime.
* **Relational Left Joins:** Merged core restaurant transaction rows with an external dimensional Country-Code Excel workbook using key dependencies via `pd.merge()`.

### 2. Programmatic Data Cleaning & Feature Engineering
* **Data Profiling:** Created dynamic list comprehensions to auto-scan field arrays and compute exact missingness metrics across parameters.
* **Structural Filtering:** Evaluated zero-rating data boundaries (`Rating color == 'White'`) to isolate regional customer feedback blind spots.
* **Multi-Conditional Matrix Grouping:** Engineered target aggregation frames using `groupby().size().reset_index()` logic to cross-examine global currency distributions, market saturation thresholds, and regional online delivery metrics.

### 3. Visual Layout Modeling (Power BI)
* **Data Core Commitment:** Output the finalized staging layer using `.to_csv(encoding='utf-8-sig')` to enforce complete string character safety inside the BI front-end.
* **UI/UX Containerization:** Built an interactive operational cockpit leveraging modern "New Card" structural blocks, curved visual border profiles (12px radius), and custom drop-shadow rendering for flat layout elevation.
* **Conditional Data Tracking:** Set up functional color-scale gradients (Zomato Crimson to Success Green) to dynamically track ratings matrices instantly across interactive data tables and geographic bubble maps.

---

## 💡 Key Analytical Insights
* **Global Footprint:** Captured operational profiles across **16 countries** containing **1,831+ distinct cuisine types** and **9.5K+ total restaurants**.
* **Regional Dominance:** Isolated volume clusters across major municipalities, tracking New Delhi's high-density 5.5K threshold compared against average quality ratings.
* **Delivery Metrics:** Structured exact breakdown matrices tracking delivery systems, identifying core volume trends across primary international clusters like India and the UAE.

---

