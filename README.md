# Best-model-per-dataset-LightGBM-XGBoost-or-CatBoost(Run on Gpu Power)
⚡ Fast & Easy Model Runner

🚀 Runs on GPU — Just Import & Run on ![Kaggle](https://img.shields.io/badge/Kaggle-blue?logo=kaggle)
## 👤 Author

| 👤 **Name** | 🔗 **Github-Profile** |🔗 **Kaggle-Profile** |
|------------|----------------|----------------|
| Riddy Mazumder | [![GitHub](https://img.shields.io/badge/GitHub-RiddyMazumder-black?logo=github)](https://github.com/RiddyMazumder)|[![Kaggle Profile](https://img.shields.io/badge/Kaggle-RiddyMazumder-blue?logo=kaggle)](https://www.kaggle.com/riddymazumder)|

This notebook allows you to quickly train and evaluate the best-performing model on any dataset using one of three powerful algorithms:

LightGBM

XGBoost

CatBoost
## 📝 How to Run 
>1️⃣ Import the Notebook

Open the notebook in your preferred environment:

1.Kaggle Notebook     [![Kaggle](https://img.shields.io/badge/Kaggle-blue?logo=kaggle)](https://www.kaggle.com/) [Easy Method]

2.Google Colab [![Google Colab](https://img.shields.io/badge/Colab-Open%20Notebook-orange?logo=googlecolab)](https://colab.research.google.com/)


3.Jupyter Notebook [![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)


>2️⃣ Activate GPU

For faster training, enable GPU acceleration:

Kaggle: Settings → Accelerator → GPU

Google Colab: Runtime → Change runtime type → GPU

Jupyter Notebook: Ensure a CUDA-enabled GPU is available on your system

Note for Jupyter and Google Colab: Ensure all required dependencies are installed: LightGBM, XGBoost, CatBoost, etc.
Simply import the notebook and execute it on Kaggle — no setup required. The code automatically detects the best model for your dataset and leverages GPU acceleration for fast training and evaluation.

>3️⃣ Select Dataset

Upload your dataset or select one from the available Kaggle/Colab datasets.

>4️⃣ Hit Run

Run all cells sequentially to start training and evaluation.

>5️⃣ View Results

The notebook automatically:

Show the best-performing model

Displays key performance metrics

Provides a summary table of results
# 🔥 Model Performance Summary
| Model              | Train Score | Validation Score | Overfitting | n_estimators | learning_rate | max_depth | subsample | colsample_bytree | min_child_weight | gamma | reg_alpha | reg_lambda | num_leaves | iterations | depth | l2_leaf_reg | border_count | bootstrap_type | best_iteration | Gap (Train - Val) | Gap_Rank | Gap_Stars | Overfit_Score | Sort_Validation | Sort_Overfit | Overfit_Rank | Combined_Rank | Best_Model 🏆 |
| ------------------ | ----------- | ---------------- | ----------- | ------------ | ------------- | --------- | --------- | ---------------- | ---------------- | ----- | --------- | ---------- | ---------- | ---------- | ----- | ----------- | ------------ | -------------- | -------------- | ----------------- | -------- | --------- | ------------- | --------------- | ------------ | ------------ | ------------- | ------------- |
| CatBoostClassifier | 0.679461    | 0.675743         | Yes         | -            | 0.10          | -         | 1.0       | -                | -                | -     | -         | -          | -          | 792        | 4     | 9           | 64           | Bernoulli      | 791            | 0.0037            | 1        | ⭐         | 0.003718      | 0.675743        | -0.003718    | 3            | 1             | 🏆            |
| XGBClassifier      | 0.687661    | 0.680436         | Yes         | 799          | 0.01          | 7         | 0.95      | 0.6              | 1                | 0.01  | 0.01      | 1          | -          | -          | -     | -           | -            | -              | -              | 0.0072            | 2        | ⭐⭐        | 0.007225      | 0.680436        | -0.007225    | 2            | 2             | -             |
| LGBMClassifier     | 0.712311    | 0.684243         | Yes         | 2000         | 0.01          | -1        | 0.95      | 1.0              | -                | -     | -         | -          | 127        | -          | -     | -           | -            | -              | -              | 0.0281            | 3        | ⭐⭐⭐       | 0.028068      | 0.684243        | -0.028068    | 1            | 3             | -             |
# CatBoostClassifier is the best model for this dataset 🏆, balancing validation performance and overfitting.
