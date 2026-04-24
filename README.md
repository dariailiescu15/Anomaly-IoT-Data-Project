# IoT Telemetry Monitoring System

> End-to-end pipeline for anomaly detection in CPU utilization data  
> SQL Storage · Python Analysis · Power BI Reporting

---

## Table of Contents

1. [Overview](#overview)
2. [Dataset](#dataset)
3. [Project Structure](#project-structure)
4. [Pipeline Architecture](#pipeline-architecture)
5. [Technologies](#technologies)
6. [License](#license)

---

## Overview

A complete **IoT data monitoring and analysis system** designed to detect anomalies in CPU utilization on an EC2 instance. The project integrates three major components — SQL storage, Python analysis, and Power BI visualization — into a cohesive end-to-end pipeline suitable for both educational and real-world system monitoring scenarios.

---

## Dataset

> **Note:** All in-code comments are written in **Romanian**.

The project uses real-world telemetry data from the **NAB (Numenta Anomaly Benchmark)** dataset.

| Property | Details |
|----------|---------|
| File | `ec2_cpu_utilization_5f5533.csv` |
| Source | Real AWS telemetry data |
| Columns | `timestamp`, `value` (CPU utilization %) |
| Purpose | Identifying unusual behaviors, potential incidents, and significant performance variations |

---

## Project Structure

```
├── data/
│   └── ec2_cpu_utilization_5f5533.csv   # Raw NAB dataset
├── sql/
│   └── schema.sql                        # Database schema and import scripts
├── notebooks/
│   └── analysis.ipynb                    # Jupyter Notebook — full analysis pipeline
└── powerbi/
    └── dashboard.pbix                    # Power BI report file
```

---

## Pipeline Architecture

```
IoT Data (CSV)  →  SQL Storage  →  Python Analysis  →  Power BI Dashboard
```

### 1. Storage — SQL Backend

- Import and organization of raw telemetry data into a relational database.
- Schema design optimized for efficient querying and downstream analysis.

### 2. Processing & Analysis — Python (Jupyter Notebook)

- **Data Cleaning & Preprocessing** — handling missing values, type casting, timestamp normalization.
- **Exploratory Data Analysis** — trends, distributions, and variance over time.
- **Anomaly Detection** — custom logic to flag abnormal CPU utilization patterns.
- **Visualizations** — charts highlighting detected anomalies in context.

The entire workflow is implemented in a Jupyter Notebook for full **transparency and reproducibility**.

### 3. Visualization & Reporting — Power BI

- Interactive dashboard presenting the full CPU utilization timeline.
- Clear visual highlighting of detected anomalies.
- Intuitive layout designed for rapid interpretation by non-technical stakeholders.

---

## Technologies

| Layer | Technology |
|-------|------------|
| Data Storage | SQL (relational database) |
| Analysis & Detection | Python 3.x — Pandas, NumPy, Matplotlib / Seaborn |
| Notebook Environment | Jupyter Notebook |
| Visualization | Power BI Desktop |
| Data Source | NAB Benchmark — AWS EC2 real telemetry |

---

## License

© 2026 — Project created by **Daria-Gabriela Iliescu**.

All rights reserved. Use, distribution, or modification of this code or associated materials is permitted only with **proper attribution to the author**.
