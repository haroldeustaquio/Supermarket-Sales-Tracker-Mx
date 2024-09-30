# Sales transaction clustering

## Project overview

This project applies a variety of machine learning models to analyze a real-world dataset. Clustering techniques, such as **clustering**, have been implemented to segment customers based on their purchasing behaviors and demographic characteristics. Additionally, classification models, such as **decision trees** and **logistic regression**, have been used in specific cases that require categorizing customers according to different criteria. In the near future, **regression** models will be applied with the aim of predicting trends and quantitative relationships between variables, allowing the company to anticipate future behaviors and optimize its business strategies. This in-depth analysis will allow marketing and sales actions to be customized, improving results in various product sectors.

## Business context

The dataset comes from a company that seeks to optimize its marketing and sales strategies based on customer behavior. The main objectives of this analysis are:

- **Segment customers**: Group customers into segments based on demographic characteristics (such as age, marital status, education level) and purchasing patterns (such as product preferences, spending habits).
- **Product sector analysis**: Analyze product sectors to identify sales trends and customer behavior for specific categories, lines, and sublines.

By leveraging clustering, the company aims to:

- **Personalize marketing strategies**: Tailor marketing campaigns to each customer segment, offering relevant products and promotions.
- **Identify new business opportunities**: Discover potential markets or customer needs that can be addressed with new product development or expansion into different sectors.
- **Improve customer experience**: Provide more personalized services, improving customer satisfaction and loyalty by understanding their specific needs and preferences.

## Data Description

The dataset contains a wide variety of variables relevant to customer purchasing and demographics:

- **Product-related variables**: `Industry`, `Type`, `Line`, `Subline`, `Presentation`, `Weight`, `Product`, `Description`
- **Transaction details**: `Date`, `Transaction`, `Order`, `Quantity`, `Price`, `Max_Price`, `Max_Price_Dif`, `Amount`
- **Customer demographics**: `Customer`, `Customer_Key`, `No._Children`, `Seniority`, `Age`, `Age_Range`, `Education`, `Marital_Status`, `State`, `Sex`
- **Business identifiers**: `Company`, `Year`
- **Other variables**: `Function`, `Group`

These variables provide detailed information about the purchasing behavior of customers, allowing the company to better understand both their demographic characteristics and how they interact with different product categories.

## Clustering algorithms

The following clustering algorithms were used in this project:

- **K-Means Clustering**: A classic partitioning algorithm that assigns each data point to the nearest cluster center based on distance.
- **Agglomerative Clustering**: This is useful for creating a hierarchy of clusters, joining the data into larger groups based on similarities, starting with each data point as its own cluster. It is particularly effective for uncovering the hierarchical structure of the data.

## Classification algorithms

The following classification algorithms were used in this project:

- **Decision trees:** a hierarchical rule-based model that segments data by successive splits, selecting features that maximize separation between classes. It is useful for clear and visual interpretations of the decision-making process.

- **Logistic regression:** a statistical model used to predict the probability of an instance belonging to a particular class. It is especially effective for binary classification problems, allowing relationships between features and classes to be modeled through a sigmoid function.

Both algorithms provided valuable insights into the categorization of the data and helped optimize the performance of the model.

## Regression algorithms

The following regression algorithms were applied in this project:

- **DecisionTreeRegressor:** A model that predicts continuous values by recursively splitting the dataset based on feature values, generating a tree structure. It selects splits that minimize the variance within each segment, making it an interpretable model with the ability to capture complex, non-linear relationships in the data. This approach is particularly useful for understanding which features most influence the target variable.

- **GradientBoostingRegressor:** A powerful ensemble method that combines multiple weak prediction models (typically decision trees) in a sequential manner. Each tree corrects the errors of its predecessor, gradually improving prediction accuracy. It is highly effective for capturing non-linear relationships and managing both overfitting and underfitting through hyperparameter tuning, making it suitable for complex regression tasks.

## Requirements

Make sure you have the following Python libraries installed:

- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`
- `seaborn`
- `shap`