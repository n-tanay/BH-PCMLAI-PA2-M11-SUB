# BH-PCMLAI-PA2-M11 - What drives the price of a car?

Link to Notebook: 

## Business Understanding

From a business perspective, the goal of this project is to identify key drivers for used car prices. This task can be reframed as a data problem where we aim to use predictive modeling to analyze which features (e.g., transmission, condition, mileage) significantly affect car prices, allowing for optimal pricing strategies.

## The Goal

The primary objective of this project is to help the used car dealership price their inventory more accurately by identifying the factors that significantly influence the price of used cars. The goals include:

1. **Maximize Profit Margins**: Price vehicles competitively but optimally to ensure high profit margins.
2. **Move Inventory Faster**: Understand which cars are priced in line with customer preferences to accelerate sales.
3. **Highlight Desirable Features**: Emphasize the features that customers value most to attract potential buyers through targeted marketing.

## Key Business Questions

1. **Which factors have the strongest influence on car prices?**
    *   Analyze features like brand, model, year, mileage, engine size, fuel type, and condition to determine their impact on pricing.
2. **How do market trends affect car prices over time?**
    *   Identify seasonal variations or trends, including the impact of newer technologies like electric vehicles.

## Data Mining Goals

*   **Develop Predictive Models**: Create models (e.g., linear regression, random forest, XGBoost) that can accurately estimate car prices based on relevant features.
*   **Segment Analysis**: Use clustering to identify groups of similar cars that exhibit similar price trends.
*   **Feature Importance**: Determine which features most impact car prices using methods like feature importance ranking.
*   **Customer Preferences Analysis**: Identify which car features or brands customers are most willing to pay for.

## Summary of Findings

Several regression models were evaluated for predicting car prices using selected features. The key metrics used to evaluate model performance were Mean Squared Error (MSE), R-squared (R²), and Mean Absolute Error (MAE):

*   **XGBoost**: Best performer across all metrics, with an MSE of 54,623,590, R² of 0.700, and MAE of 4914.
*   **LightGBM**: Comparable to XGBoost with an MSE of 54,651,120, R² of 0.700, and MAE of 4922.
*   **Linear and Ridge Regression**: Moderate performance, R² of 0.561, less accurate than XGBoost and LightGBM.
*   **Random Forest**: Lowest R² (0.527) and highest MAE (6912), indicating poor performance.

### Best Model

The **XGBoost** model is recommended for deployment due to its superior performance in predicting car prices accurately and consistently across all metrics.

## Next Steps and Recommendations

1. **Deploy XGBoost Model**: Use XGBoost to estimate car prices for the dealership's inventory to maximize profits.
2. **Feature Importance for Marketing**: Highlight key features (e.g., Transmission, Condition, Fuel Type) in marketing campaigns to attract buyers and accelerate inventory movement.
3. **Optimize Pricing Strategy**: Use model predictions to adjust prices and ensure alignment with customer preferences and market trends.
4. **Segment Analysis for Stability**: Segment cars by category and analyze price trends to aid in informed stocking decisions.
5. **Regional Pricing Insights**: Consider regional differences in pricing strategies to optimize sales in different locations.
6. **Continuous Model Monitoring**: Monitor model performance and retrain periodically to maintain accuracy, especially when new market trends emerge.
7. **Customer Insights**: Analyze influential features to better understand customer preferences and inform targeted marketing strategies.

By following these recommendations, the dealership can achieve its goals of optimizing profit margins, accelerating inventory turnover, and attracting buyers by focusing on key vehicle features.