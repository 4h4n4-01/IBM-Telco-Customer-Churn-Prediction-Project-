# Telco Churn ML Lab (Jupyter / VS Code)

IBM Telco Customer Churn project — **all code lives in Jupyter notebooks** for learning supervised & unsupervised ML with **scikit-learn** and **PyTorch**.

## Location

```
C:\Users\Ahana\Desktop\telco-churn-ml-lab
```

## VS Code setup

1. Install [Python](https://www.python.org/downloads/) and [VS Code](https://code.visualstudio.com/).
2. Install extensions: **Python**, **Jupyter**.
3. Open folder: **File → Open Folder** → `telco-churn-ml-lab`.
4. Terminal → create environment:

   ```powershell
   cd "C:\Users\Ahana\Desktop\telco-churn-ml-lab"
   python -m venv .venv
   .venv\Scripts\Activate.ps1
   pip install -r requirements.txt
   python -m ipykernel install --user --name=telco-ml --display-name "Python (telco-ml)"
   ```

5. Download dataset → save as:
   `data/raw/WA_Fn-UseC_-Telco-Customer-Churn.csv`  
   [Kaggle link](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

6. Open `notebooks/` and run notebooks **in order**. In each notebook: **Select Kernel** → `Python (telco-ml)`.

## Notebook order

| # | Notebook | Topic |
|---|----------|--------|
| 00 | `00_setup_and_eda.ipynb` | Load data, clean, explore |
| 01 | `01_supervised_sklearn.ipynb` | Logistic Regression, Random Forest, churn |
| 02 | `02_unsupervised_sklearn.ipynb` | KMeans customer segments |
| 03 | `03_supervised_pytorch.ipynb` | MLP classifier, training curves |
| 04 | `04_unsupervised_pytorch.ipynb` | Autoencoder + clustering |
| 05 | `05_compare_models.ipynb` | Compare metrics, sample predictions |

## Outputs (after running notebooks)

- `data/processed/telco_clean.csv` — cleaned data
- `models/` — saved sklearn & PyTorch models, metrics JSON, plots
