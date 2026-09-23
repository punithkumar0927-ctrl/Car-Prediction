# 🚗 Car Price Prediction Using Machine Learning

## 📌 Project Overview

Car Price Prediction is a machine-learning regression project that predicts the price of a car based on its technical specifications and features.

The project uses the `CarPrice_Assignment.csv` dataset and compares multiple regression algorithms to identify a suitable model for predicting car prices. It includes data cleaning, exploratory data analysis, categorical encoding, model training, performance evaluation, and prediction for new vehicles.

## 🎯 Objectives

- Analyze car-related data using Python.
- Clean and preprocess the dataset.
- Explore relationships between vehicle features and price.
- Convert categorical features into numerical values.
- Train multiple machine-learning regression models.
- Compare model performance using evaluation metrics.
- Predict the estimated price of a new car.
- Save the trained model for future predictions.

## 📂 Dataset

The project uses the `CarPrice_Assignment.csv` dataset. It contains information about cars, their technical specifications, fuel economy, and market price.

### Important Features

| Feature | Description |
|---|---|
| `car_ID` | Unique identification number of the car |
| `symboling` | Insurance risk rating |
| `CarName` | Name and manufacturer of the car |
| `fueltype` | Fuel type, such as gas or diesel |
| `aspiration` | Aspiration type |
| `doornumber` | Number of doors |
| `carbody` | Type of car body |
| `drivewheel` | Drive-wheel configuration |
| `enginelocation` | Engine location |
| `wheelbase` | Distance between the front and rear axles |
| `carlength` | Length of the car |
| `carwidth` | Width of the car |
| `carheight` | Height of the car |
| `curbweight` | Weight of the car without passengers or luggage |
| `enginetype` | Type of engine |
| `cylindernumber` | Number of engine cylinders |
| `enginesize` | Engine displacement size |
| `fuelsystem` | Fuel-delivery system |
| `horsepower` | Engine horsepower |
| `peakrpm` | Maximum engine revolutions per minute |
| `citympg` | Fuel efficiency in city driving |
| `highwaympg` | Fuel efficiency on highways |
| `price` | Target variable representing car price |

## 🔍 Exploratory Data Analysis

The project explores the relationship between car specifications and price using:

- Correlation analysis.
- Distribution plots.
- Scatter plots.
- Box plots.
- Categorical-feature comparison.
- Outlier analysis.
- Price comparison by fuel type and car body.
- Horsepower, engine-size, and mileage analysis.

Important observations may include:

- Engine size and horsepower can strongly influence car price.
- Heavier and larger vehicles may have higher prices.
- Highway and city mileage can show an inverse relationship with engine performance.
- Luxury manufacturers may have higher average prices.
- Some categorical features require encoding before model training.

## 🧹 Data Preprocessing

The following preprocessing steps are performed:

1. Load the dataset.
2. Inspect columns and data types.
3. Check for missing values.
4. Remove unnecessary identifier columns.
5. Extract useful information from `CarName`.
6. Convert categorical values into numerical values.
7. Separate input features and target variable.
8. Split the data into training and testing sets.
9. Scale numerical features when required.
10. Prepare the data for machine-learning models.

## 🤖 Machine-Learning Workflow

```text
Load dataset
     ↓
Understand data structure
     ↓
Clean and preprocess data
     ↓
Perform exploratory data analysis
     ↓
Encode categorical features
     ↓
Split data into training and testing sets
     ↓
Train regression models
     ↓
Evaluate model performance
     ↓
Compare algorithms
     ↓
Save the best model
     ↓
Predict the price of a new car
```

## 🧠 Models Compared

The project can compare the following regression algorithms:

- Linear Regression
- Ridge Regression
- Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor

The final model should be selected based on test-set performance and not only training accuracy.

## 📏 Evaluation Metrics

The models are evaluated using:

- Mean Absolute Error, or MAE
- Mean Squared Error, or MSE
- Root Mean Squared Error, or RMSE
- \(R^2\) score

A lower MAE and RMSE indicate smaller prediction errors. A higher \(R^2\) score indicates that the model explains more variation in car prices.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Google Colab
- Jupyter Notebook

## 📁 Project Structure

```text
car-price-prediction/
│
├── CarPrice_Assignment.csv       # Dataset
├── car_price_prediction.ipynb    # Main analysis notebook
├── model.pkl                     # Saved trained model
├── requirements.txt              # Python dependencies
├── README.md                     # Project documentation
└── .gitignore                    # Ignored files
```

## 💻 Installation

### Prerequisites

Install the following:

- Python 3.9 or above
- pip
- Git
- Jupyter Notebook or Google Colab

### 1. Clone the Repository

```bash
git clone [https://github.com/punithkumar0927-ctrl/car-price-prediction.git](https://github.com/punithkumar0927-ctrl/car-price-prediction.git)
```

### 2. Navigate to the Project Directory

```bash
cd car-price-prediction
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
car_price_prediction.ipynb
```

You can also upload the notebook and dataset to Google Colab.

## ▶️ Usage

Run the notebook cells in the following order:

1. Import libraries.
2. Load `CarPrice_Assignment.csv`.
3. Inspect and clean the data.
4. Perform exploratory data analysis.
5. Encode categorical columns.
6. Split the dataset.
7. Train the regression models.
8. Compare model metrics.
9. Select the best-performing model.
10. Save the model using Joblib.
11. Enter new car specifications.
12. Generate the estimated car price.

Example model-saving code:

```python
import joblib

joblib.dump(best_model, "model.pkl")
```

Example model-loading code:

```python
import joblib

model = joblib.load("model.pkl")
prediction = model.predict(new_car_data)
```

## 📊 Results

Add your actual model results below after running the notebook.

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | Add result | Add result | Add result |
| Ridge Regression | Add result | Add result | Add result |
| Lasso Regression | Add result | Add result | Add result |
| Decision Tree Regressor | Add result | Add result | Add result |
| Random Forest Regressor | Add result | Add result | Add result |
| Gradient Boosting Regressor | Add result | Add result | Add result |

### Best Model

```text
Best model: Add model name
Test MAE: Add value
Test RMSE: Add value
Test R² score: Add value
```

Do not add invented accuracy or \(R^2\) values. Replace the placeholders with the results produced by your notebook.

## 🔮 Future Improvements

- Build a web interface using Streamlit or Flask.
- Add a form for entering new-car specifications.
- Deploy the prediction application online.
- Add cross-validation.
- Perform hyperparameter tuning.
- Use logarithmic transformation for highly skewed prices.
- Add manufacturer-level analysis.
- Add explainable-AI visualizations.
- Include newer vehicle datasets.
- Compare predictions with current market prices.

## ⚠️ Limitations

- Predictions depend on the quality and size of the dataset.
- The dataset may not represent current market prices.
- Vehicle prices can change according to location, condition, mileage, demand, and model year.
- The model should be used for educational and analytical purposes.
- Predictions are estimates and should not be treated as official vehicle valuations.

## 📸 Screenshots

Add screenshots of your analysis and results here:

```markdown




```

## 👨‍💻 Author

**Punith Kumar**

- GitHub: [@punithkumar0927-ctrl](https://github.com/punithkumar0927-ctrl)
- Portfolio: Add your portfolio link
- LinkedIn: Add your LinkedIn profile link

## ⭐ Acknowledgement

This project was created for learning and demonstrating the use of Python, data analysis, and machine-learning regression techniques.

---

⭐ If you found this project useful, consider giving the repository a star.
