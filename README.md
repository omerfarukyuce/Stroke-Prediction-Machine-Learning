# 🧠💻 Stroke Prediction Machine Learning Project 

## 🎯 Project Objective 
This project involves the development of a machine learning model to predict stroke risk using individuals' health data. Data preprocessing, feature engineering and natural language processing (NLP) techniques were used. As a result of the dataset used and the methods applied, an average success rate of 52% was achieved. This reveals both the limitations of the dataset and the complexity of stroke prediction. Higher success rates are targeted in the future with more comprehensive datasets and advanced modeling methods.

## 📚 Libraries Used 
- **`pandas`**: For data analysis and manipulation.
- **`numpy`**: For numerical computations.
- **`matplotlib`**: For data visualization.
- **`sklearn`**: For machine learning algorithms and model evaluation.
- **`xgboost`**: For advanced tree-based modeling.
- **`nltk`**: For natural language processing.
- **`graphviz`**: For visualizing decision trees.

## 📊 Dataset Information 

The dataset includes:

- Demographic details (Age, Gender, Marital Status)
- Health conditions (Hypertension, Heart Disease, Glucose Level, BMI, HDL, LDL)
- Lifestyle factors (Smoking, Alcohol, Physical Activity, Diet)
- Symptoms (free-text `Symptoms` column)
- Stroke history, family history, and diagnosis info

The dataset contains 15,000 patient records and includes the following columns:

| Column Name                     | Non-Null Count | Data Type  |
|---------------------------------|----------------|------------|
| Patient ID                      | 15000          | int64      |
| Patient Name                    | 15000          | object     |
| Age                             | 15000          | int64      |
| Gender                          | 15000          | object     |
| Hypertension                    | 15000          | int64      |
| Heart Disease                   | 15000          | int64      |
| Marital Status                  | 15000          | object     |
| Work Type                       | 15000          | object     |
| Residence Type                  | 15000          | object     |
| Average Glucose Level           | 15000          | float64    |
| Body Mass Index (BMI)           | 15000          | float64    |
| Smoking Status                  | 15000          | object     |
| Alcohol Intake                  | 15000          | object     |
| Physical Activity               | 15000          | object     |
| Stroke History                  | 15000          | int64      |
| Family History of Stroke        | 15000          | object     |
| Dietary Habits                  | 15000          | object     |
| Stress Levels                   | 15000          | float64    |
| Blood Pressure Levels           | 15000          | object     |
| Cholesterol Levels              | 15000          | object     |
| Symptoms                        | 12500          | object     |
| Diagnosis                       | 15000          | object     |

## 🧹 Data Preprocessing

- No missing values in the dataset
- Numerical features were scaled using Min-Max normalization
- `Symptoms` column:
  - Stopwords removed
  - Converted to lowercase
  - Combined with underscores (`difficulty_speaking`, `loss_balance`, etc.)
  - A new `Cleaned_Symptoms` column was added

 ## 🧠 Feature Engineering

- CountVectorizer and TF-IDF applied to the `Symptoms` column
- Text mining techniques applied to `Cleaned_Symptoms`
- One-hot or TF-IDF matrices can be used as additional model features

## 📈 Results 
The modeling process evaluated the success rates and classification reports obtained using different machine learning algorithms. The results demonstrate the complexity of stroke prediction and the limitations of the dataset.

## 🚀 Usage 
The project is designed to be run on Google Colab. Necessary libraries should be installed, and the dataset should be processed appropriately.

## 📝 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## 🔍 Code And Kaggle Link
Project: [Stroke Prediction](https://github.com/omerfarukyuce/stroke-prediction-machine-learning)

Kaggle: [🧠Stroke Prediction & Analysis (EDA)🩺](https://www.kaggle.com/code/merfarukyce/stroke-prediction-analysis-eda)

## 📊 Dataset
Dataset: [Dataset](https://www.kaggle.com/datasets/teamincribo/stroke-prediction?select=stroke_prediction_dataset.csv)
