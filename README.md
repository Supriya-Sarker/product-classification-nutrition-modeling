# Product Classification and Nutrient Prediction

Machine learning on two public product datasets: classifying drug products into pharmacological classes, and predicting nutrient content of foods (Spring 2025).

## Projects

### 1. Drug product classification (`drug_product_classification/`)
- **Task:** predict a product's pharmacological class from its attributes (a product categorization problem).
- **Models:** naive Bayes, KNN, and random forests, tuned with grid search and stratified k-fold cross-validation.

### 2. Nutrient prediction and food segmentation (`nutrition_prediction/`)
- **Task:** predict protein content of foods from their other nutrient attributes, and group similar foods.
- **Models:** KNN and random forest regressors, and a neural network tuned with KerasTuner.
- **Unsupervised:** PCA, t-SNE, and K-means clustering for product segmentation.

## Evaluation note
Validation is being redesigned to avoid data leakage: products that share an active ingredient will be kept in the same fold, and features that are derived from the target will be removed. Results will be reported after these fixes.

## Data
Public Kaggle datasets (drug products and USDA nutrition data). The data files are not stored in this repo; download links will be added here.

## Status
In progress. Cleaned notebooks, scripts, and results will be added to each folder step by step.

## Tech
Python, pandas, NumPy, scikit-learn, TensorFlow/Keras, KerasTuner, Matplotlib
