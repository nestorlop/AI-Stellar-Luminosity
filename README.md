# AI-Stellar-Luminosity

**Course:** Transformación Digital y Soluciones Empresariales (TDSE)
**Student:** Nestor David Lopez Castañeda
**Date:** August 3, 2026

This project studies how a regression model learns from data. It implements vectorized
linear and polynomial regression from first principles (with no machine-learning libraries)
to model the relationship between the mass and luminosity of main-sequence stars, compares
both models, and reflects on what the experiment teaches about AI in general. The complete
technical work — code, plots, results, and reflections — is in `stellar_luminosity_hands_on.ipynb`.

## Requirements

- Python 3
- NumPy
- Matplotlib
- Jupyter Notebook

## How to run

1. Clone the repository:
   `git clone https://github.com/nestorlop/AI-Stellar-Luminosity.git`
2. Create a virtual environment and install dependencies:
   `python -m venv .venv` → activate it → `pip install numpy matplotlib jupyter`
3. Open and run the notebook:
   `jupyter notebook stellar_luminosity_hands_on.ipynb` → Kernel → Restart & Run All

## Main result

The polynomial model using mass and mass squared provides a much better fit to the observed data than the linear model, with a final cost of 2.96 compared to 13.82. The residuals also appear more randomly distributed, suggesting that the model captures the trend in the data better. However, a lower training error does not guarantee that the model is physically meaningful. When extrapolating beyond the observed range (for example, at mass = 5.0), both models produce unreliable predictions, highlighting the importance of choosing an appropriate model and considering the limits of the available data.