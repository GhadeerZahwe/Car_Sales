# Car Price Prediction using Machine Learning

## Project Overview
This project aims to predict car prices based on various features such as make, color, odometer reading, number of doors, and more. It explores different regression models, including Ridge Regression and Random Forest Regressor, with a focus on hyperparameter tuning to improve performance.

---

## Dataset
The dataset contains information about various car listings, including:

- **Make**: Brand of the car (e.g., Honda, Toyota)  
- **Colour**: Color of the car  
- **Odometer (KM)**: Distance traveled by the car in kilometers  
- **Doors**: Number of doors  
- **Price**: Target variable (car price)  

Data cleaning involved removing rows with missing `Price` values to ensure data integrity.

---

## Feature Engineering & Preprocessing
- Removed rows with missing `Price` values.  
- Handled missing data with **imputation techniques**.  
- Encoded categorical variables using **One-Hot Encoding**.  
- Scaled numerical features where necessary.  
- Built **preprocessing pipelines** for reproducibility.  

---

## Models Used
We experimented with several regression models using Scikit-Learn:

- **Ridge Regression** – A linear model with L2 regularization.  
- **Support Vector Regressor (SVR, kernel="linear")** – Fits a linear regression line using support vectors.  
- **Support Vector Regressor (SVR, kernel="rbf")** – Uses a radial basis function kernel for non-linear regression.  
- **Random Forest Regressor** – An ensemble method combining many decision trees for more robust predictions.  

Each model was built into a preprocessing + modeling **Pipeline**, trained on the car sales dataset, and evaluated using the **R² score**. Ridge was also further evaluated with **MAE, MSE, and R²**.

---

## Evaluation Metrics
- **R² Score** – measures the proportion of variance explained by the model.  

---


## Setup & Installation
1. **Clone the repository**
```bash
git clone https://github.com/GhadeerZahwe/Car_Sales.git
cd Car_Sales
```
2. **Create & activate a virtual environment**
```bash
# On Linux/Mac
python -m venv carsales
source carsales/bin/activate

# On Windows (PowerShell)
python -m venv carsales
.\carsales\Scripts\activate
```
