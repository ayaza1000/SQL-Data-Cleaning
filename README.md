# **SQL Data Cleaning Project**

## **Overview**
This project demonstrates how to clean and preprocess real estate transaction data using SQL. The dataset, **Nashville Housing**, contains inconsistencies such as missing values, duplicate records, and unstructured data fields. The SQL queries used in this project help standardize, organize, and optimize the dataset for further analysis.

## **Objectives**
- Standardize date formats
- Populate missing property addresses
- Split address fields into separate columns
- Normalize categorical data
- Remove duplicate records
- Drop unnecessary columns

## **Dataset**
The dataset used is **NashvilleHousing** . The Excel file is uploaded to this repository.

## **Cleaning Steps**

### **1. Standardizing Date Format**
Converted `SaleDate` from `Datetime` to `Date` format.

### **2. Populating Missing Property Addresses**
Used self-join to fill in missing property addresses based on matching `ParcelID`.

### **3. Splitting Address into Separate Columns**
Extracted street address and city from `PropertyAddress` and `OwnerAddress`.

### **4. Normalizing "Sold as Vacant" Field**
Replaced 'Y' and 'N' values with 'Yes' and 'No'.

### **5. Removing Duplicate Records**
Used `ROW_NUMBER()` to identify and remove duplicate entries.

### **6. Deleting Unused Columns**
Dropped unnecessary columns to optimize the dataset.

## **Tools Used**
- **SQL Server Management Studio (SSMS)**
- **Microsoft SQL Server**

## **How to Use**
1. Clone this repository.
2. Import the dataset into your SQL Server.
3. Run the SQL scripts in sequence to clean and transform the data.
4. Use the cleaned dataset for further analysis or visualization.

## **Author**
Ayaz Ahmed - Data Analyst

## **License**
This project is open-source and free to use under the MIT License.

