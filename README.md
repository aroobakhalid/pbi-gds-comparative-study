# Comparative Analysis of Data Visualization Tools and Techniques: A Case Study of Power BI and Google Data Studio

## Paper Information
- **Journal:** VFAST Transactions on Software Engineering (VTSE)
- **Authors:** Arooba Khalid, Rimsha Anam, Fatima Tariq, Muhammad Junaid Anjum

## Overview
This repository contains the datasets, transformation configurations, dashboard materials, evaluation records, and supporting documentation for the comparative study of Microsoft Power BI (PBI) and Google Data Studio (GDS) in a retail analytics context.

## Repository Structure

| Folder | Contents |
|--------|----------|
| `data/raw/` | Original datasets from Kaggle + SHA-256 hashes |
| `data/cleaned/` | Transformed datasets used in dashboards |
| `excel/` | Excel files used for GDS preprocessing |
| `power_query/` | Exported Power Query M code (PBI) |
| `dax/` | DAX measures used in PBI dashboards |
| `calculated_fields/` | GDS calculated fields and gauge configs |
| `screenshots/` | Dashboard screenshots (PowerBI and LookerStudio subfolders) |
| `evaluation/` | Evaluation scoring workbook |
| `observed_interaction_effort/` | Task-level interaction comparison |
| `dashboard_component_specification/` | Component encoding comparison |
| `spss/` | ICC analysis files |
| `analysis/` | Distributional analysis notebook link |

## Datasets

| Dataset | Source | Records | Fields | URL |
|---------|--------|---------|--------|-----|
| Amazon Sales Dataset | Kaggle (user: aliiihussain) | 50,000 | 13 | [Link](https://www.kaggle.com/datasets/aliiihussain/amazon-sales-dataset) |
| Walmart Product Sales Dataset | Kaggle (user: shriyasingh900) | 1,000 | 17 | [Link](https://www.kaggle.com/datasets/shriyasingh900/walmart-product-sales-dataset) |

File integrity can be verified using the SHA-256 hashes provided in `data/raw/SHA256_HASHES.txt`.

## Platform Configurations

| Parameter | Power BI | Google Data Studio |
|-----------|----------|-------------------|
| Version | Desktop 2.154.1260.0 (64-bit) | Web-based application |
| License | Free (Desktop) | Free |
| Preprocessing | Power Query (native) | Microsoft Excel (external) |
| Calculated Fields | DAX | GDS Calculated Fields |

## Evaluation Framework

Five independent evaluators assessed all four dashboard implementations across ten dimensions using dimension-specific scoring anchors. Inter-rater reliability: ICC(2,5) = 0.940 (95% CI: 0.886-0.973, p < .001).

| Evaluation Dimension | PBI Mean | GDS Mean |
|---------------------|----------|----------|
| Dataset Handling | 3.4 | 2.6 |
| ETL Capability | 4.6 | 1.2 |
| Observed Interaction Effort | 3.2 | 4.6 |
| KPI and Target Monitoring | 4.8 | 2.8 |
| Filter and Slicer | 4.6 | 3.6 |
| Chart Quality and Labeling | 4.2 | 2.4 |
| Geographic Visualization | 3.0 | 4.6 |
| Dashboard Consistency | 4.8 | 3.4 |
| Analytical Capability | 4.6 | 2.6 |
| No-Code Suitability | 3.0 | 4.6 |
| **Total** | **40.2** | **32.4** |

## Distributional Analysis

The distributional analysis (CV, Fisher's skewness, normalized Shannon entropy) was computed in Python. The notebook is available at:
[Google Colab Notebook](https://colab.research.google.com/drive/1mOkShYZqOMrxAALBqcYaymlPHjQCnN0u?usp=sharing)

## No-Code Declaration

All dashboard development and ETL work was carried out without programming or scripting, using only the native features of each platform. The Python notebook for distributional analysis is a supporting research computation, not part of the dashboard workflow.

## License

This repository is provided for academic and research purposes in support of the published paper.
