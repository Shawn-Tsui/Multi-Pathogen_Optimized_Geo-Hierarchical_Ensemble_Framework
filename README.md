# Multi-Pathogen-Optimized-Geo-Hierarchical-Ensemble-Framework

This repository accompanies the manuscript **"A Multi-Pathogen Hospitalization Forecasting Model for the United States: An Optimized Geo-Hierarchical Ensemble Framework"**, providing the code and resources used for developing and evaluating models for forecasting hospitalizations due to **Influenza**, **COVID-19**, and **RSV** in the United States.

## Repository Structure

### 1. COVID-19 and Influenza Folders
- Contains the forecasting models:
  - **Single-State Model**: Captures state-specific hospitalization trends.
  - **Regionally-Trained Model**: Trained on geographically clustered groups of states.
  - **Nationally-Trained Model**: Trained on aggregated data across all states.
- Each folder includes:
  - **`overall_analysis.ipynb`**: Aggregates outputs from individual models to generate ensemble forecasts.

### 2. RSV Folder
- Contains:
  - **Single-State Model**
  - **Nationally-Trained Model**
- Due to data limitations (only 12 reporting states), RSV models do not include a regionally-trained model.
- Includes **`overall_analysis.ipynb`** for ensemble forecast generation.

### 3. Common Features
- All models were developed and executed in **Google Colab**, leveraging **T4 GPU** for computational efficiency.
- Each notebook includes comments and step-by-step instructions for replicating the analyses.

## Usage Instructions

1. 	Navigate to the desired pathogen folder (e.g., influenza, covid-19, or rsv).
2.	Open the overall_analysis.ipynb file in Google Colab to:
	-	Aggregate model outputs.
	-	Generate ensemble forecasts using the Optimized Geo-Hierarchical Ensemble Framework.
3. Follow the provided steps in the notebooks to train, test, and evaluate forecasting models.

## Notes

-	Models for Influenza and COVID-19 include a three-tier structure (single-state, regionally-trained, and nationally-trained), while RSV models only include single-state and nationally-trained due to data constraints.
-	Ensemble weighting methods (e.g., Linear Programming (LP) and RECI by Horizon) are implemented in the overall_analysis.ipynb files.

For additional details on methodologies, models, and ensemble strategies, please refer to the manuscript.
