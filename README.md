# BigMart Sales Data Neural Network
  
## Overview

This project focuses on leveraging regression analytics to predict future sales for a diverse range of products across various store locations. The sales data, collected from BigMart in the year 2013, serves as the foundation for this predictive analysis. The primary objective is to utilize historical sales data, product attributes, and location-related factors to build a robust regression model that can accurately forecast sales in the future.

**Benefits of Sales Prediction:**
Predicting future sales has significant benefits for both businesses and consumers. For BigMart, accurate sales predictions enable strategic inventory management, optimizing stock levels to prevent overstocking or stockouts. This, in turn, enhances operational efficiency and reduces carrying costs. Additionally, sales predictions allow the identification of high-demand products and locations, aiding in targeted marketing campaigns and improved resource allocation. For consumers, accurate sales predictions can lead to more consistent product availability and potentially lower prices due to optimized inventory management.

As this project encompasses contributions from diverse aspects such as data preprocessing, feature engineering, regression modeling, and location-based analysis, it showcases the collaborative efforts of contributors with varied expertise, ultimately culminating in a predictive model that can drive informed decision-making for BigMart.

Please click [here](https://docs.google.com/presentation/d/1MLGNz3lZow-65TH0pca2mxmcsVfNuM0Paq-pxnvl1vI/edit#slide=id.g278fa82c89e_0_50) to view our findings presentation.  

## Datasets
Click [here](https://www.kaggle.com/code/hiralmshah/bigmart-sales-prediction/notebook) to view one of our primary datasets!  

# Contributors & Responsibilities
- Alex Kopp
- Andrew Skorupa
- Savannah Porter
- Mohamed Abou elkhier

  ## Alex

- **File Name:** Sales_predict_rf.ipynb
- **Methods:** RandomForestRegressor, train_test_split, StandardScaler, tensorflow_decision_forests, mean_squared_error
- **Performance:** The model's R-squared value of 0.586 showcases reasonable performance on the dataset, indicating its ability to capture sales patterns with a certain degree of accuracy.

## Savannah

- **File Name:** RF3.ipynb
- **Methods:** RandomForestRegressor, train_test_split, StandardScaler, RandomizedSearchCV
- **Performance:** RF3 achieves an R-squared value of 0.6080, indicating improved predictive accuracy compared to RandomForest's default settings.

## Mohamed

- **File Name:** GBR.IPYNB
- **Methods:** GradientBoostingRegressor, MinMax, KFold, hyperparameter tuning with nested loops
- **Performance:** The model achieves an R-squared value of around 0.705, indicating decent-to-good fit. Such performance is typically acceptable for real-world scenarios, showcasing the model's ability to capture meaningful data patterns.

## Andrew

- **File Name:** Exploratory_Analysis.ipynb
- **Methods:** train_test_split, StandardScaler, mean_squared_error, ensemble.GradientBoostingRegressor
- **Performance:** Evaluated by Mean Squared Error (MSE), the model's calculated MSE of approximately 0.0013 signifies accurate predictions aligned with actual sales. The accompanying deviance plot highlights its effective error minimization through boosting iterations.

 ## Mohamed

- **File Name:** XGBR_final_results.ipynb
- **Methods:** train_test_split, XGBRegressor, StandardScaler, SimpleImputer, sklearn.metrics
- **Performance:** The model achieved an R-squared value of approximately 0.82, indicating good performance for sale predictions. This level of performance is attributed to the model's ability to capture underlying sales patterns while considering real-world variability and noise.

## Alex

- **File Name:** Sales_predict_product.ipynb
- **Methods:** train_test_split, StandardScaler, LabelEncoder, XGBRegressor, sklearn.metrics
- **Performance:** The model achieved an R-squared value of about 0.543, suggesting moderate predictive accuracy. While the model captures a significant portion of sales data patterns, there's potential for improvement to enhance its predictive power.


## Highest Performing Model

Among the contributions, the code provided by **Mohamed** in the file `XGBR_final_results.ipynb` stands out as the highest performing model. This model achieved an impressive R-squared value of approximately 0.82, indicating a robust predictive capability for sales. Several factors likely contributed to its exceptional performance:

1. **XGBoost Algorithm:** The code utilizes the XGBoost algorithm, known for its ability to handle complex relationships and capture non-linear patterns in data effectively. The algorithm's boosted ensemble nature aids in refining predictions through multiple iterations.

2. **Feature Preprocessing:** The use of `StandardScaler` and `SimpleImputer` to preprocess features ensures that the data is properly scaled and missing values are handled appropriately. This preprocessing enhances the model's convergence and overall performance.

3. **Binned Target Variable:** Mohamed's code binned the "Item_Outlet_Sales" target variable by increments of 400 USD. This binning approach likely helped the model focus on predicting broader sales trends, reducing the impact of outliers and fine-grained variations.

4. **Hyperparameter Tuning:** The model configuration includes carefully tuned hyperparameters such as `learning_rate`, `n_estimators`, `max_depth`, and more. These optimized hyperparameters enable the model to fine-tune its predictions, resulting in better fit to the data.

5. **Real-World Variability:** The code takes into account the inherent variability and noise present in real-world sales data. This consideration likely contributes to the model's ability to generalize well to unseen data, yielding a more accurate predictive performance.

6. **Dataset and Preprocessing:** Mohamed's code reads the dataset from `Train_modified_Binned_150.csv` and performs one-hot encoding on various categorical features. This meticulous preprocessing ensures that the model receives relevant and structured input data.

7. **Model Training:** The code constructs an XGBoost regressor with carefully selected hyperparameters and trains it on scaled training data. This structured approach to model training contributes to its high predictive accuracy.

8. **Performance Evaluation:** The code evaluates the model's performance using the R-squared metric, indicating how well the model's predictions align with the actual sales data.

In conclusion, Mohamed's code demonstrates a well-structured approach to feature preprocessing, model selection, and hyperparameter tuning. The utilization of the XGBoost algorithm, binned target variable, and the understanding of real-world data dynamics have likely synergized to produce a model with exceptional predictive power for sales data.

---

## Insights from the data:







<br>
<br>
<br>
**Please visit our individual Github pages below**  
[Alex Kopp](https://github.com/alexkopp12)  
[Andrew Skorupa](https://github.com/AndyMSkor)  
[Savannah Porter](https://github.com/SavannahWithAnH)  
[Mohamed Abou elkhier](https://github.com/nabroo101)  
 
