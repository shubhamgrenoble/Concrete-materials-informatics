# Hybrid Concrete Strength Prediction (Physics + AI)

## Project Overview
This project demonstrates a **hybrid modeling approach** to predict the compressive strength of concrete. Unlike standard "black box" machine learning models, this solution integrates **domain knowledge (Civil Engineering physics)** with **Data Science**.

It was developed to solve the common industry challenge of optimizing concrete formulations while minimizing costly experimental trial batches.

## Key Features
- **Physical Modeling:** Implements a generalized form of **Abram’s Law** (Water/Binder ratio) to constrain predictions within physically realistic bounds.
- **Machine Learning:** Uses a **Random Forest Regressor** to capture complex, non-linear interactions between chemical admixtures (superplasticizers) and mineral additions (Slag/Fly Ash).
- **Optimization Engine:** Includes an algorithm to find the most cost-effective mix design (minimizing binder content) for a specific target strength (e.g., 40 MPa).

## Technical Stack
- **Language:** Python 3.x
- **Libraries:** Pandas, NumPy, Scikit-Learn, SciPy (Curve Fitting)
- **Physics:** Feret's Equation / Abram's Law implementation

## Results
- **Physical Model:** $R^2 \approx 0.60$ (Provides interpretability and baseline)
- **Hybrid Random Forest:** $R^2 > 0.90$ (Provides high precision)
- **Outcome:** The model successfully identifies mix designs that meet strength requirements while optimizing for sustainability.

## How to Run
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
