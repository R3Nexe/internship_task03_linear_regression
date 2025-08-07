# Housing Price Prediction - Linear Regression Model

This model focusses on predicting house prices

## Project Workflow

### 1. Data Cleaning and Preprocessing

- dropped illogical entries (e.g., 5-bedroom homes with very low prices).
- Converted categorical and boolean columns to integer/binary values.
- Applied one-hot encoding to categorical columns like 'furnishing_status'.
### 2. Feature Engineering

- Added custom features to improve the model, such as:
  - Area per bedroom
  - Area per Bathroom
- Removed features that were redundant or strongly multicollinear.
- Handled outliers

### 3. Feature Scaling

- Scaled all numerical features using 'StandardScaler'.

### 4. Model Training

- Trained a 'LinearRegression' model using scikit-learn.
- Evaluated performance using:
  - **MAE (Mean Absolute Error)**
  - **MSE (Mean Squared Error)**
  - **R² Score**

### 5. Model Evaluation

- After feature engineering and scaling:
  - **MAE**: ~₹726,000
  - **MSE**: ~₹8.77 × 10¹¹
  - **R²**: 0.771
