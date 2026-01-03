# Airbnb Price Optimization & Market Analysis

**Main Notebook:** `AirBnB.ipynb`  
**Course:** 2025-Fall-CS 6220
**Team:** Daksh Patel, Zi Wang  

---

## 🧾 Overview

This project analyzes Airbnb listing markets and builds predictive models to support:
- **Dynamic pricing insights**
- **Market segmentation**
- **Price prediction using regression models**
- **Cluster-based strategy recommendations**

All notebook steps are **reproducible end-to-end**.

---

## 📁 Data Sources
Inside Airbnb (https://insideairbnb.com/explore/)

Accepted formats:
- `.csv`
- `.csv.gz` (GZIP compressed)
- `.zip` (must contain a CSV file)

After upload, the notebook automatically:
✓ Decompresses `.gz` or `.zip` files into `.csv`  
✓ Loads files into `pandas` dataframes (`boston_df`, `nyc_df`)  
✓ Assigns a `city` label to each listing  
✓ Merges both into a single dataset for unified modeling  

---

## 📊 Data Loaded in Current Version

| City | Rows | Columns (before merge) |
|------|------:|------:|
| Boston | 4,419 | 80 |
| New York City | 36,111 | 80 |
| **Combined Dataset** | **40,530** | **81** (includes `city` tag) |

---

## 🔁 Analysis Pipeline

The notebook executes the sections below sequentially:

1. **Data Loading**
2. **Data Cleaning + Preprocessing**
3. **EDA + Visualizations**
4. **Feature Engineering**
5. **Regression Price Models**
6. **Model Evaluation**
7. **Clustering Segmentation**

---

## ⚙️ Setup & Running (Local Computer)

```bash
git clone https://github.com/2025-F-CS6220/project-airbnb.git
cd project-airbnb

python -m venv venv
source venv/bin/activate      # macOS / Linux
# OR
venv\Scripts\activate         # Windows

pip install -r requirements.txt
jupyter notebook
# Open AirBnB.ipynb and run all cells from top → bottom
```

---

## 🌐 Setup & Running (Google Colab)

1. Open **Colab**
2. Click → `File → Open Notebook → GitHub`
3. Paste repo link → select `AirBnB.ipynb`
4. Click → `Runtime → Run all`
5. Upload data files when notebook prompts appear

_The project is Colab-compatible by design._

---

## 📦 Dependencies

Listed in `requirements.txt`:

```
pandas>=1.3.0
numpy>=1.20.0
matplotlib>=3.4.0
seaborn>=0.11.0
scikit-learn>=1.0.0
```

Install them using:

```bash
pip install -r requirements.txt
```

---

## ✅ Expected Outputs

After execution, you will see:

- Library import check + version printouts
- Analysis timestamp
- Data loading validation
- Missing value summary
- Engineered amenity group stats
- Regression model scores (MAE, RMSE, R², MAPE)
- Best model selected by validation R²
- Clustering segmentation summary
- Graphs from EDA & clustering stages

---
