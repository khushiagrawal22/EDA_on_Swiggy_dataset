# EDA_on_Swiggy_dataset
The Swiggy dataset contains information on restaurants, such as their names, locations, ratings, and more. By performing EDA on this dataset, I gained a better understanding of the relationships between these different variables and discover some interesting insights about the restaurant industry.

Importing libraries: The necessary libraries such as numpy, pandas, matplotlib, and seaborn are imported.

Reading CSV: The Swiggy dataset is read from a CSV file and stored in the variable Swiggy_data. The first five rows of the dataset are displayed using the head() function.

Data exploration: Some initial exploration of the dataset is performed, including checking the shape of the data (number of rows and columns), displaying column names, and checking the data types of columns.

Data preprocessing: Irrelevant columns (Address, Area, and Locality) are dropped from the dataset. Duplicates are also removed.

Data cleaning: The "Rating" column contains missing values (NaN), which are filled with the mean value of the column.

Column renaming: The column name "Cost for two" is renamed to "Cost2plates", and "Long Distance Delivery" is renamed to "Delivery".

Cleaning the "Category" column: The "Category" column is analyzed to identify categories with a frequency of less than 300. These categories are replaced with "others" for better visualization.

Data visualization: Various visualizations are created using seaborn and matplotlib to explore the data. These visualizations include the total number of restaurants in each city, food delivery availability, restaurant type (veg or non-veg), the relationship between food delivery and rating, and city-wise ratings of restaurants.

I explored different aspects of the dataset and here are few of my observations:
✅Total number of restaurants in each city:
A bar chart or a count plot is created to display the total number of restaurants in each city.The cities are represented on the x-axis, and the corresponding count of restaurants is shown on the y-axis.
✅ Food delivery availability:
A bar chart is generated to illustrate the availability of food delivery in different cities. The chart shows the proportion or count of restaurants offering food delivery and those that do not. The slices or bars are labeled to indicate the percentage or count of restaurants falling into each category.
✅Restaurant type (veg or non-veg):
A bar chart is used to depict the distribution of restaurant types, i.e., vegetarian or non-vegetarian. The chart showcases the proportion or count of veg and non-veg restaurants in the dataset. Labels are added to each slice or bar to indicate the percentage or count of restaurants belonging to each type.
✅Relationship between food delivery and rating:
A line plot is employed to explore the relationship between food delivery and restaurant ratings. The x-axis represents the food delivery availability, while the y-axis represents the restaurant ratings. Each data point on the plot represents a restaurant, and its position signifies the rating and delivery status.
✅City-wise ratings of restaurants:
A box plot or a violin plot is utilized to visualize the distribution of restaurant ratings across different cities. Each city is represented on the x-axis, while the y-axis denotes the rating values. The plot displays the median, quartiles, and potential outliers, offering insights into the rating distribution for each city.
