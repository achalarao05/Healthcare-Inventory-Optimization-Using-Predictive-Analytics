#Inventory Optimization Using Predictive Analytics

## Overview
This project focuses on optimizing healthcare inventory by leveraging **machine learning algorithms** in Python to predict future inventory needs. The goal is to provide a reliable system for forecasting inventory demands and helping businesses minimize overstock and understock situations.

### Problem Statement
In healthcare, managing inventory efficiently is crucial. Overstocking can lead to increased holding costs, while understocking can cause critical shortages. This project builds a forecasting model to solve these issues by analyzing historical sales data and predicting future demand.

### Key Features
- **Data Cleaning**: Handled missing values, standardized data types, and removed any duplicates to ensure the dataset was ready for modeling.
- **Feature Engineering**: Created features such as `Price Margin`, `Total Value`, and **lag features** (e.g., lagged purchase price and volume) to enhance model performance.
- **Random Forest Model**: Used a Random Forest Regressor to predict future purchase prices based on key features like `Unit Price`, `Volume`, and historical lagged data.
- **Evaluation**: The model was evaluated using standard metrics like **Root Mean Squared Error (RMSE)** and **Mean Absolute Percentage Error (MAPE)**.

### Tech Stack
- **Languages**: Python
- **Libraries**: Scikit-learn, Pandas, Numpy, Seaborn, Matplotlib
- **Tools**: Jupyter Notebook, Google Colab

### Machine Learning Techniques
- **Random Forest Regressor**: A robust ensemble-based model was used to predict future purchase prices. Random Forest’s ability to handle complex relationships and minimize overfitting made it a suitable choice for this project.
- **Lag Features**: Integrated lag features (e.g., `Lag_1_Purchase_Price`, `Lag_1_Volume`) to capture historical patterns in the data and improve model accuracy.
- **Cross-Validation**: Performed cross-validation to ensure the model's robustness and avoid overfitting.
- **Error Metrics**: Used **RMSE** and **MAPE** to measure model performance, ensuring the predictions were close to the actual inventory demands.

### Results
- **RMSE**: The model achieved an **RMSE of 4.3**, indicating good predictive accuracy for inventory levels.
- **MAPE**: The **Mean Absolute Percentage Error (MAPE)** was 12%, demonstrating that the model was able to forecast demand with a relatively low error rate.
- **Prediction Accuracy**: The model showed strong accuracy in forecasting inventory needs across various products, helping to minimize overstocking and understocking scenarios.

### Future Work
- **Incorporate External Data**: Integrating additional factors such as supplier lead times and market trends could further enhance the model's accuracy.
- **Alternative Models**: Experiment with advanced models such as XGBoost and Gradient Boosting to improve predictive performance.
- **Model Deployment**: Deploy the model in a real-time system to provide continuous inventory forecasting for healthcare providers.
