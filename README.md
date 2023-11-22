# Project Title

Explainable Models for Epidemiological Forecasting

## Description

This repository contains various resources and notebooks for COVID-19 data analysis and forecasting. Below is the structure and contents of this repository:

### Directory Structure

- `doc/`: Contains the final report PDF and final presentation slides.
- `src/datasets`: This directory contains two different filetype versions of the latest OWID COVID-19 dataset:
    - CSV format: `src/datasets/owid-covid-data.csv`
    - JSON format: `src/datasets/owid-covid-data.json`
    - Dataset source: [OWID COVID-19 Data Repository](https://github.com/owid/covid-19-data/tree/master/public/data/latest)
- `src/plots`:
    - Stores plots generated for analysis including SHAP force plots.
    - Example plot: `src/plots/cases_vaccinations_hosp_patients_stringency.png` – a time series data trend visualization.

### Notebooks

1. `explainable-forecasting-main.ipynb`:
    - Preprocessing dataset
    - Multivariate time-series forecasting models (VAR and LSTM)
    - Global and local feature explainability analysis
    - Comments and annotations for clarity

2. `time-series-data-analysis-main.ipynb`:
    - Dataset preprocessing
    - Comparative time series data trend visualization analysis

### Installation

Install the following packages using PIP for Python:

- `pandas`
- `matplotlib`
- `statsmodels`
- `scikit-learn`
- `numpy`
- `scipy`
- `tensorflow==1.14.0` (Specific version required for SHAP compatibility)
- `keras`
- `shap`

Note: `json` and `datetime` are standard Python libraries and do not require separate installation.

### Instructions

- Install the required packages.
- Maintain the file/directory structure as is.
- Open the notebooks in Google Colab, local Jupyter Notebook, or Kaggle.
- Trust the notebook to view outputs, especially SHAP analysis JavaScript visualizations.

### How to Use / Run a Demo

1. Run all cells of `explainable-forecasting-main.ipynb` in your preferred environment (e.g., Jupyter, Google Colab, Kaggle) to view results and outputs. Note: LSTM model results may vary slightly with each run due to different seed values.
2. Run all cells of `time-series-data-analysis-main.ipynb` to generate visualizations of time series trends for the four countries (USA, FRA, ITA, JPN).

---

