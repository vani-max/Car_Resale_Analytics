# Car Resale Dataset Analyis

## Project Overview

This dataset contains used car resale prices across multiple cities in India, updated as of August 2023.
It is provided in a raw and uncleaned format to offer hands-on experience with real-world data preprocessing, analysis, and modeling.

![Dataset Analysis image](car.png)

## File Details

* **File name** : car_resale_value.csv
* **Total Records** : 1,79,490

## Data Dictionary
| **Column Name** | **Description** | **Data Type**|
|-------------|-------------|----------|
|**Index**    | Numbering   | Integer|
|**Name**	    |Car brand and model|	text|
|**Year**	|Manufacturing year|	Integer|
|**Selling_Price**|	Resale price of the car (INR)|	Float|
|**Present_Price**	|Original showroom price (INR)|	Float|
|**Km_Driven**|	Total distance driven (in km)|	Integer|
|**Fuel_Type**|	Petrol / Diesel / CNG|	Categorical|
|**Seller_Type**|	Individual or Dealer|	Categorical|
|**Transmission**|	Manual / Automatic	|Categorical|
|**Owner**|	Number of previous owners|	Integer|
|**Mileage**|	Fuel efficiency (km/l or km/kg)|	Float|
|**Engine**|	Engine capacity (CC)	|Integer|
|**Max_Power**|	Maximum engine power (bhp)|	Float|
|**Seats**|	Seating capacity |Integer|

## Key Insights & Statistics




## Analysis Suggestions




## Data Cleaning Notes 
* Converted price, mileage, engine capacity, max power, and kms driven columns to numeric format by removing units and text.
* Standardized mixed units and inconsistencies in mileage and max_power columns.
* Handled missing and zero values using median imputation (numerical) and mode (seats).
* Normalized categorical columns (insurance, fuel_type, owner_type, body_type, city) using proper casing and trimming.
* Consolidated insurance types into Comprehensive, Third Party, and Not Available.
* Removed duplicate records and created a new feature car_age from registered year.

## Dashboard
