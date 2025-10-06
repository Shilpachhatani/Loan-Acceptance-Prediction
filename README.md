# Loan-Acceptance-Prediction

## 📌 Project Overview & Task Objective

The (`Personal_Loan_Prediction.ipynb`) focused on predicting which bank customers are likely to accept a personal loan offer.
The primary objective is to build classification models that can accurately identify
potential loan acceptors, leveraging the provided **Bank Marketing Dataset** from the UCI
Machine Learning Repository.

## 📂 Dataset Information
The project utilizes the Bank Marketing Dataset (from the UCI Machine Learning
Repository). This dataset contains various features related to bank customers and their
responses to a direct marketing campaign for personal loans. The target variable is **y**
`(1 = Accepted Loan, 0 = Not Accepted)`.

**Key Issues Handled**: - Categorical data (e.g., `job , marital , education , default ,
housing , loan , contact , month , poutcome` ) requiring encoding

## 🔧 Features

-  Data loading and initial inspection  
-  Encoding categorical variables (Label Encoding & One-Hot Encoding)  
-  Exploratory Data Analysis (EDA)  
-  Training & evaluating classification models: Logistic Regression, Decision Tree  

## ⚙️ Installation

To run the notebook locally, install the required libraries:

```bash
pip install pandas matplotlib seaborn scikit-learn
```

## 🚀 My Approach
My approach to Loan Acceptance Prediction involved the following steps:

1. 📚 **Library Import**  
   Imported essential Python libraries for data manipulation `( pandas )`,
   visualization `( matplotlib , seaborn )`, and machine learning `( sklearn )`.
   
3. 📄 **Data Loading**  
   Loaded `bank.csv` into a pandas DataFrame

4. 🧹 **Data Cleaning & Preparation**  
   - Ensured the target column y is numeric.
   - Checked for missing values (none found in this dataset).
   -  Encoded Categorical Variables: Applied Label Encoding for binary categorical features and One-Hot Encoding for multi-class
      categorical features.
    
6. 📊 **EDA**  
   - Explored how features like age, job, and marital status influence loan acceptance through various visualizations.
     
7. 🤖 **Model Training & Testing**  
   The dataset was split into training and testing sets.
   - **Logistic Regression**: A Logistic Regression model was trained. * Decision Tree
   - **Classifier**: A Decision Tree model was trained
     
8. 📈 **Model Evaluation**  
   - Evaluated the trained models using **accuracy score**, **confusion matrices**, and **classification reports** to
     assess their performance in predicting loan acceptance

## 🧰 Technologies Used

- PYTHON  
-  PANDAS  
-  MATPLOTLIB  
-  SEABORN  
-  SCIKIT-LEARN

## 📊 Visualizations

- 📋 **Categorical Features**: Bar plots for job, marital status, education
  - **Job and Loan Acceptance**
    ![image](https://github.com/user-attachments/assets/69fee8e0-3ca9-4d81-9cb6-b4fb6c2588ba)


        **Insight**:
        The Above Graph Shows:

        - **Management**, **technicians**, and **admin** have high participation.
        - **Students**, **entrepreneurs**, and **self-employed** have a higher acceptance rate, even if total counts are lower.
        - `Retired, housemaids, and blue-collar` workers have low acceptance.
    
    - **Marital Status vs Loan Acceptance**
      ![image](https://github.com/user-attachments/assets/3f73bc53-da8e-458b-b234-3b11fb33d97f)


        **Insight**:
        The Above Graph Shows:

        - Most clients are married, but the acceptance rate is low in that group.
        - Single people show a relatively higher acceptance rate than married or divorced.

    - **Education vs Loan Acceptance**
      ![image](https://github.com/user-attachments/assets/8a54e9d3-74bf-472b-be0e-43a1f27afa40)

      
        **Insight**:
        The Above Graph Shows:
        
        - People with tertiary (higher) education are more likely to accept offers.
        - Those with only primary education rarely accept.
        - Clients with unknown education also show very low acceptance.

  
- 📈 **Numerical Features**: Histograms/density plots for age, balance, duration
  - **Age and Loan Acceptance**
    ![image](https://github.com/user-attachments/assets/b22fb091-a04f-44e0-b636-2d9df8023ef1)


        **Insight**:
        The Above Graph Shows

        - Most clients are aged 30–40.
        - People around 30–35 are slightly more likely to accept.
        - Overall, younger people (25–40) have more acceptances than older ones.
  
- 🔁 **Confusion Matrix**: Performance visualization of each model
  - **Logistic Regression**
    ![image](https://github.com/user-attachments/assets/da15795d-7889-4f73-9356-3245c8b73553)

  - **Decision Tree**
    ![image](https://github.com/user-attachments/assets/a1279989-4dae-48a7-a1dd-c1059155c574)
    
        **Insight**:
        - Logistic Regression Accuracy: 89.39 %
        - Decision Tree Accuracy: 87%


## 📉 Results and Insights

💡 **Key Insights**:

- 🔍 Feature Importance:  duration of `contact`, `poutcome (previous outcome)`, and `balance` often show strong correlations with loan acceptance.  
- 🧠 Model Performance: The notebook evaluates **Logistic Regression** and **Decision Tree models**. The performance metrics `(accuracy, precision, recall, F1-score)`
     indicate their effectiveness in predicting loan acceptance. Logistic Regression model outperform the Decision Tree model depending on the dataset characteristics.  
- ⚠️ Target Imbalance: The dataset might exhibit an imbalance in the target variable (number of loan acceptors vs. non-acceptors), which is important to consider during evaluation.


✅ **Final Outcome**:  
Successfully built a pipeline for loan acceptance prediction—from preprocessing to model evaluation. These models assist banks in targeting customers for marketing efforts. Future improvements can include advanced feature engineering, class imbalance handling, and ensemble methods.


## 📎 Usage

```bash
# Clone the repository (replace URL with your actual GitHub repo)
git clone https://github.com/your-username/Personal-Loan-Prediction.git

# Navigate into the directory
cd Personal-Loan-Prediction

# Open the notebook
jupyter notebook Personal_Loan_Prediction.ipynb
```

Run all notebook cells to explore analysis, training, and predictions.

---


## 🤝 Contributing

Contributions are welcome!  
Feel free to open an issue or submit a pull request with suggestions or improvements.

## 📬 Contact
For questions or collaboration:

GitHub: `AhsanNFt`
Email: `syedahsan0991@gmail.com`
