# MLP-CW4

# Market Regime Prediction Using Self-Supervised Learning: A Contrastive Approach

This repository contains code for Market Regime Prediction using the baseline, **CoST (Contrastive Learning for Time Series)** model, **Time Series Temporal Contrastive Coding (TS-TCC)**, and **Temporal Neighborhood Coding (TNC)** . The models are applied to S&P 500 index data and sectoral data (XLK, XLF, XLV, XLE, XLY, XLI).

## Repository Structure

```
financial-time-series-analysis/
├── data/
│   └── final_data.csv            # Preprocessed dataset
├── notebooks/
│   ├── baseline.ipynb            # Baseline model implementation
│   ├── CoST_model.ipynb          # CoST model implementation
│   ├── ts-tcc.ipynb              # Time Series Temporal Contrastive Coding (TS-TCC) 
│   └── tnc.ipynb                  # Time Series Classification (TC) implementation
├── README.md                     # This file
```

## Getting Started

### 1. Clone the Repository

Clone this repository to your local machine using the following command:

```bash
git clone https://github.com/pragati2526/MLP-CW4.git
cd MLP-CW4
```

### 2. Download the Dataset

The preprocessed dataset (`final_data.csv`) is required to run the notebooks. It contains the following data:
- **S&P 500 Index Data**
- **Sectoral Data**: XLK (Technology), XLF (Financial), XLV (Healthcare), XLE (Energy), XLY (Consumer Discretionary), XLI (Industrial).

Download the dataset from the `data` folder or use the following link:  
[Download final_data.csv](https://your-dataset-link/final_data.csv)

Place the downloaded `final_data.csv` file in the `data` folder.

### 3. Set Up the Environment

Install the required Python dependencies using the provided `requirements.txt` file:

```bash
pip install -r requirements.txt
```

### 4. Run the Notebooks

The `notebooks` directory contains the following Jupyter notebooks:

- **`baseline.ipynb`**: Baseline model implementation for financial time series analysis.
- **`CoST_model.ipynb`**: Implementation of the CoST (Contrastive Learning for Time Series) model.
- **`ts-tcc.ipynb`**: Implementation of Time Series Temporal Contrastive Coding (TS-TCC).
- **`tnc.ipynb`**: Implementation of Temporal Neighborhood Coding (TNC).

To run the notebooks, navigate to the `notebooks` directory and open the desired notebook in Jupyter:

```bash
cd notebooks
jupyter notebook
```

Then, open and run the notebooks one by one to replicate the results.

---

## Dataset Details

The `final_data.csv` file contains the following columns:

- **Date**: The date of the observation.
- **Ticker**: The ticker symbol (e.g., `^GSPC` for S&P 500, `XLK` for Technology, etc.).
- **Open**: The opening price.
- **High**: The highest price during the day.
- **Low**: The lowest price during the day.
- **Close**: The closing price.
- **Volume**: The trading volume.

---

## Models Overview

### 1. Baseline Model (`baseline.ipynb`)
- Implements a simple baseline model for financial time series analysis.
- Uses traditional statistical and machine learning techniques.

### 2. CoST Model (`CoST_model.ipynb`)
- Implements the **CoST (Contrastive Learning for Time Series)** model.
- Captures both seasonal and trend components in the time series data.
- Uses contrastive learning to improve representation learning.

### 3. TS-TCC Model (`ts-tcc.ipynb`)
- Implements **Time Series Temporal Contrastive Coding (TS-TCC)**.
- Focuses on temporal contrastive learning for time series data.

### 4.TNC Model (`tnc.ipynb`)
- Implements Temporal Neighborhood Coding (TNC)
- Focuses on learning representations by contrasting temporal neighborhoods in the time series data.

---
