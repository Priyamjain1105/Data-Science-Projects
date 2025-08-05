# Teenagers Phone Addiction
[Exploratory Data Analysis](EDA.ipynb)

## Hypothesis Testing and Models
- #### [Students Grade Prediction Based on their different Screen Times](H1.ipynb) 
  ### Project Report: Student Grade Prediction Based on Screen Time
    **1. Project Title:**
    Student Grade Prediction Based on Screen Time

    **2. Objective:**
    The primary goal of this project was to develop and evaluate machine learning models capable of predicting student grades based on their screen time data. A secondary objective was to analyze the impact of different feature engineering techniques on model performance, thereby determining the most effective approach for this prediction task.

    **3. Dataset:**
    The project utilized a dataset containing student information, with a particular focus on their recorded screen time and corresponding academic grades. The dataset was split into training and testing sets to ensure robust model evaluation.

    **4. Methodology:**

    The project followed a structured, comparative approach to assess the performance of the selected models under different data conditions.

    **a. Model Selection:**
    * **Linear Regression:** Chosen as a baseline parametric model due to its simplicity and interpretability. It assumes a linear relationship between screen time and grades, making it a good starting point for analysis.
    * **K-Nearest Neighbors (KNN) Regression:** Selected as a non-parametric alternative. This model's predictions are based on local data points, which can capture more complex, non-linear relationships that might not be detected by a linear model.

    **b. Feature Engineering Techniques:**
    * **Baseline Evaluation (No Feature Engineering):** Initial model training and evaluation were performed on the raw dataset. This step was crucial for establishing a baseline performance metric against which all other results could be compared.
    * **MinMax Scaling:** This technique was applied to scale the screen time data to a fixed range, typically [0, 1]. This normalization method is beneficial for algorithms that are sensitive to the magnitude of the input variables, such as KNN, as it prevents features with larger values from dominating the distance calculations.
    * **Standardization (Z-score Scaling):** This method transformed the screen time data to have a mean of 0 and a standard deviation of 1. Standardization is particularly effective for models that assume a Gaussian distribution of the features or those that rely on gradients, like Linear Regression, as it can stabilize learning and speed up convergence.

    **c. Performance Evaluation:**
    * **Metric Used:** The **Mean Squared Error (MSE)** was the sole performance metric utilized. MSE is a robust measure for regression problems that quantifies the average of the squared differences between predicted and actual values. A lower MSE indicates a more accurate model.

    **5. Implementation and Results:**

    The project was implemented using Python and standard machine learning libraries.

    * The Linear Regression and KNN models were trained on the training set.
    * Predictions were generated for the test set.
    * The MSE was calculated for each model under all three data conditions (raw, MinMax scaled, and standardized).
    * The results were documented to provide a direct comparison of the models' predictive accuracy and the impact of the feature engineering techniques.

    **6. Conclusion:**

    The project successfully demonstrated the process of building and evaluating predictive models for student grades. The comparative analysis of Linear Regression and KNN, alongside the application of MinMax Scaling and Standardization, provided valuable insights into:

    * The inherent predictive power of each model for this specific problem.
    * The significant role of data preprocessing in improving model accuracy and stability.

    The final report and analysis allowed for a clear conclusion on which model and data preparation strategy yielded the most accurate predictions based on the Mean Squared Error metric.
