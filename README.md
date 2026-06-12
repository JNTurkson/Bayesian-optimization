# Predicting Wettability of Hydrogen Mixtures Using Bayesian-Optimized Regression Model

## 1. Overview

This repository provides an interactive implementation of a Bayesian-optimized Extremely Randomized Trees (ET) model for predicting wettability of hydrogen mixtures. The model is deployed through a Gradio-based interface that enables rapid estimation of contact angle under variable reservoir conditions.

---

## 2. Model Description

The framework is based on an Extremely Randomized Trees (ET) regression model optimized using Bayesian hyperparameter tuning.

- **Model type:** Extremely Randomized Trees (ET)
- **Optimization method:** Bayesian optimization
- **Output variable:** Contact angle (<sup>o</sup>)
- **Input features:**
  - Pressure (MPa)
  - Temperature (K)
  - Salinity (mol/kg)
  - Gas composition
  - Density difference (kg/m<sup>3</sup>)

---

## 3. Features

- Interactive Gradio-based user interface  
- Real-time prediction of hydrogen wettability  
- Multivariable reservoir condition handling  
- Fast evaluation of subsurface scenarios  

---

## 4. Input Parameters

The model is valid within the following training ranges:

| Parameter | Training Range |
|------------|----------------|
| Pressure (MPa) | 3.45 – 20.68 |
| Temperature (K) | 303.15 – 343.15 |
| Salinity (mol/kg) | 0.34 – 3.42 |
| Hydrogen mole fraction (mol%) | 20 – 80 |
| Nitrogen mole fraction (mol%) | 5 – 70 |
| Methane mole fraction (mol%) | 5 – 70 |
| Density difference (kg/m<sup>3</sup>)| 836 – 1087 |

---

## 5. How to Run

### 5.1 Run the application

To use the tool:

1. Download or clone the repository to local computer.
2. Install the required Python packages: `gradio`; `pandas` ; `joblib`; `scikit-learn`; `numpy`.
3. Open and run the Jupyter Notebook (`HyWett_App.ipynb`).
4. Once executed, a local link will appear in the output.
5. Open the link in your web browser to access the interface.

### 5.2 Using the tool

Enter the required reservoir parameters in the interface:

- Pressure (MPa)  
- Temperature (K)  
- Salinity (mol/kg)  
- Hydrogen mole fraction (mol%)  
- Nitrogen mole fraction (mol%)  
- Methane mole fraction (mol%)  
- Density difference (kg/m³)  

Ensure that all inputs remain within the training ranges shown in the interface for reliable predictions.

### 5.3 Output

The model provides:

- Predicted contact angle (°)  
- Input validity status based on training range checks

### 5.4 Prediction Example
![HyWett GUI](https://github.com/JNTurkson/Bayesian-optimization/blob/main/Prediction_example.jpg)

---

## Citation
To be provided

---

## References

Muhammed, N. S., Haq, B., & Al Shehri, D. (2023b). Role of methane as a cushion gas for hydrogen storage in depleted gas reservoirs. **Int. J. Hydrogen Energy**. [https://doi.org/10.1016/j.ijhydene.2023.04.173](https://doi.org/10.1016/j.ijhydene.2023.04.173).

Muhammed, N. S., Haq, B., & Al Shehri, D. A. (2023c). Hydrogen storage in depleted gas reservoirs using nitrogen cushion gas: A contact angle and surface tension study. **Int. J. Hydrogen Energy**, 48(98), 38782-38807. [https://doi.org/10.1016/j.ijhydene.2023.06.208](https://doi.org/10.1016/j.ijhydene.2023.06.208).
