# Employee Burnout Analysis and Prediction

This project focuses on analyzing and predicting employee burnout using a dataset. The primary objective is to understand the key factors contributing to burnout and develop a predictive model for identifying burnout levels.

## Features
- **Data Cleaning and Preprocessing**: Handle missing values, encode categorical variables, and scale numerical features.
- **Exploratory Data Analysis (EDA)**: Visualize feature importance and model performance.
- **Burnout Prediction**: Use a Random Forest Regressor to predict the "Burn Rate" for employees.
- **Interactive User Input**: Predict burnout for custom user inputs.

## Dataset
The dataset contains the following key columns:
- `Employee ID`
- `Date of Joining`
- `Gender`
- `Company Type`
- `WFH Setup Available`
- `Designation`
- `Resource Allocation`
- `Mental Fatigue Score`
- `Burn Rate` (target variable)

### Handling Missing Values
- **Resource Allocation** and **Mental Fatigue Score**: Filled with their respective means.
- **Burn Rate**: Filled with its median.

## Prerequisites
Install the required Python libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## How to Use
### Step 1: Clone the Repository
```bash
git clone https://github.com/your-repo/employee-burnout-analysis.git
cd employee-burnout-analysis
```

### Step 2: Add Dataset
Place your dataset (`Employee_burnout_analysis-AI_2.csv`) in the project directory.

### Step 3: Run the Code
Execute the Python script:
```bash
python burnout_analysis.py
```

### Step 4: Predict Burnout for Custom Input
The script will prompt you to enter employee details (e.g., Gender, Company Type, Resource Allocation, etc.). Based on the input, it will predict the burnout rate.

## Code Highlights
### Training and Evaluation
- A Random Forest Regressor is used to predict the burnout rate.
- The model achieves high accuracy with metrics such as:
  - **Mean Absolute Error (MAE)**
  - **Root Mean Squared Error (RMSE)**
  - **R² Score**

### Visualization
- **Feature Importance**: Bar plot showing which features contribute most to burnout prediction.
- **Prediction vs. Actual**: Scatter plot comparing predicted and actual burnout rates.

### Interactive Prediction
- Enter custom employee details via the console to predict burnout levels.

## Output
1. **Model Evaluation Metrics**:
   - MAE
   - RMSE
   - R² Score

2. **Visualizations**:
   - Feature importance plot
   - Prediction vs. actual scatter plot

3. **Interactive Prediction**:
   - Predicted burnout rate for user-input employee details.

## Example Input for Prediction
```plaintext
Enter the following details for prediction:
Gender (Male/Female): Male
Company Type (Product/Service): Service
WFH Setup Available (Yes/No): Yes
Designation (1 to 5): 3
Resource Allocation (1 to 10): 7.5
Mental Fatigue Score (0 to 10): 6.8
```

### Example Output
```plaintext
Predicted Burn Rate: 0.4675
```

## Contributing
Contributions are welcome! If you have ideas for improvements, feel free to fork the repository and submit a pull request.
