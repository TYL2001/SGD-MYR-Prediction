## SC1015 Mini-Project
This repository is submitted to Nanyang Techonological University (NTU) for the course SC1015 (Introduction to Data Science and Artificial Intelligence), and for the tutorial group **FCS7, Group 2.**
## Contributors
Tan Yi Liang (YTAN273@e.ntu.edu.sg)

Chong Zhao Hui (ZCHONG025@e.ntu.edu.sg)

Dinh Pham Minh Anh (DINH0016@e.ntu.edu.sg)

**All members had equal part in this project.**
## Libraries
- [Pandas](https://pandas.pydata.org/)
- [Numpy](https://numpy.org/)
- [Scikit-learn](https://scikit-learn.org/stable/)
- [Matplotlib](https://matplotlib.org/)
## Datasets
Datasets used for this project can be found [here](https://github.com/TYL2001/SGD-MYR-Prediction/tree/main/Datasetshere), with the sources found [here](https://github.com/TYL2001/SGD-MYR-Prediction/blob/main/Datasets/Source.txt).



# Exchange Rate Prediction Model
## Project Overview
This project aims to predict the currency exchange rates between Singapore and Malaysia based on historical economic data. Our motivation stems from the understanding that exchange rates are influenced by numerous dynamic factors, and accurate predictions can benefit financial analysis and investment strategies. By applying machine learning techniques, we aim to develop models that may be able to reflect the complexities of currency valuation. The Jupyter Notebook can be found [here](https://github.com/TYL2001/SGD-MYR-Prediction/blob/main/SGD_MYR_Prediction.ipynb).

## Exploratory Data Analysis (EDA)
For our EDA, we employed linear regression to identify basic trends and correlations within the data from historical years excluding the latest 3 years. This phase helped us understand the relative influence of different variables on exchange rates.
- **Trend Analysis**: We studied the data trends over the years to spot any consistent patterns.
- **Correlation and Prediction**: Using RMSE (Root Mean Square Error), we measured the accuracy of our predictions, highlighting the challenge of using a singular model to predict exchange rates due to their dependency on multiple factors.

## Modelling Techniques
Recognizing the limitations of a single-model approach, we explored stacking ensemble modelling to enhance predictive performance. This technique combines predictions from several models to reduce bias, variance, and improve interpretability.
![image](https://github.com/TYL2001/SGD-MYR-Prediction/assets/147519488/986bc22c-11a7-4997-9383-b89ab7cc9be9)


## Model Variants
- Complete Dataset Model: Utilizes all available data, excluding rows with missing values.
- KNN Imputation Model: Employs K-Nearest Neighbors to impute missing values, testing for improved RMSE.
- KNN Imputation Model excluding 2023 Data: Avoids the year 2023 due to high inaccuracy in KNN-imputed values for that year.
- Mean Imputation Model: Uses mean values for imputation, testing different data handling strategies.
- Macro Economic Model: Focuses on macroeconomic indicators and uses KNN Imputation technique.
- Trading and Investing Model: Concentrates on trading volumes and investment flows and uses KNN Imputation technique.
- Economic Health Model: Looks at indicators of a country's economic health and uses KNN Imputation technique.

## Findings
The RMSE of the above models was extremely high, signifying that the models had a terrible accuracy in predicting the exchange rates.

## Conclusion
This project highlights the significant challenges involved in forecasting exchange rates with high accuracy. Despite employing advanced ensemble techniques and multiple model variations, the persistently high RMSE values across all models reflect the unpredictable nature of exchange rates.

## Sources
- Sources for datasets are found [here](https://github.com/TYL2001/SGD-MYR-Prediction/blob/main/Datasets/Source.txt).
- https://www.investopedia.com/trading/factors-influence-exchange-rates/
