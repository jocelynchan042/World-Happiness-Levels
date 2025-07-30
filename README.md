# Happiness Prediction Levels with Logistic Regression and Random Forest

This project explores and predicts **Happiness Levels** (Low, Medium, High) across countries based on social, economic, and political indicators using **machine learning classification models**.

## 📊 Dataset

The dataset is derived from the **World Happiness Report** and includes features such as:

- Log GDP per capita  
- Social support  
- Healthy life expectancy  
- Freedom to make life choices  
- Generosity  
- Perceptions of corruption  
- Positive & Negative affect  
- Confidence in national government  
- Democratic Quality  
- Delivery Quality  

## 🧰 Tools & Libraries

- **Python**  
- **pandas** – data loading and manipulation  
- **seaborn** & **matplotlib** – visualizations  
- **scikit-learn** – machine learning (model building, evaluation, hyperparameter tuning)  
- **NumPy** – numerical operations  

## 🧠 Models Used

### 1. Logistic Regression (multinomial)
- StandardScaler used for feature scaling
- GridSearchCV for hyperparameter tuning
- Evaluated with accuracy, precision, recall, F1-score, and confusion matrix

### 2. Random Forest Classifier
- No feature scaling required
- RandomizedSearchCV for hyperparameter tuning
- Evaluated with same classification metrics

## 📈 Performance Summary

| Model             | Accuracy | Macro F1 | Comments                                  |
|------------------|----------|----------|-------------------------------------------|
| Logistic (default) | ~73.7%   | ~0.73    | Strong for Medium class, weaker on others |
| Logistic (tuned)   | ~73.8%   | ~0.73    | Slightly improved, more stable precision  |
| Random Forest (default) | **~79.8%** | ~0.77    | Best overall performance                  |
| Random Forest (tuned)   | ~78.9%   | ~0.78    | Balanced recall across all classes        |

## 📂 File Structure
├── happiness_prediction.ipynb

├── README.md

└── data/

  └── world_happiness.csv

## 📌 Key Takeaways

- **Random Forest** outperformed Logistic Regression in most metrics.
- Tuning helped both models become more balanced.
- "Medium" happiness levels are easiest to predict, while "Low" had the most misclassifications.
- This project highlights how social and economic indicators influence national happiness levels.


