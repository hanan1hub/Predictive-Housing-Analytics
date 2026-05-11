# Predictive Housing Analytics: Custom Linear Regression & Gradient Descent

## 📌 Project Overview
This repository features a custom implementation of a Linear Regression model built entirely from scratch using Python and NumPy. Moving beyond high-level machine learning APIs, this project demonstrates a strong grasp of fundamental supervised learning algorithms by manually implementing gradient descent and L2 regularization to predict California housing prices. This end-to-end pipeline is structured with software development best practices in mind, efficiently handling data processing, mathematical optimization, and model evaluation.

**Author:** Hanan Majeed

## 📊 Dataset
* **Source:** California Housing Dataset (`housing.csv`)
* **Features Selected:** `housing_median_age`, `total_rooms`, `population`
* **Target Variable:** `median_house_value`

## 🚀 Core Features & Methodology

### 1. Data Preprocessing & Scaling
* Engineered a clean data pipeline to ingest the data and perform a reproducible 80/20 train-validation split.
* Normalized feature columns using **Min-Max Scaling** to ensure stable and efficient convergence during the gradient descent optimization process.

### 2. Mathematical Implementation (From Scratch)
* **Cost Function:** Formulated the mean squared error cost function to calculate training and cross-validation errors, integrating an L2 regularization penalty (`lambd`) to prevent overfitting.
* **Gradient Descent Optimizer:** Developed a custom gradient descent algorithm that computes partial derivatives for feature weights and bias iteratively, updating them to minimize the cost function.

### 3. Model Training & Evaluation
* Executed a full training loop over 1,000 epochs.
* Continuously tracked and evaluated training versus validation loss to monitor model health and generalization capabilities.
* Generated convergence curves using Matplotlib to visually validate the learning process.

### 4. Hyperparameter Tuning Pipeline
* Designed a systematic evaluation function to test multiple distinct learning rates (`alpha`) and regularization strengths.
* Conducted experiments demonstrating that a learning rate of `0.01` yielded excellent, stable convergence without erratic fluctuations, while regularization values up to `1.0` maintained strong generalization to unseen data.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Core Libraries:** NumPy (Matrix operations & Calculus), Pandas (Data handling)
* **Visualization:** Matplotlib
* **Utilities:** Scikit-learn (Utilized solely for the initial train-test split and Min-Max scaling)

## ⚙️ Local Setup & Installation

1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/hanan1hub/Predictive-Housing-Analytics.git](https://github.com/hanan1hub/Predictive-Housing-Analytics.git)
    ```
 2.Navigate to the project directory:

 ```Bash
cd Predictive-Housing-Analytics
```
3. Install the required dependencies:
 
```Bash
pip install numpy pandas matplotlib scikit-learn
```
4. Ensure the housing.csv dataset is located in the root directory.

5. Launch the Jupyter Notebook environment to run the pipeline:

```Bash
jupyter notebook california_housing_regression.ipynb
```
(Note: Ensure your notebook file is named california_housing_regression.ipynb or replace this command with your specific filename).

🤝 Contributing
Contributions, optimizations, and feedback are highly encouraged. Please feel free to open an issue or submit a pull request if you have suggestions for improving the optimization algorithm or data pipeline.
