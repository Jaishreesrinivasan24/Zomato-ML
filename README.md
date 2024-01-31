# Zomato-ML

Navigating to dataset for reference
https://www.kaggle.com/datasets/narsingraogoud/zomato-restaurants-dataset-for-metropolitan-areas

**About the Client:**
I'm working on the Ecommerce domain with restaurants tied up with food delivery partner "Zomato" application in Indian metropolitan areas.
In this dataset, we have more than 127000 rows and 12 columns, a fairly large dataset. We have variables like Restaurant Name,	Dining Rating,	Delivery Rating,	Dining Votes,	Delivery Votes,	Cuisine,	Place Name,	City,	Item Name,	Best Seller,	Votes,	Prices

![zomato-1200x600-1](https://github.com/Jaishreesrinivasan24/Zomato-ML/assets/145618580/bd74efbb-a7d0-45e6-87da-c17bddee78c2)


As a Data analyst, Loaded the dataset for cleaning and processing the data, to find insightful results.

**Observations:**
Column name have spaces, should be edited
Each variable have its unique value whereas placename and city together makes sense 
There are missing values in certain variables like Dining Rating, Delivery Rating, Best Seller
Need to clean individual column for better results
Remove NaN values and equalize the rows for better analysis

**Cleaning and Preprocessing**
Substituting the null values with average values for better analysis
Dropping nulls values in all the variables if available
Removed column name 'City'


**Insights**
1. Average delivery rating shows the restaurants received reviews for takeouts
        Utilized histogram to visualize it to find the average delivery rating
          Result: 3.95-4.2 is the average value

2. Depending on cuisines distribution of prices been visualized
        Utilized barplot to represent the cuisines highest to lowest price
           Result: Lucknowi, Kebab and Continental takes first 3 position and
                   Maharastrian, Kerala and tea are the cuisines take last 3.

3. Top 10 Restaurant Names by Dining Rating and their special dishes
        Utilized Pie chart and subplot graphs to show the Top 10 restaurants and their special dishes
           Result: Natural Icecream- Tender coconut icecream tops in Dining Rating among others.

4. Most popular Restaurant by Place in India
         Calculated Total Rating by adding both Dining and Delivery Rating
           Result: Top 10 popular restaurant been listed as per place name and Rating: 9.3
                   Place Name : Connaught Place, New Delhi	Restaurant Name :Natural Ice Cream	

**Machine learning**

For customer retention, customer satisfaction and to improve the delivery service we take Delivery Rating as target variable

Splitting the data into training and testing sets
Defining preprocessing steps
Define the pipeline and train the model
Evaluate the model

Calculate the R2 score and Mean Squared error(MSE)
Created a pickle file to use the model later with more data been added also.
For Stakeholder collaboration created cleaned zomato dataset file in csv format

**Conclusion:**
**MSE** measures the average squared difference between the predicted values and the actual values. It is calculated as the average of the squared differences between each predicted and actual value.
In the above dataset the MSE value is approximately 1.33e-06, which is a very low value. Lower MSE values indicate better model performance, as it means that the model's predictions are close to the actual values. 

**R-squared** is a statistical measure of how well the regression predictions approximate the real data points. It is a value between 0 and 1, where 1 indicates a perfect fit, and 0 indicates that the model does not explain the variance in the target variable.
In the above dataset, the R-squared value is approximately 0.999979, which is very close to 1. This suggests that the model explains a high percentage (about 99.9979%) of the variance in the delivery ratings.

R-squared is particularly useful for understanding the proportion of the target variable's variability that can be explained by the model. A high R-squared indicates a good fit of the model to the data.
