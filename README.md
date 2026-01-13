# Autonomous Data Quality Analyzer

An end-to-end **Autonomous Data Quality Analyzer** that automatically inspects datasets, detects data quality issues, recommends fixes, and (optionally) applies them — producing clean datasets and detailed reports with minimal human intervention.

---

## Project Overview

In real-world data pipelines, poor data quality leads to unreliable analysis and weak ML models. This project simulates an **industry-grade data quality system** that:

* Profiles datasets automatically
* Detects common data quality issues
* Suggests intelligent fixes
* Applies fixes in autonomous mode
* Generates visual and downloadable reports

---

## Key Features

*  Automated data ingestion (CSV)
*  Dataset profiling & statistics
*  Detection of:

  * Missing values
  * Duplicate records
  * Outliers
  * Schema & type inconsistencies
*  Rule-based recommendation engine
*  Optional auto-fix pipeline
*  Data quality scoring (0–100)
*  HTML / PDF report generation
*  Streamlit-based UI (optional)

---

## 🗂️ Project Structure

```
autonomous-data-quality-analyzer/
├── data/
│   ├── raw/              # Raw input datasets
│   ├── processed/        # Cleaned datasets
│   └── reports_input/
│
├── outputs/
│   ├── reports/          # HTML / PDF reports
│   ├── logs/             # Pipeline logs
│   └── metrics/          # Quality scores & summaries
│
├── src/
│   ├── ingestion/        # Data loading logic
│   ├── profiling/        # Dataset profiling
│   ├── checks/           # Data quality checks
│   ├── recommendations/ # Fix suggestions
│   ├── fixes/            # Auto-fix logic
│   └── reporting/        # Report generation
│
├── ui/                   # Streamlit UI
├── config/               # Configurations & thresholds
├── tests/                # Unit tests
│
├── run.py                # Entry point
├── requirements.txt
└── README.md
```

---

##  Pipeline Flow

```
Ingestion → Profiling → Quality Checks → Recommendations → Auto-Fix → Reporting
```

Each stage is modular and independently extensible.

---

##  How to Run

### 1️⃣ Clone the Repository

```bash
git clone <repo-url>
cd autonomous-data-quality-analyzer
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Add Dataset

Place your CSV file inside:

```
data/raw/
```

### 4️⃣ Run the Pipeline

```bash
python run.py
```

---

## 📤 Outputs Generated

*  Cleaned dataset (`data/processed/`)
*  Quality metrics (`outputs/metrics/`)
*  HTML / PDF reports (`outputs/reports/`)
*  Logs (`outputs/logs/`)

---

##  Example Data Quality Issues Detected

| Issue Type     | Example               |
| -------------- | --------------------- |
| Missing Values | 8.5% missing in `age` |
| Duplicates     | 75 duplicate rows     |
| Outliers       | Extreme salary values |
| Schema Errors  | Mixed data types      |

---

##  Quality Score

A composite score (0–100) is generated based on:

* Missing value severity
* Duplicate ratio
* Outlier proportion
* Schema violations

---

## 👤 Author

**Aditya Sharma**
Computer Science & Engineering
Aspiring Data Scientist / ML Engineer

---

