# Cefepime Resistance Predictor: Unlocking E. coli Insights

This project predicts the resistance and susceptibility of the Cefepime antibiotic in *E. coli* bacteria. It analyzes three machine learning models—Random Forest Classifier, Logistic Regression, and Gradient Boosting—using two feature types: gene Presence/Absence and K-mers. The goal is to identify genetic mutations and sequences responsible for Cefepime resistance.

## Author

Jhanavi Dave

## Project Overview

- **Models Used:** Random Forest, Logistic Regression, Gradient Boosting
- **Feature Sets:** 
  - Presence/Absence (high-level genetic markers)
  - K-mers (fine-grained genomic details)
- **Approach:** 
  - Data loading and preprocessing
  - Feature engineering (gene presence/absence matrix, k-mer counting)
  - Model training and prediction
  - Hyperparameter tuning (Grid Search and Randomized Search)
  - Performance evaluation and visualization

## Workflow Summary

1. **Data Loading:**  
   Loads presence/absence data, k-mer features, labels, and genome IDs from CSV and NPY files.  
2. **Feature Engineering:**  
   - Builds gene presence/absence matrices.
   - Generates k-mer features from genomic sequences.
3. **Model Training:**  
   - Trains Random Forest, Logistic Regression, and Gradient Boosting models on both feature sets.
   - Saves predictions for each model-feature combination.
4. **Visualization:**  
   - Plots predictions for each model and feature type.
5. **Hyperparameter Tuning:**  
   - Performs Grid Search and Randomized Search for optimal model parameters.
6. **Evaluation:**  
   - Reports balanced accuracy scores for all models and feature sets.
   - Compares results using both cross-validation and Kaggle test scores.

## Key Results

- **Random Forest with K-mers features** achieved the highest balanced accuracy and Kaggle test score.
- Combining multiple feature sets improves model robustness and prediction accuracy.
- Gradient Boosting was less effective due to computational constraints.

### Example Balanced Accuracy Scores

- **Random Forest (K-mers):**  
  - Grid Search: 0.82  
  - Random Search: 0.84  
  - Kaggle: 0.91
- **Logistic Regression (K-mers):**  
  - Grid Search: 0.81  
  - Random Search: 0.80  
  - Kaggle: 0.81

## Repository

Project notebook and code:  
[https://github.com/jhanavidave/Cefepime-Resistance-Predictor-Unlocking-E.-coli-Insights.git](https://github.com/jhanavidave/Cefepime-Resistance-Predictor-Unlocking-E.-coli-Insights.git)

---

**Note:** The latest contents and updates are yet to be added.