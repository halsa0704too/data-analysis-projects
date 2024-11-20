# data-analysis-projects
# NBA Player Performance Prediction (Regression Analysis)

## Project Overview

This project aims to predict NBA player performance, particularly their points scored (`pts`), using historical player data. The analysis utilizes linear regression and ridge regression models to identify key predictors and evaluate model performance using various metrics, including R-squared and Mean Absolute Error (MAE).

The following steps were performed during this project:
1. **Exploratory Data Analysis (EDA):**  
   - Visualized distributions of key statistics (`pts`, `reb`, `ast`).
   - Analyzed correlations between features to identify important predictors of performance.

2. **Feature Engineering:**  
   - Standardized numerical features to improve model accuracy.
   - Investigated possible new features that could help predict performance (e.g., performance trends).

3. **Feature Selection:**  
   - Used correlation analysis and feature importance from Ridge Regression to identify the most significant predictors of `pts`.

4. **Model Training and Evaluation:**  
   - Trained both Linear Regression and Ridge Regression models.
   - Evaluated models using R-squared and MAE metrics to assess performance.
   - Performed hyperparameter tuning on Ridge Regression to find the optimal alpha value.

5. **Residual Analysis:**  
   - Analyzed residuals to check for patterns and validate model assumptions.

---

## **Project Structure**

```
NBA_Player_Performance_Prediction/
│
├── data/
│   └── nba_players.csv               # Dataset containing NBA player stats
│
├── notebooks/
│   └── NBA_Performance_Prediction.ipynb # Jupyter notebook with code and analysis
│
├── README.md                         # Project description and instructions
└── requirements.txt                  # List of dependencies
```

---

## **Dependencies**

The following libraries are required to run the code:

- **pandas**: For data manipulation
- **numpy**: For numerical operations
- **matplotlib**: For data visualization
- **seaborn**: For advanced visualizations
- **scikit-learn**: For machine learning models and metrics

To install the dependencies, run the following command:

```bash
pip install -r requirements.txt
```

---

## **Instructions**

1. **Clone the repository**  
   First, clone this repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/NBA_Player_Performance_Prediction.git
   ```

2. **Prepare the data**  
   Ensure that you have the dataset (`nba_players.csv`) placed inside the `data` folder.

3. **Run the Jupyter Notebook**  
   Open the Jupyter notebook (`NBA_Performance_Prediction.ipynb`) using the following command:

   ```bash
   jupyter notebook notebooks/NBA_Performance_Prediction.ipynb
   ```

   The notebook will guide you through the analysis steps, including:
   - Loading and cleaning the data.
   - Performing EDA and visualizing key statistics.
   - Feature engineering and scaling.
   - Training models and evaluating them.
   - Conducting residual analysis.

4. **Results**  
   After running the notebook, you will obtain the following outputs:
   - EDA visualizations (distribution of `pts`, `reb`, `ast`).
   - A correlation heatmap of the features.
   - Model evaluation metrics (R-squared and MAE for Linear Regression and Ridge Regression).
   - A brief summary of feature importance and the contribution of each feature to the predictions.

---

## **How to Run the Code**

- Install the required libraries by running `pip install -r requirements.txt` in your terminal.
- Make sure the dataset (`nba_players.csv`) is in the correct path (`data/nba_players.csv`).
- Open the Jupyter notebook and run all cells in order.
- Check the results and visualizations as you progress through the notebook.

---

## **Key Insights from the Analysis**

- **Important Features:**  
  Features like `usg_pct`, `ts_pct`, and `ast` were identified as significant predictors of player points.
  
- **Model Performance:**  
  The Ridge Regression model performed well after hyperparameter tuning (R-squared: **0.8889**, MAE: **1.364**). Linear Regression also performed adequately, with similar results.

- **Feature Engineering:**  
  Feature scaling and selection significantly impacted the accuracy of the models.

---

## **Acknowledgements**

- The dataset used in this project is provided by [insert source of dataset if applicable].

---

### Feel free to customize this README according to your exact project setup and results! Let me know if you need further assistance with the README or any other part of the project.
