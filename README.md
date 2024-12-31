![image](https://github.com/user-attachments/assets/a6ecf9d0-7811-442f-8fe0-2efbc885c927)



<h1 align="center"> 🌡️ Time Series Forecasting with Amazon Chronos 🌡️</h1>

<p align="center">
  <strong>A comprehensive Python application for time series forecasting using Amazon Chronos and a multi-site air quality dataset.</strong>
</p>

<p align="center">
  <a href="https://github.com/yourusername/yourrepository">
    <img src="https://img.shields.io/github/license/its-amann/Amazon-Chrones-Model.svg" alt="License">
  </a>
  <a href="https://github.com/yourusername/yourrepository/issues">
    <img src="https://img.shields.io/github/issues/its-amann/Amazon-Chrones-Model.svg" alt="Issues">
  </a>
  <a href="https://github.com/yourusername/yourrepository/stargazers">
    <img src="https://img.shields.io/github/stars/its-amann/Amazon-Chrones-Model.svg" alt="Stars">
  </a>
</p>

---

## 🚀 Overview

Welcome to the **Time Series Forecasting project**, a robust and analytical tool designed for predicting future values in time-dependent data. This project utilizes the **Amazon Chronos** library, a powerful time series forecasting framework, along with a multi-site air quality dataset from Beijing. It's ideal for anyone looking to understand, analyze, and predict time series data efficiently.

✨ **Key Highlights:**

-   **Advanced Forecasting:** Leverages Amazon Chronos for accurate time series predictions.
-   **Comprehensive Data Analysis:** Includes exploratory data analysis to understand the data patterns.
-   **Cross-Validation:** Implements cross-validation techniques for robust model evaluation.
-   **Parameter Tuning:** Features a parameter tuning module to optimize model performance.
-   **Visualization:** Generates clear visualizations for both data exploration and forecast evaluation.

---

## 🛠 Features

-   **Data Loading & Cleaning:** Imports and processes a multi-site air quality dataset.
-   **Exploratory Data Analysis (EDA):** Visualizes data patterns, including hourly, monthly, and quarterly seasonality.
-   **Amazon Chronos Integration:** Utilizes pre-trained Amazon Chronos models for forecasting.
-   **Cross-Validation:** Evaluates model robustness using time series cross-validation.
-   **Hyperparameter Tuning:** Optimizes model performance through parameter grid search.
-   **Future Prediction:** Forecasts future time steps using the best-tuned model.
-   **Visualizations:** Plots actual data alongside predictions for easy comparison.
-   **Error Metrics:** Calculates and displays RMSE to assess prediction accuracy.

---

## 📸 Screenshots

![image](https://github.com/user-attachments/assets/2aac59af-d46c-4c60-98a7-ac3b54793ec7)
<p align="center">
  <font size="6">
    Hourly temperature data plot.
  </font>
</p>

![image](https://github.com/user-attachments/assets/4e8e76e7-a88d-4531-9333-119bf86e409d)

<p align="center">
  <font size="6">
    Monthly seasonality of temperature, red lines represent monthly means.
  </font>
</p>

![image](https://github.com/user-attachments/assets/13aeac85-3e82-483b-82a7-55e1ea508cb4)

<p align="center">
  <font size="6">
    Quarterly seasonality of temperature data.
  </font>
</p>

![image](https://github.com/user-attachments/assets/6792ae31-570f-43a4-b75b-67b843f7d9ce)

<p align="center">
  <font size="6">
  First cross-validation, Actual vs. Predicted values.
  </font>
</p>

![image](https://github.com/user-attachments/assets/770e674e-90af-40ea-9810-0a4aaae6e537)

<p align="center">
  <font size="6">
  Second cross-validation, Actual vs. Predicted values.
  </font>
</p>


![image](https://github.com/user-attachments/assets/625ae209-78bc-4a6c-a240-cc6f21ba43fc)

<p align="center">
  <font size="6">
  Fourth cross-validation, Actual vs. Predicted values.
  </font>
</p>

![image](https://github.com/user-attachments/assets/c5d7b8f2-4ce3-492c-bc03-08c237295646)

<p align="center">
  <font size="6">
  Fifth cross-validation, Actual vs. Predicted values.
  </font>
</p>




![image](https://github.com/user-attachments/assets/02d21ffa-ba04-4edb-88fb-12512789f3b4)

<p align="center">
  <font size="6">
  Tenth cross-validation, Actual vs. Predicted values.
  </font>
</p>

![image](https://github.com/user-attachments/assets/95d3cbe3-ca21-43ee-9192-79b5a6bf3ca8)

<p align="center">
    <font size="6">
   Final forecast plot with tuned model parameters, Actual vs. Predicted values.
  </font>
</p>
---

## 🔧 Installation

### Prerequisites

-   **Python 3.x** installed on your machine. [Download Python](https://www.python.org/downloads/)
-   **pip** package installer.
-   **git** for cloning the repository

### Steps

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/yourusername/yourrepository.git
    cd your-repository
    ```

2.  **Install Dependencies:**
    ```bash
    pip install -q git+https://github.com/amazon-science/chronos-forecasting.git
    pip install -q tsdb
    pip install pandas
    pip install matplotlib
    pip install statsmodels
    pip install scikit-learn
    pip install numpy
    pip install torch
    ```

3.  **Run the Application:**
    ```bash
    python your_script_name.py
    ```

---

## 💻 Usage

The script will automatically execute the following steps:

1.  **Data Import:** Loads the multi-site air quality dataset from the `tsdb` library.
2.  **Data Preprocessing:** Cleans and prepares the data for analysis, including creating a datetime index.
3.  **Exploratory Data Analysis:** Generates plots to visualize hourly, monthly, and quarterly temperature data patterns.
4.  **Model Initialization:** Initializes the Amazon Chronos forecasting model.
5.  **Initial Forecast:** Generates an initial forecast using default parameters.
6.  **Cross-Validation:** Evaluates the model performance using time series cross-validation, printing RMSE values for each fold.
7.  **Cross-Validation Visualization:** Plots cross-validation forecasts against actual values for all validation folds.
8.  **Parameter Tuning:** Conducts a grid search to identify the optimal model parameters.
9.   **Best Model:** Exports the best hyper parameters for future use.
10. **Final Forecast:**  Generates a forecast with the best parameters and visualizes the final forecast against the actuals.

### Code Details
-  **Libraries** 
     - `pandas` : For data manipulation and analysis.
    - `matplotlib` :  For data visualization.
    - `statsmodels` : For time series analysis plots like month_plot and quarter_plot.
    - `sklearn` : For model evaluation metrics such as mean_absolute_error, mean_squared_error, etc.
    - `numpy` :  For numerical operations.
    - `tsdb` : To load the dataset.
    - `chronos` : Amazon Chronos for time series forecasting.
     -`datetime` : For creating date time variables.
     -`torch` :  Deep learning library used for Chronos model.

-  **Data Loading and Preprocessing** 
    -  The script loads air quality data from multiple sites in Beijing, using the `tsdb` library.
    -  It converts date and time columns into a datetime format and set it as the index of the dataframe.
    -  The script focuses specifically on the `TEMP` column (renamed to `y`) from the 'Wanliu' station for analysis.

-  **Exploratory Data Analysis (EDA)**
     -  The script visualizes the time series data at hourly, monthly, and quarterly intervals to reveal trends and patterns.

-  **Amazon Chronos Model**
    - A ChronosPipeline model is instantiated using a pre-trained model from "amazon/chronos-t5-base".
    - It demonstrates how to get predictions for the time series data.

-  **Cross-Validation**
    -  The script implements time series cross-validation to evaluate the model's predictive capability by splitting the data into several train/test folds and evaluates the RMSE in each fold.

-  **Parameter Tuning**
   - The script defines a grid of hyperparameters (temperature, top_k, top_p, num_samples) to tune the Chronos model using ParameterGrid from Scikit-learn.
   - It performs cross-validation for each combination of parameters to find the optimal configuration based on the RMSE.

-  **Final Prediction**
     -  Using the best parameters from the tuning process, the script performs a final forecast on the entire time series.

-   **Visualizations:**
    - Actual vs. predicted values plots, for both cross validation folds and the final forecast are plotted using the `matplotlib` library.
---

## 🤝 Contributing

1.  **Fork the Project**
2.  **Create your Feature Branch:** `git checkout -b feature/AmazingFeature`
3.  **Commit your Changes:** `git commit -m 'Add some AmazingFeature'`
4.  **Push to the Branch:** `git push origin feature/AmazingFeature`
5.  **Open a Pull Request**

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 🙏 Acknowledgments

-   This project leverages the powerful **Amazon Chronos** library for time series forecasting.
-   The multi-site air quality dataset from Beijing is provided by the **TSDB** library.
-   Inspired by the need for robust and efficient time series analysis solutions.

<p align="center">
  Made with ❤️ by Aman
</p>
content_copy
download
Use code with caution.
Markdown
