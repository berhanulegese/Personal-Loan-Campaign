## Personal Loan Campaign Prediction

This project builds and evaluates a supervised machine learning model to identify bank customers with a high likelihood of purchasing a personal loan. By analyzing historical campaign data and customer attributes, the model helps the marketing team target prospects more effectively, improving campaign efficiency and conversion rates.

### What This Project Accomplishes
- Predicts which liability customers are likely to accept a personal loan offer (binary classification).
- Quantifies feature importance to explain key drivers of loan uptake (e.g., income, credit usage, education).
- Evaluates model performance using accuracy, precision, recall, F1-score, and a confusion matrix on a hold-out test set.
- Provides a reproducible workflow in a Jupyter/Colab notebook that can be adapted for local runs.

### Data
- File: `Loan_Modelling.csv`
- Target: `Personal_Loan` (0 = No, 1 = Yes)
- Example features: `Age`, `Experience`, `Income`, `Family`, `CCAvg`, `Education`, `Mortgage`, `Securities_Account`, `CD_Account`, `Online`, `CreditCard`, `ZIPCode`.

### How to Use
1. Open `AIML_ML_Project_Full_Code_Notebook.ipynb` in Jupyter or Google Colab.
2. For local use, comment out any Google Drive mounting code and set the data path to the local file:
   ```python
   file_path = 'Loan_Modelling.csv'
   df = pd.read_csv(file_path)
   ```
3. Run cells sequentially to train, tune (via `GridSearchCV` for decision trees), and evaluate the model. The notebook reports metrics and feature importance, and visualizes results.

### Repository Contents
- `AIML_ML_Project_Full_Code_Notebook.ipynb`: End-to-end modeling workflow.
- `AIML_ML_Project_Full_Code_Notebook.html`: Rendered version of the notebook.
- `Loan_Modelling.csv`: Dataset used for training and evaluation.
- `README.md`: Project overview and usage.

### Dependencies
Core Python packages: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `scipy`. If using Colab, these are preinstalled; for local runs, install as needed.
