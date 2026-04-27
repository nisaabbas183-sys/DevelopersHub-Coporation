# Heart Disease Prediction

## 📋 Project Overview

This project implements a machine learning model to predict the presence of heart disease in patients using **Logistic Regression**. The model is trained on a comprehensive medical dataset containing 303 patient records with 13 medical features.

## 🎯 Objective

To build a predictive system that can accurately classify whether a person has heart disease (defective heart) or a healthy heart based on medical attributes.

## 📊 Dataset Information

### Dataset Size
- **Total Records**: 303 patients
- **Features**: 13 medical attributes
- **Target Variable**: 1 column (heart disease presence)

### Features Description

| Feature | Description | Type |
|---------|-------------|------|
| age | Age of the patient in years | Integer |
| sex | Gender (0 = Female, 1 = Male) | Binary |
| cp | Chest pain type (0-3) | Integer |
| trestbps | Resting blood pressure (mm Hg) | Integer |
| chol | Serum cholesterol (mg/dl) | Integer |
| fbs | Fasting blood sugar > 120 mg/dl (0 = No, 1 = Yes) | Binary |
| restecg | Resting electrocardiographic results (0-2) | Integer |
| thalach | Maximum heart rate achieved | Integer |
| exang | Exercise-induced angina (0 = No, 1 = Yes) | Binary |
| oldpeak | ST depression induced by exercise | Float |
| slope | Slope of the peak exercise ST segment (0-2) | Integer |
| ca | Number of major vessels (0-4) | Integer |
| thal | Thalassemia (0-3) | Integer |

### Target Variable
- **1**: Defective Heart (Heart Disease Present)
- **0**: Healthy Heart (No Heart Disease)

### Data Distribution
- Records with Heart Disease: 165 (54.46%)
- Healthy Records: 138 (45.54%)

## 🔧 Installation & Setup

### Prerequisites
- Python 3.7 or higher
- pip (Python package manager)

### Step 1: Clone the Repository
```bash
git clone https://github.com/nisaabbas183-sys/DevelopersHub-Coporation.git
cd DevelopersHub-Coporation/task1
```

### Step 2: Install Required Libraries
```bash
pip install -r requirements.txt
```

### Step 3: Prepare the Data
Ensure you have the `heart.csv` file in the same directory as the notebook.

### Step 4: Run the Notebook
```bash
jupyter notebook "Heart Disease Prediction.ipynb"
```

## 📈 Project Workflow

### 1. **Importing Dependencies**
   - NumPy for numerical operations
   - Pandas for data manipulation
   - scikit-learn for machine learning algorithms

### 2. **Data Collection and Processing**
   - Load CSV data into a Pandas DataFrame
   - Display first and last 5 rows
   - Check dataset shape: (303, 14)
   - Verify data types and integrity
   - Check for missing values (None found)

### 3. **Exploratory Data Analysis (EDA)**
   - Generate descriptive statistics
   - Analyze target variable distribution
   - Understand feature ranges and distributions

### 4. **Data Preprocessing**
   - Split features (X) and target (Y)
   - X: 303 rows × 13 features
   - Y: 303 target values

### 5. **Train-Test Split**
   - Training Set: 242 samples (80%)
   - Test Set: 61 samples (20%)
   - Uses stratification to maintain class distribution
   - Random state: 2 (for reproducibility)

### 6. **Model Training**
   - Algorithm: Logistic Regression
   - Solver: lbfgs (default)
   - No feature scaling applied

### 7. **Model Evaluation**
   - **Training Accuracy**: 85.12%
   - **Testing Accuracy**: 81.97%
   - Model shows consistent performance (no significant overfitting)

### 8. **Predictive System**
   - Example prediction with custom input
   - Real-time classification for new patients

## 📊 Model Performance

| Metric | Value |
|--------|-------|
| Training Accuracy | 85.12% |
| Testing Accuracy | 81.97% |
| Total Samples | 303 |
| Training Samples | 242 |
| Testing Samples | 61 |

## 🔮 Example Prediction

### Input Data:
```python
Age: 62, Sex: 0, CP: 0, TrestBPS: 140, Chol: 268, FBS: 0,
RestECG: 0, Thalach: 160, Exang: 0, Oldpeak: 3.6, Slope: 0, CA: 2, Thal: 2
```

### Prediction Output:
```
The Person does not have a Heart Disease
```

## 📁 Project Files

- `Heart Disease Prediction.ipynb` - Main Jupyter notebook with complete implementation
- `requirements.txt` - Python package dependencies
- `README.md` - Project documentation
- `heart.csv` - Dataset (required for running the notebook)

## 💡 Key Insights

1. **Class Balance**: Dataset has relatively balanced classes (54% vs 46%)
2. **Model Performance**: ~82% accuracy on test data indicates a reliable model
3. **Generalization**: Similar accuracy on training and test data shows good generalization
4. **Interpretability**: Logistic Regression provides interpretable probability scores

## 🚀 Future Enhancements

- Implement feature scaling (StandardScaler, MinMaxScaler)
- Try alternative algorithms (Random Forest, SVM, Neural Networks)
- Perform hyperparameter tuning
- Add cross-validation
- Create feature importance analysis
- Build a web interface for predictions
- Generate confusion matrix and classification reports

## ⚠️ Important Notes

- The model requires exactly 13 input features in the correct order
- Input features should be numerical values
- Feature values should be within the ranges observed in the training data
- Model is for educational purposes and should not be used for actual medical diagnosis

## 📚 Libraries Used

- **NumPy** (1.24.3) - Numerical computing
- **Pandas** (2.0.3) - Data manipulation and analysis
- **scikit-learn** (1.3.0) - Machine learning algorithms
- **Jupyter** (1.0.0) - Interactive notebook environment

## 👨‍💻 Author

Nisa Abbas  
GitHub: [@nisaabbas183-sys](https://github.com/nisaabbas183-sys)

## 📄 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check [issues page](https://github.com/nisaabbas183-sys/DevelopersHub-Coporation/issues).

## 📞 Support

If you have any questions or need help, please open an issue on GitHub.

---

**Last Updated**: April 27, 2026
