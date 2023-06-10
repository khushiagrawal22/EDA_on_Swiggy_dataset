# EDA_on_Swiggy_dataset
The Swiggy dataset contains information on restaurants, such as their names, locations, ratings, and more. By performing EDA on this dataset, I gained a better understanding of the relationships between these different variables and discover some interesting insights about the restaurant industry.

Importing libraries: The necessary libraries such as numpy, pandas, matplotlib, and seaborn are imported.

Reading CSV: The Swiggy dataset is read from a CSV file and stored in the variable Swiggy_data. The first five rows of the dataset are displayed using the head() function.

Data exploration: Some initial exploration of the dataset is performed, including checking the shape of the data (number of rows and columns), displaying column names, and checking the data types of columns.

Data preprocessing: Irrelevant columns (Address, Area, and Locality) are dropped from the dataset. Duplicates are also removed.

Data cleaning: The "Rating" column contains missing values (NaN), which are filled with the mean value of the column.

Column renaming: The column name "Cost for two" is renamed to "Cost2plates", and "Long Distance Delivery" is renamed to "Delivery".

Cleaning the "Category" column: The "Category" column is analyzed to identify categories with a frequency of less than 300. These categories are replaced with "others" for better visualization.

I explored different aspects of the dataset and here are few of my observations:

✅Visualizing Total Resturants in Cities
The provided code creates a bar plot using Seaborn's countplot() function to visualize the total number of restaurants in each city. The figure size is adjusted to make the plot larger, the x-axis tick labels are rotated for better readability, and a title is added to describe the purpose of the plot.

✅Visualizing Food Delivery
he code creates a bar plot using Seaborn's countplot() function to visualize the availability of food delivery. It counts the occurrences of 0 (indicating food delivery not available) and 1 (indicating food delivery is available) and represents them as bars in the plot. The figure size is adjusted to 5 inches by 5 inches.

✅Visualizing Restaurant type (Veg or Nonveg)
The output of this code is a bar plot that visualizes the restaurant types (veg or non-veg) based on the values in the 'Veg' column. The figure size is adjusted to 5 inches by 5 inches, and the color palette used for the bars is 'rainbow'. The title of the plot is set to 'Restaurant Type'.

✅Visualizing Food Delivery VS Rating
The output of this code is a box plot that compares the distribution of ratings for different categories of food delivery availability. The figure size is adjusted to 5 inches by 5 inches. The x-axis represents the food delivery availability (0 for not available, 1 for available), and the y-axis represents the ratings. The plot shows the median, quartiles, and possible outliers for each category of food delivery availability. The title of the plot is set to 'Food Delivery vs Rating'.

✅Visualizing City wise Ratings of Restro
The output of this code is a bar plot that shows the average ratings of restaurants in different cities. The figure size is adjusted to 16 inches by 8 inches. The x-axis represents the cities, and the y-axis represents the ratings. Each bar represents the average rating for a specific city. The x-axis tick labels are rotated by 90 degrees to improve readability when there are many cities.

✅Cities with Highest Rated Resturants
The output of this code is a bar plot that displays the mean ratings of the top 10 cities with the highest ratings. The figure size is adjusted to 8 inches by 6 inches. The x-axis represents the cities, and the y-axis represents the mean ratings. Each bar represents the mean rating for a specific city. The x-axis tick labels are rotated by 90 degrees to improve readability when there are many cities.

✅Visualizing long Distance Delivery Facility, City wise
The output of this code is a pivot table named df, where the 'city' column serves as the index, and the 'Delivery' values ('0' or '1') are used as columns. Each cell in the pivot table represents the count of restaurants in a specific city and whether they offer long-distance delivery or not. If a city doesn't have any restaurants with a particular delivery option, the corresponding cell value will be 0.
