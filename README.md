[california_housing_prediction.ipynb](https://github.com/user-attachments/files/32053971/california_housing_prediction.ipynb)

# California House Price Predictor

## 📌 Project Overview
This project builds a Machine Learning regression model to predict housing prices in California using the public California Housing dataset. The goal is to provide accurate property valuation estimates based on key demographic and geographic features, such as median income, average rooms and location.

## 🛠️ Tech Stack & Skills Demonstrated
* **Languages:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
* **Machine Learning:** Data Preprocessing, Data Splitting (Train/Test), Linear Regression Modeling, Model Evaluation

## 📊 Dataset Insights
The dataset contains 20,640 samples with 8 predictive features. The target variable is the median house value (`MedHouseVal`) for California districts, expressed in hundreds of thousands of dollars ($100 000).
* **Key Features Used:** Median Income (`MedInc`), House Age (`HouseAge`), Average Rooms (`AveRooms`), Population, and Latitude/Longitude.

## 📈 Model Performance & Evaluation
The model was trained on 80% of the dataset and evaluated on the remaining 20% using standard regression metrics:

* **R² Score (Coefficient of Determination):** `0.58` (0.575787...) — This indicates that approximately 58% of the variance in California house prices is predictable from the baseline features.
* **RMSE (Root Mean Squared Error):** `0.75` (0.745581...) — Since the target variable is expressed in hundreds of thousands of dollars ($100,000), this means that, on average, the model's price predictions deviate from the actual value by roughly **$74,558**.

### Actual vs. Predicted Price Visualization
To validate the model's behavior, a scatter plot was generated to compare the actual baseline values against the model's predictions. The dashed red line represents a perfect prediction model.

![Actual vs Predicted Prices Visual](actual%20vs%20predicted%20house%20values.png)

## 🚀 How to Run This Project Local
1. Clone this repository:
   ```bash
   git clone https://github.com
   ```
2. Install the required dependencies:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```
3. Run the script or Jupyter Notebook:
   ```bash
   california_housing_prediction.ipynb
   ```

## 🔮 Future Enhancements
* Implement more complex supervised learning algorithms like **Random Forest** or **Gradient Boosting (XGBoost)** to capture non-linear relationships.
* Perform feature engineering (e.g., combining latitude and longitude into clustering zones).
* Optimize hyperparameters using Grid Search cross-validation.
