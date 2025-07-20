🏡 Housing Price Prediction – MLOps Project
This repository presents a complete machine learning workflow for predicting house prices using the Boston Housing dataset. It highlights modular code development, regression modeling, hyperparameter optimization, and CI/CD implementation via GitHub Actions—executed as part of an academic MLOps assignment.

📁 Project Structure

HousingRegression/
├── .github/workflows/ci.yml       # GitHub Actions workflow for CI
├── regression.py                  # Main script to train and evaluate models
├── utils.py                       # Utility functions for data handling and modeling
├── requirements.txt               # Python package dependencies
├── README.md                      # Project documentation


🔧 Environment Setup
Set up a clean Conda environment and install all dependencies:
  conda create -n houseprice python=3.10 -y
  conda activate houseprice
  pip install -r requirements.txt


🗂️ Dataset
This project uses the Boston Housing dataset. Since it is deprecated in scikit-learn, it is manually fetched from:
📎 http://lib.stat.cmu.edu/datasets/boston
The load_data() function in utils.py takes care of loading and preprocessing the data.


🧮 Models Implemented
In the reg branch:
  Linear Regression
  Ridge Regression
  Lasso Regression

In the hyper branch:
The same models enhanced with hyperparameter tuning via GridSearchCV
📈 Evaluation Metrics
Each model is evaluated using:
  Mean Squared Error (MSE)
  R² Score (Coefficient of Determination)


🚀 Running the Project
Execute the following command to train and evaluate the models:
python regression.py
This will display the performance metrics for each model on the console.


🤖 CI/CD with GitHub Actions
Each push to the reg or hyper branches automatically triggers the CI pipeline (ci.yml), which:
Sets up Python 3.10
Installs required packages
Runs regression.py to verify model functionality
You can monitor the pipeline under the Actions tab of the repository.


🌿 Branch Overview
Branch	Description
main	Final integrated project
reg	Baseline regression models without tuning
hyperb	Models with hyperparameter tuning implemented


📦 Deliverables
Clean, modular code (regression.py, utils.py)
Dependency list in requirements.txt
CI pipeline integrated via GitHub Actions
Fully reproducible Conda environment
Evaluation reports for both baseline and tuned models


📬 Contact
For academic queries, feel free to reach out:
Sree Charan
g24ai10295@iitj.ac.in
