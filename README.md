
## Dataset Analysis and Preprocessing

### Overview
This project involves analyzing a dataset sourced from Kaggle, where the target variable is imbalanced. The dataset consists of features related to infants' birth conditions. The primary goals are:
1. **Exploratory Data Analysis (EDA)** to understand the data distribution.
2. **Balancing the Dataset** to address class imbalance.
3. **Splitting Data** for model training and testing.

---

### Steps Implemented

#### 1. Exploratory Data Analysis (EDA) and Preprocessing
- **Class Distribution**:
  - The target variable (`smoke`) was found to be imbalanced.
  - A bar plot was created to visualize the class distribution.
- **Normalization**:
  - Numerical features (`bwt`, `gestation`, `age`, `height`, `weight`) were normalized using Min-Max Scaling.
  - Missing values were handled using mean imputation for numerical columns.

#### 2. Dataset Balancing
- **Technique**: Synthetic Minority Oversampling Technique (SMOTE) was used to balance the class distribution.
- **Results**:
  - Before Balancing: Imbalanced class distribution was observed.
  - After Balancing: The dataset was successfully balanced.

#### 3. Data Splitting
- The dataset was split into **training** (80%) and **testing** (20%) sets using `train_test_split` from Scikit-Learn.
- Stratification ensured proportional class representation in both sets.

---

### Usage
1. Clone the repository or download the dataset file `babies.csv`.
2. Install required Python libraries:
   ```bash
   pip install pandas matplotlib scikit-learn imbalanced-learn
   ```
3. Run the Python script for analysis and preprocessing.

---

### Results
- The dataset is now balanced and ready for training predictive models.
- Preprocessing ensures high data quality for machine learning tasks.

---
