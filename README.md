# Custom Linear Regression from Scratch: Agriculture Crop Yield Analysis

## Project Overview
This project builds a **custom Linear Regression model from scratch** using NumPy, pandas, and matplotlib to predict maize crop yield.
Unlike standard implementations that use `sklearn.linear_model`, this project manually implements:
* **Hypothesis Function:** $h_\theta(x) = \theta \cdot x + b$
* **Cost Function:** Mean Squared Error (MSE) using the formula $J(\theta, b) = \frac{1}{2n} \sum_{i=1}^{n} (h_\theta(x^{(i)}) - y^{(i)})^2$.
* **Vectorized Gradient Descent:** Utilizing NumPy transpositions (`X.T`) and dot products to update weights ($\theta$) and bias ($b$) simultaneously across all training examples.
* **Feature Scaling:** Z-score normalization (Standardization) to ensure Gradient Descent stability.

## Dataset
[Dataset on Kaggle](https://www.kaggle.com/datasets/akshatgupta7/crop-yield-in-indian-states-dataset))
The dataset (`crop_yield.csv`) contains crop production records across Indian states, seasons, and years. After filtering for **Maize** crops only:
- **Total samples:** 975 rows
- **Features used:** Annual Rainfall(mm), Fertilizer(kg), Pesticide (kg), Area cultivated (ha)
- **Target variable:** Yield (production per unit area) (metric tons per ha)
- 
## Visualizations
The notebook includes:
1. **Scatter Plots**
2. **Cost History** – How MSE decreased (or didn't decrease) over gradient descent iterations
3. **Comparison Table** – Actual vs Predicted yields with error metrics

## Libraries Used
- Python 3.x
- pandas – Data loading and filtering
- numpy – Array operations and math
- matplotlib – Visualizations
- scikit-learn – Only for train_test_split, scaling and evaluation metrics (not for the model itself)
- Seaborn- to gain deeper insights into the data distribution and feature relationships:

## How to Run This Project
### Before You Start: Install What You Need
If you haven't already, download and install these first:
| Software | Download Link | Why You Need It |
|----------|---------------|-----------------|
| **Git** | [git-scm.com/downloads](https://git-scm.com/downloads) | To clone the repository |
| **Anaconda** | [anaconda.com/download](https://www.anaconda.com/download) | To run Jupyter Notebook |

> **Installation tips:** For both installers, just click "Next" and keep the default options. Anaconda takes a few minutes — that's normal.
### Step-by-Step Instructions
#### Step 1: Open Command Prompt
| Action | How To |
|--------|--------|
| Press | `Windows + R` on your keyboard |
| Type | `cmd` |
| Click | `OK` or press `Enter` |
**You'll see a black window like this:**
```cmd
C:\Users\YourName>

#Step 2: Clone the Repository
> **Important:** Replace `YOUR_USERNAME` with your actual GitHub username
**Type this command exactly:**
git clone https://github.com/YOUR_USERNAME/Linear-Regression-on-Agricultural-Data-Maize-Yield-Prediction.git

#Step 3: Enter into Folder
cd Linear-Regression-on-Agricultural-Data-Maize-Yield-Prediction

you will then obtain the actual code for this project

#Step 4:Launch Jupyter Notebook
jupyter notebook

If you found this project useful, please consider giving it a ⭐

