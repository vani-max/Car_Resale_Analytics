# Car Resale Dataset Analysis

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

## Analysis Suggestions
* Build regression or ML models to predict resale_price using car specifications and usage details.
* Analyze how car_age impacts resale price across different car segments.
* Examine the relationship between kms_driven and resale value.
* Compare average resale prices across fuel_type and transmission_type.
* Study how resale prices vary across different Indian cities.
* Identify the most influential factors affecting car resale value.

## Key Insights & Statistics
* Typical Resale Price: The median resale price is ₹5.65 lakh, which better represents the market than the higher average of ₹8.37 lakh due to premium outliers.
* Age-Driven Depreciation: Average car age is 9.5 years, with sharp value drops observed beyond the 8–10 year range.
* Usage Threshold Effect: Vehicles driven beyond 60,000 km experience accelerated depreciation.
* Fuel Preference: Petrol vehicles dominate listings (~65%), while diesel vehicles retain relatively higher value in older age buckets.
* Insurance Premium: Comprehensive insurance listings command a clear resale premium over third-party insured vehicles.
* Market Concentration: A limited number of cities contribute disproportionately to higher-value listings.
* Segment Skewness: Price distribution is right-skewed due to the presence of luxury vehicles.
* Data Quality Impact: Standardization of units and insurance categories materially improves analytical reliability.


## Data Cleaning Notes 
* Converted price, mileage, engine capacity, max power, and kms driven columns to numeric format by removing units and text.
* Standardized mixed units and inconsistencies in mileage and max_power columns.
* Handled missing and zero values using median imputation (numerical) and mode (seats).
* Normalized categorical columns (insurance, fuel_type, owner_type, body_type, city) using proper casing and trimming.
* Consolidated insurance types into Comprehensive, Third Party, and Not Available.
* Removed duplicate records and created a new feature car_age from registered year.

## Dashboard
![Dashboard image](dashboardd.png)
