# 🏠 AirBnB-Booking-Analysis-EDA

![airbnb_booking](https://github.com/ankesh-aman/AirBnB-Booking-Analysis-EDA/assets/170477956/953c182d-3973-4b8f-9272-eaa5b535bd38)

## 📌 Project Type
Exploratory Data Analysis (EDA)

**Contribution**: Individual Project

**Author**: Ankesh Aman

## 📊 Project Summary

This project presents an in-depth exploratory data analysis (EDA) of Airbnb bookings in New York City, aimed at uncovering key insights that influence listing prices and availability. The analysis is designed to support travelers, hosts, and business stakeholders with data-driven insights for better decision-making.

Through this project, I:

* Explored and cleaned the Airbnb dataset for quality and consistency

* Identified outliers and handled missing values

* Conducted detailed statistical summaries and visual analysis

* Discovered trends, patterns, and relationships between variables (like room types, price, reviews, location, etc.)


## ✅ Key Goals:
* Understand what factors influence Airbnb pricing

* Analyze availability trends across neighborhoods

* Derive insights for both guests and hosts using data visualization


## 🧹 Data Cleaning & Preparation

Raw data often contains inconsistencies and errors that can skew analysis. To ensure accuracy and insightfulness, the dataset underwent a comprehensive cleaning process, which included the following steps:

1. **Missing Values Handling**

  * Checked for missing values across all columns using isnull().sum().
  
  * Columns with a significant amount of missing data were either dropped or imputed appropriately.
  
  * For example, listings with missing host_name or reviews were carefully analyzed and dropped if irrelevant.

2. **Data Type Conversion**
  * Converted columns like last_review to proper datetime format
  
  * Ensured numeric fields such as price, minimum_nights, number_of_reviews, and availability_365 were correctly typed

3. **Duplicate and Irrelevant Records**
  * Removed any duplicate entries to prevent skewed counts
  
  * Filtered out listings with unrealistic values, such as:
  
    - Prices of $0 or extremely high values (treated as outliers)
    
    - Listings with 0 availability or excessive minimum night stays (over 365 days)

4. **Outlier Detection & Removal**
  * Used visualization tools like boxplots to detect outliers in numerical columns
  
  * Capped or removed extreme outliers using percentile thresholds to ensure fair distribution for modeling and visualization

5. **Data Filtering**
  * Focused on listings within valid New York City boroughs
  
  * Filtered columns to retain only relevant features for the analysis
  
  * With a clean, structured dataset, the foundation was set for a meaningful and bias-free exploration.


## 🛠 Tools & Technologies Used

| Tool / Library       | Description                             |
|----------------------|-----------------------------------------|
| Python               | Core programming language for analysis  |
| Pandas               | Data cleaning, manipulation, and analysis |
| NumPy                | Numerical operations and array handling |
| Matplotlib           | Static visualizations (plots, charts)   |
| Seaborn              | Statistical data visualization           |
| Jupyter Notebook     | Interactive code and narrative writing  |



## 📈 Insights & Observations

The EDA revealed several compelling insights about how Airbnb operates in New York City, providing a mix of business intelligence and user experience understanding.

### 🏘 Neighborhood & Location Impact
  * Manhattan is the most expensive and highly saturated borough with a significant number of listings
  
  * Brooklyn is more affordable yet still popular among travelers
  
  * Staten Island and Bronx have the least number of listings and are often overlooked, but they offer more budget-friendly options

### 🛏 Room Type vs Price
  * Entire homes/apartments have the highest average prices, ideal for families and long-term stays
  
  * Private rooms offer a balanced trade-off between privacy and cost, making them attractive to solo travelers
  
  * Shared rooms are the least common and cheapest, often priced under $50

### 📆 Availability Trends
  * Listings with availability_365 = 0 were removed as they indicate inactive or placeholder listings
  
  * Hosts with multiple listings often have greater availability but less frequent reviews, hinting at commercial property management

### 💵 Price Distribution & Influencing Factors
* Majority of listings fall under $200 per night

* Outliers above $500 were treated as luxury or boutique properties, skewing the average price upwards

* Price tends to correlate with:

  - Room type
  
  - Location
  
  - Minimum nights
  
  - Host listing count

### 📝 Reviews & Host Behavior
* Listings with a high number of reviews tend to be lower-priced but consistently booked

* Hosts with multiple properties show more professional behavior but sometimes less personalized guest engagement

### 🔍 Correlation Highlights
Weak but visible correlation between:

  * Availability & Number of reviews (more availability may increase exposure)
  
  * Minimum nights & Price (longer stays may influence pricing strategy)

### 📊 Visualizations Used
  * Box plots: Outlier detection in price, minimum nights
  
  * Heatmaps: Showed correlation between numerical variables
  
  * Bar charts: Distribution of listings across neighborhoods and room types
  
  * Scatter plots: Price vs other variables (e.g., reviews, availability)
  
These insights could be useful not only for travelers deciding where to stay but also for Airbnb hosts and business strategists optimizing listing strategies, pricing, and service offerings.



## 🚀 How to Run This Project

Follow these steps to run the project locally on your machine:

1. **Clone the Repository**

```
git clone https://github.com/yourusername/Airbnb-Booking-Analysis.git
```

2. **Navigate to the project folder**

```cd Airbnb-Booking-Analysis```

3. **Launch the notebook using Jupyter**

```jupyter notebook AirBnB__Booking_Analysis_EDA.ipynb```


## 🙌 Acknowledgements

Thanks to Airbnb and open data platforms for providing the dataset. This project is a part of my Capstone Submission to demonstrate data analysis, visualization, and storytelling skills.






