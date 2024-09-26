# Pivot Table, VLOOKUP, Plotting

Exploring  different methods to look at data differently and how it leads to more effective and efficient data cleaning. 
To start with, we can get a visual in the form of a Pivot table by looking at specific parts of the data.

## Pivot Table in Google Spreadsheets:

A pivot table is a data summarization tool. It can be used in data processing and in data cleaning, for which pivot tables offer a quick, clutter-free view of your data. Pivot tables help sort, reorganize, group, count, total, or average data in a dataset

Lets consider a scenario where we only want to look at the most profitable product in a certain cosmetic company.

Select the entire table then go to _INSERT_ and select _Pivot Table_ option from the dropdown.
It will give you the dialog box for creating a new sheet as shown below-

![image](https://github.com/user-attachments/assets/ff7c5d8a-63ff-4f69-8229-16587de1e505)

Once the pivot table is created, Google Sheets creates a new sheet where you can define the pivot table. 
You can use the Pivot table editor to add specific data to your pivot table.

![image](https://github.com/user-attachments/assets/965d8687-523e-4c3f-af3a-364ceec74bf3)

Notice that the top two most ordered products are 15143Exfo and 32729Masc. The rest of the orders total less than $10,000.

## VLOOKUP - Vertical Lookup

VLOOKUP is a spreadsheet function that vertically searches for a certain value in a column to return a corresponding piece of information. There might be cases where we need to search across multiple sheets or even different databases for a specific informarion and VLOOKUP helps bring the information together.

Using the pivot table, we found the product codes of the most ordered products. In order to find the names of these products, we will use VLOOKUP.

Formula for VLOOKUP: 
```=VLOOKUP(data to look up, 'where to look'!Range, column, false)```

![image](https://github.com/user-attachments/assets/082a6c0b-05fd-4e3e-a8f3-749a1fb19a35)

![image](https://github.com/user-attachments/assets/6b1fe1ef-e8ca-4675-a8cd-3c0376e315c3)

Using the product code from the pivot table we can look for the top selling products and to do that we can make use of the FIND tool provided by google spreadsheets and get a list of desired products.

![image](https://github.com/user-attachments/assets/5f163023-d618-4673-ae8a-619221a5c032)

## Creating a Sample Table

To practice more spreadsheet functions and data cleaning I have created a data sample and performed the below-mentioned steps.

### 1. Cleaning the data
The first step here is to clean the data by eliminating the extra blank spaces the table has using the TRIM() and replicating the table below

 ![image](https://github.com/user-attachments/assets/d906637a-beb3-4bd5-9629-3432743cba67)

 ![image](https://github.com/user-attachments/assets/a4222c0a-2bb2-4734-be11-f61d7632cf9d)

### 2. Replicating the table
In order to replicate the cells in the same sheet we make use of the VALUE()

 ![image](https://github.com/user-attachments/assets/4476ca6b-d004-4260-a33d-0dd897142860)

 ![image](https://github.com/user-attachments/assets/ff6fdffd-b4f0-46b5-ace3-fbd896509aa4)

 ![image](https://github.com/user-attachments/assets/f9b3e089-1edc-4567-bba8-3530ccdf761e)

 ![image](https://github.com/user-attachments/assets/5dc7fc3e-b01c-4c44-af9e-f0518951e805)

### 3. Performing Calculations
Google spreadsheets provide a wide range of calculation functions which are of great use when we want to compute values in our table as shown below.

 ![image](https://github.com/user-attachments/assets/0f9a9ad3-9a7a-4c1a-9d81-53d9be84f1e5)

 ![image](https://github.com/user-attachments/assets/3f9c94db-5615-4229-a3ae-43c9e68ac121)

### 4. Use of VLOOKUP
There are times when we need to bring in the columns from different spreadsheets and that is when VLOOKUP helps a lot as we can see below,

 ![image](https://github.com/user-attachments/assets/f23f0c1d-ac8c-4dd2-9266-2c57a22a0598)

 ![image](https://github.com/user-attachments/assets/d4db99d8-64c9-4716-8c50-8a2ac3c1d045)

 ![image](https://github.com/user-attachments/assets/641fd7d2-4bd8-421c-99de-ec539d2b3fd7)

 ![image](https://github.com/user-attachments/assets/5c0e0dd5-5d5f-4322-ab19-4ead38e94a38)

The final table after performing all the above steps:
  
![image](https://github.com/user-attachments/assets/8703352e-9642-40d0-b0ea-e923d7ece18b)

### 4. Creating a PIVOT table
We can further analyze the data with the help of the Pivot table as shown below.

![image](https://github.com/user-attachments/assets/b3d215f3-6682-4850-8549-55e53a018565)

![image](https://github.com/user-attachments/assets/4df09883-e335-4c27-8f77-5e5afe0837c2)

![image](https://github.com/user-attachments/assets/3c53f562-4f44-4976-a7ce-38fafab9d798)

## RESULT

![image](https://github.com/user-attachments/assets/fd7c6112-de7a-4406-8b4a-ffd315e70f86)

The data has been cleaned and labelled correctly, using VLOOKUP the data was imported from another sheet and a pivot table was created.

## Plotting:
The plotting tool allows us to quickly create a graph, chart, table, or other visual from data. Plotting is useful for identifying skewed data or outliers. Let us go ahead and see if we have any outliers in our table. The data set used to demonstrate this is a predefined dataset named as "Cosmetic Dataset"

![image](https://github.com/user-attachments/assets/a2978690-a6c1-414a-bad1-514299bf8d42)

As we have the data in the form of a chart we can check for obvious outliers and fix them in the spreadsheet. For example, you might notice that an item in the middle of the chart has an extremely low price of $0.73. The decimal point is in the wrong place. In cell B14, correct this price to $7.30, and notice that Google Sheets automatically updates the chart.
