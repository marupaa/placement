# Customer Churn Analysis — Setup Guide

This document explains how to prepare your Google Drive and run the data preparation script/notebook for the Customer Churn Analysis project.

---

## 📂 Google Drive Setup

1. Open **Google Drive**.

2. Inside **MyDrive**, create a new folder named:

   ```
   CustomerChurnAnalysis
   ```

3. Upload your raw dataset into this folder.

4. Rename the dataset file to:

   ```
   originalDataSet.csv
   ```

---

## ✅ Final Folder Structure

After setup, your Google Drive should look like this:

```
MyDrive/
└── CustomerChurnAnalysis/
    └── originalDataSet.csv
```

---

## 🚀 Running in Google Colab

1. Mount your Google Drive:

   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

2. Open and run `customerChurnAnalysis.ipynb` (or `customerChurnAnalysis.py`).

3. Outputs will be saved automatically into:

   ```
   /content/drive/MyDrive/CustomerChurnAnalysis/Data_Preparation/
   ```

---

## 📊 Expected Outputs

After running the notebook/script, you should see the following files in `Data_Preparation/`:

* `01_missing_data_handled.csv`
* `02_categorical_encoded.csv`
* `X_train.csv`, `X_test.csv`
* `y_train.csv`, `y_test.csv`
* `Preprocessing_Report.md`
* `Scaling_Techniques_Documentation.md`
* `Train_Test_Split_Documentation.md`

---

## 📝 Notes

* Always keep the dataset file name exactly as `originalDataSet.csv`.
* The folders `Data_Preparation` (and later `Clustering_Analysis`) will be created automatically when you run the scripts.
