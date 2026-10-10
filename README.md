# Machine Learning for Manufacturing

Course projects completed for **Machine Learning for Manufacturing** at  
**Case Western Reserve University**.

**Author:** BATHLOMEW A. EBIKA

This repository contains Jupyter Notebook implementations of machine-learning
methods applied to manufacturing process data.

---

## Repository Contents

### Project 1

**File:** `Project_1_PCE13.ipynb`

Project 1 introduces the application of machine-learning methods to a
manufacturing-data problem. The notebook contains the complete workflow,
including data preparation, model development, evaluation, visualization,
and interpretation of results.

---

### Project 2 – Material Removal Rate Prediction

**File:** `Project_2_PCE13.ipynb`

Project 2 focuses on predicting **Material Removal Rate (MRR)** in a
Chemical Mechanical Polishing (CMP) process using multiple regression and
Multilayer Perceptron neural networks.

The project compares two sensing-variable combinations:

- All sensing variables, **x7–x25**
- Polishing pad and dresser condition variables, **x7–x10**

### Models Implemented

1. Multiple Linear Regression using self-coded Gradient Descent
2. Multiple Linear Regression using Scikit-Learn
3. Self-coded Three-Layer Multilayer Perceptron
4. Three-Layer MLP using PyTorch
5. Self-coded Four-Layer Multilayer Perceptron

Different learning rates, hidden-layer sizes, network architectures, and
feature combinations were evaluated.

### Performance Metrics

Model performance was evaluated using:

- Root Mean Square Error (**RMSE**)
- Coefficient of Determination (**R²**)

### Best Project 2 Result

The best overall performance was obtained using a **self-coded four-layer MLP**
with the reduced **x7–x10** input-variable set.

- Architecture: `4 → 8 → 4 → 1`
- Learning rate: `0.0002`
- Test RMSE: **3.1160**
- Test R²: **0.3281**

The results demonstrated that increasing model complexity or adding more input
variables does not necessarily improve generalization. The reduced polishing
pad and dresser feature set provided strong predictive information for MRR.

---

## Technologies Used

- Python
- Jupyter Notebook
- NumPy
- SciPy
- Matplotlib
- Scikit-Learn
- PyTorch

---

## Running the Notebooks

Clone the repository:

```bash
git clone https://github.com/peaceebika/Machine-Learning-for-Manufacturing.git
