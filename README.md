## Insights on Property Investment Profitability
<img src="./Image/RASB-berry.png" alt="RASB Berry Image" width="1000" height="700" class="blog-image">

## Table of Contents
- [Project Overview](#project-overview)
- [Business Problem](#business-problem)
- [Data Understanding](#data-understanding)
- [Methodology](#methodology)
- [Modeling](#modeling)
- [Conclusion](#conclusion)
   - [Key Findings](#key-findings)
   - [Recommendations](#recommendations)
   - [Limitations](#limitations)
- [Installation](#installation)
- [Usage](#usage)
- [Dependecies](#dependecies)
- [Folder Structure](#folder-structure)
- [License](#license)

## Project Overview<a name="project-overview"></a>
In this project, we're diving deep into the [King County House](map.html) Sales dataset to understand what makes properties profitable in King County's real estate market. Our main aim is to provide valuable insights to RASB-berry Property Investors who want to make smart investment decisions. We'll be looking at various aspects of properties, like their size, number of bedrooms, and condition, to see which factors have the most impact on the sale prices of houses. By doing this, we hope to help RASB-berry investors optimize their strategies and increase their chances of getting better returns in the King County real estate market.

## Business Problem<a name="business-problem"></a>
### Stakeholder: RASB-berry Property Investors
RASB-berry Property investors are looking to optimize their investment strategies by purchasing properties with the potential for high returns. They want to know which property attributes, such as square footage, number of bedrooms,and condition of the property, are most strongly correlated with sale prices.

## Data Understanding<a name="data-understanding"></a>
The dataset contains information about real estate properties in King County, consisting of 21 columns. These columns provide details such as property price, number of bedrooms, bathrooms, square footage, floors, waterfront status, condition, grade, and more. Some columns have missing values, like 'yr_renovated' and 'waterfront.' This dataset is valuable for analyzing the factors influencing property prices and making informed investment decisions in the King County real estate market.

## Methodology<a name="methodology"></a>
To help RASB-berry Property investors make informed decisions, we're using multiple linear regression analysis. Our goal is to build a predictive model for house prices in King County.

We're focusing on sale prices and studying how they relate to various property attributes. We'll use regression models to quantify these relationships and provide insights for RASB-berry Property Investors.

Our approach starts with a baseline model and refines it as we identify key factors influencing property values. We'll also use data visualization and descriptive analysis to understand the dataset better, ensuring our analysis is thorough and insightful..

## Modeling<a name="modeling"></a>
In this analysis, we developed three models: a baseline model (model 1), model 2, and model 3. The baseline model helped us identify the variable with the highest correlation with sale price. We then created model 2 to introduce additional variables, though it didn't significantly differ from the baseline.

However, model 3 stands out. It boasts a higher R-squared value, indicating improved performance and statistical significance. When we evaluated this model, it exhibited lower MAE, MSE, and RMSE values, indicating better predictive accuracy. 

We strongly recommend RASB-berry Property investors use this model for predicting sale prices due to its superior performance.

### Key takeways:
Overall Model Significance: The model as a whole is statistically significant, indicated by the low p-value of the F-statistic (p < 0.001). This suggests that at least one of the independent variables has a significant impact on housing prices.

Explained Variance: Our model explains approximately 59.2% of the variance in housing prices. This indicates a strong ability to capture and explain the variability in prices compared to our baseline model and model 2.

Significance of Categorical Variables: Several categorical variables, such as waterfront, view, condition, and grade, have a significant impact on housing prices. Notably, properties with waterfront views command substantially higher prices.

Limited Impact of Some Conditions: The "condition" variable, particularly the "Fair" and "Poor" conditions, does not have a statistically significant impact on prices in this model.

Luxury and Mansion Grades: Properties classified as "Luxury" and "Mansion" grades significantly increase housing prices, indicating that higher-grade properties are valued more.

Lower Grades: Conversely, lower-grade properties such as "Poor," "Low," and "Fair" have a substantial negative impact on prices

### Conclusion<a name="conclusion"></a>
After a comprehensive evaluation of the three models we've developed, it's evident that the third model stands out as the most promising choice. This conclusion is primarily based on its significantly lower Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE) compared to the other two models.

Notably, the MAE of the third model, when considered alongside the average housing price of approximately $541,317.18, is notably lower. This implies that, on average, the model's predictions deviate by a relatively smaller amount from the actual prices, showcasing its superior predictive accuracy.

Therefore, given the compelling performance metrics, particularly the lower MAE concerning the average price, we recommend adopting the third model as the preferred choice for predicting housing prices. This model demonstrates a more accurate estimation of prices, which can be highly valuable for real estate investment decisions and related applications.

   ## Key Findings<a name="key-findings"></a>
Here are some of the key findings from our analysis of the King County housing market:

Square Footage Matters: The square footage of living space (sqft_living) has a significant positive impact on housing prices. Investing in properties with larger living spaces tends to result in higher prices.

Waterfront Properties Command a Premium: Waterfront properties are highly desirable and come with a substantial price premium. Investors should consider these properties for potentially higher returns.

Views Enhance Value: Homes with excellent views or very good views also tend to fetch higher prices. This feature can be a valuable investment consideration.

Condition and Grade Influence Price: The condition and grade of a property are important factors affecting its price. Properties in very good condition and with higher grades tend to have higher values.

Budget Planning: With an average housing price of approximately $541,317.18, investors should budget and plan their investments accordingly.

   ### Recomendations<a name="recommendations"></a>
Here are the key recommendations and conclusions for RASB-berry Property investors based on our analysis:

Model Selection: We recommend using the third model as it demonstrates superior predictive accuracy with lower Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE) compared to the other two models.

Price Influencers: Focus your investment strategy on the factors that have the most significant impact on housing prices, which include square footage of living space (sqft_living), waterfront properties, views, condition, and grade.

Property Features: Prioritize properties with larger square footage (sqft_living) and those with waterfront views, excellent views, very good conditions, and higher grades, as these tend to command higher prices.

Diversification: Consider diversifying your real estate investments across different property types and neighborhoods to reduce risk and capture opportunities in various market segments.

Stay Informed: Continuously monitor local market trends, economic conditions, and regulations to make informed investment decisions.

Budget Planning: Given the average housing price of approximately $541,317.18, plan your investments accordingly and ensure your budget aligns with market conditions.
## Limitations<a name="limitations"></a>
Some of the limitations of the analysis were:

Limited Feature Set: The dataset may not include all the relevant features or variables that influence property prices. Other important factors, such as neighborhood crime rates, school quality, and proximity to amenities, may not be present in the dataset.
Temporal Data: The dataset may not include data on important temporal factors like economic conditions, interest rates, or changes in local regulations that can affect property prices.

Sample Size: The dataset's size may be limited, which can affect the robustness of predictive models, especially if you're working with small subsets of data.

Bias: The data may contain bias in terms of property types, locations, or price ranges, which can impact the generalizability of predictive models to other real estate markets.

Non-Stationarity: Real estate data often exhibits non-stationarity, meaning that trends and relationships can change over time. Accounting for this can be challenging.

Seasonality: Real estate markets can have seasonal patterns that are not explicitly captured in the dataset. For example, housing prices may vary based on the time of year.

Model Complexity: Depending on the complexity of the problem you're trying to solve, linear models or basic machine learning algorithms may not capture intricate patterns in the data.

Data Imbalance: If the dataset has an imbalanced distribution of target variables (e.g., a few high-value properties and many low-value properties), it can lead to modeling challenges.

Generalization: The dataset may represent a specific geographic area or time period. Models built on this data may not generalize well to different regions or time frames.

External Factors: Real estate prices can be influenced by external factors such as economic recessions or natural disasters, which may not be accounted for in the dataset.

To address these limitations and improve the accuracy of predictive projects, you can consider:

Collecting additional data from various sources to supplement the dataset.
Performing feature engineering to create new informative features.

  ## Dependecies<a name="dependecies"></a>
The analysis was conducted using Python with the following libraries:

1. Pandas
2. Numpy
3. Matplotlib
4. Seaborn
5. StatsModels
6. Sklearn
   
   ## Folder Structure<a name="folder-structure"></a>
- data
    -kc_house_data
    -column_names
-Property Investment Profitability Analysis.ipynb
-Non-Technical Presentation
    -Phase II Slides.pptx
    -Phase II Slides.pdf
-image/
    -RASB - berry.png
- map.html
- map_with_clustered_prices.html
- Property Investment Profitability Analysis.pdf    
- README.md


### Installation<a name="installation"></a>

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/PHASE-2-PROJECT.git
   ```

2. Navigate to the project directory:

   ```bash
   cd PHASE-2-PROJECT
   ```

3. Install the required Python packages

## Usage<a name="usage"></a>

To use this project:

1. Open the Jupyter Notebook files in the `notebooks` directory to explore the analysis, models, and visualizations.
2. Follow the instructions within the notebooks to run the code and generate predictions.

## Contributing<a name="contributing"></a>

We welcome contributions from the community. If you'd like to contribute to this project, please follow our [contribution guidelines](CONTRIBUTING.md).

## License<a name="license"></a>

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments<a name="acknowledgments"></a>

We would like to thank the King County Housing Market for providing the dataset used in this project. Additionally, we acknowledge the contributions of the open-source community for the tools and libraries used in our analysis.



