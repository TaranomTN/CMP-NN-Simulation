# CMP-NN-Simulation

## Model Comparison on Simulated Count Data

This project evaluates the performance of two variants of the **Compound Poisson Neural Network (CMP-NN)** in predicting count data using simulated datasets. The focus is on comparing models with different latent variable settings.

Models compared:
- **Poisson Neural Network with ν = 1**  
- **Poisson Neural Network with ν = 2**

---

### 📊 Model Comparison Based on MAE, MSE, and RMSE

| Model                            | Number of Parameters | MAE   | MSE    | RMSE |
|----------------------------------|----------------------|-------|--------|------|
| Poisson NN (ν = 1)               | 141                  | 4.14  | 31.78  | 5.63 |
| **Poisson NN (ν = 2)**    | **162**              | **1.26** | **2.21** | **1.48** |

> ✅ Our proposed model with **ν = 2** achieves significantly lower error rates across all metrics, while having a slightly higher number of parameters.

---

### 🧠 Key Insights

- Increasing the latent variable ν improves model flexibility and predictive accuracy.
- The model with ν = 2 captures complex patterns in count data more effectively.
- Despite higher complexity, the improvement in accuracy justifies the increased parameter count.

---

### 📁 Files

- `cmp_nn_simulation.ipynb`: Colab notebook containing simulation setup, model training, and evaluation.


---

### 🔧 Requirements

- Python 3.x
- Jupyter Notebook or Colab
- Required libraries: `pandas`, `numpy`, `scikit-learn`, `torch`, `statsmodels`

Install dependencies:
```bash
pip install pandas numpy scikit-learn torch statsmodels
```
