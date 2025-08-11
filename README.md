# Diwali_Sales_Data_Analysis

Problem Statement:I want to understand how people shop during Diwali by looking at sales data. This includes finding out which products sell the most, who buys them, and where the sales are highest.Analyze Diwali sales data to improve customer experience and sales.

This dataset contains retail transaction records from Diwali season sales across various cities and product categories. It offers insights into consumer demographics, purchasing behavior, and sales trends, enabling businesses to optimize marketing strategies and enhance customer engagement.

Libraries Used
 1.pandas – for data loading, cleaning, and manipulation
 2.numpy – for numerical operations and handling missing values
 3.matplotlib – for creating static visualizations
 
The dataset includes details such as:
- User_ID: Unique identifier for each customer
- Cust_name: Name of the customer
- Product_ID: Unique identifier for each product
- Gender: Male/Female
- Age Group: Age category of the customer
- Age: Exact age of the customer
- Marital_Status: 1 = Married, 0 = Unmarried
- State: State where the purchase was made
- Zone: Geographical zone (e.g., North, South, East, West)
- Occupation: Profession of the customer
- Product_Category: Type of product purchased
- Orders: Number of items ordered
- Amount (₹): Total amount spent on the order
- Status: (Empty column — no data available)
- unnamed1: (Empty column — likely irrelevant)

Data Preprocessing Steps:
 1. Manual Column Insertion:
      'Status', 'unnamed1'.
      Droping those unrelated Column.
     
 2.Duplicate Removal (Python):
     Removed duplicate entries using:// df = df.drop_duplicates()
     
 3.Null Value Detection:
     Detected missing values using:// df.isnull().sum()
      I have missing values in:
           Amount              12
           
 5.Droping null values:
     //df.dropna(inplace=True)
     
 6.Converting DataType:
      The Amount column from float64 to int, which is useful if we want to work with whole numbers—especially for currency values where decimal       precision isn’t needed.
 
 7.Describe():
      describe() method returns description of the data in the DataFrame (i.e. count, mean, std, etc)
      
Data Visualizations Created:

1.Pie Chart (Gender)
  Shows the proportion of male vs female buyers as a percentage of total.

2.Bar chart (Gender vs Amount)
  Compares total purchase amount between genders, highlighting spending power.
  
3.Bar Chart (Age Group vs Amount)
  Displays which age groups contribute most to sales, revealing buyer demographics.
  
4.Bar Chart (State vs Orders)
  Highlights top 10 states by number of orders, showing regional demand.

5.Bar Chart (State vs Amount)
  Shows top 10 states by total sales amount, indicating high-revenue regions.

6.Correlation Heatmap
Shows relationships between numerical variables like Age, Orders, and Amount.

Conclusion:
 Married women age group 26-35 yrs from UP, Maharastra and Karnataka working in IT, Healthcare and Aviation are more likely to buy products from   Food, Clothing and Electronics category.


   



