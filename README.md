# Google Meridian Demo

This repository demonstrates how to set up and run **Google Meridian**, an advanced open-source Marketing Mix Modeling (MMM) framework, using sample marketing data. The example focuses on a use case with 5 geo locations and 4 marketing channels, including impressions, spend, conversions, and reach/frequency data.

---

## Features

- **Data Loading:** Load and preprocess marketing, conversions, and reach/frequency data  
- **Model Configuration:** Define model specifications and priors tailored to your data  
- **Model Diagnosis:** Run Bayesian sampling and evaluate convergence diagnostics  
- **Visualization:** Generate insightful plots for ROI, saturation, reach/frequency, and budget allocation  
- **Budget Optimization:** Perform media spend optimization to maximize incremental KPI (conversions)  

---

## Repository Structure

```
.venv/              # Python virtual environment with google-meridian installed
data/               # Sample dataset (demo_v1.csv)
models/             # Save and load trained Meridian models
notebooks/          # Jupyter notebook demo.ipynb showcasing full workflow
reports/            # Generated model reports and visualizations
LICENSE             # MIT License
README.md           # This documentation file
```

---

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/bhauryal-eliya/Meridian-Demo.git
   cd meridian-demo
   ```

2. Create and activate the Python virtual environment:
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate   # On Windows: .venv\Scripts\activate
   ```

3. Install required packages including Google Meridian:
   ```bash
   pip install --upgrade pip
   pip install google-meridian
   ```

4. Open the Jupyter notebook and run the demo:
   ```bash
   jupyter notebook notebooks/demo.ipynb
   ```

---

## Usage

The notebook `demo.ipynb` walks through the entire modeling pipeline:

- Loading the example dataset (`data/demo_v1.csv`) containing impressions, spend, conversions, revenue per conversion, population, and reach/frequency data  
- Setting up the model with geo-location hierarchy and control variables  
- Running MCMC sampling for model fitting  
- Diagnosing model performance and generating plots  
- Performing budget optimization to suggest spend adjustments across channels  

You can replace the sample data with your own by updating the CSV file and adjusting the configuration accordingly.

---

## License

This project is licensed under the MIT License.

---
