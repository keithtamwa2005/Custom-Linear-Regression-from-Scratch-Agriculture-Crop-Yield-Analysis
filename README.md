# Custom Linear Regression from Scratch: Agriculture Crop Yield Analysis

## Project Overview

This project builds a **custom Linear Regression model from scratch** using NumPy, pandas, and matplotlib to predict maize crop yield. No scikit-learn linear models were used — everything from gradient descent to cost calculation was implemented manually. However we only used sklearn to access the metrics at the end

## Dataset
[Dataset on Kaggle](https://www.kaggle.com/datasets/akshatgupta7/crop-yield-in-indian-states-dataset))
The dataset (`crop_yield.csv`) contains crop production records across Indian states, seasons, and years. After filtering for **Maize** crops only:
- **Total samples:** 975 rows
- **Features used:** Annual Rainfall(mm), Fertilizer(kg), Pesticide (kg), Area cultivated (ha)
- **Target variable:** Yield (production per unit area) (metric tons per ha)

## What was Built?
| Component | Implementation |
| Linear Regression | Custom class with gradient descent |
| Cost Function | Mean Squared Error (MSE) |
| Optimization | Gradient descent with configurable learning rate |
| Evaluation | MAE, MSE, RMSE, R² Score |
| Visualization | Matplotlib for scatter plots and learning curves |

## Key Results
| Metric | Value |
| R² Score | **-2.08** |
| Mean Absolute Error (MAE) | ~2.00 |
| Root Mean Squared Error (RMSE) | ~2.83 |

### What Does Negative R² Mean for this simple case?
> An R² score below 0 means the model performs worse than simply predicting the **mean yield value** for every sample.
This is a valuable diagnostic result — it proves that:
- Yield has a **non-linear** relationship with the given features
- Important factors (soil quality, temperature, irrigation) are missing
- More complex models (random forests, polynomial regression) are needed

## Visualizations
The notebook includes:
1. **Scatter Plot** – Fertilizer usage vs Yield (log scale)
2. **Cost History** – How MSE decreased (or didn't decrease) over gradient descent iterations
3. **Comparison Table** – Actual vs Predicted yields with error metrics

## Technologies Used
- Python 3.x
- pandas – Data loading and filtering
- numpy – Array operations and math
- matplotlib – Visualizations
- scikit-learn – Only for train_test_split, scaling and evaluation metrics (not for the model itself)

## How to Run This Project
**Before You Start: Install What You Need
If you haven't already, download and install these first:
Git – git-scm.com/downloads (click "Download for Windows", run installer with default options)

Anaconda – anaconda.com/download (download the Windows installer, run it)**

**Step-by-Step Command Prompt Instructions

Step 1: Open Command Prompt
Press Windows + R on your keyboard (Windows only)
Type cmd in the box that appears
Press Enter or click "OK"
You'll see a black window

**Step 2: Clone the Repository
Type this command (replace YOUR_USERNAME with your actual GitHub username):
git clone https://github.com/YOUR_USERNAME/Linear-Regression-on-Agricultural-Data-Maize-Yield-Prediction.git

**Step 3: Enter the Project Folder
Type this and press Enter:
cd Linear-Regression-on-Agricultural-Data-Maize-Yield-Analysis

**Step 4: Launch Jupyter Notebook
Type this and press Enter:
cmd
jupyter notebook
