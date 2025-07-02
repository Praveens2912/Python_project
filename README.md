# Python_project

# 🏙 Airbnb Data Analysis — NYC 2024

---

##  Overview

This project explores Airbnb listings data from New York City to extract insights using **Python**. With tools like **Pandas**, **Seaborn**, and **Matplotlib**, we perform a full **data exploration and visualization pipeline**, identifying trends in pricing, availability, and review behavior across boroughs.

 Technologies Used:  
`Pandas`, `NumPy`, `Seaborn`, `Matplotlib`, `Jupyter Notebook / VS Code`

---

##  Goals

- Examine pricing patterns across different room types and boroughs
- Understand host activity and availability
- Detect pricing anomalies and visualize them
- Help users and hosts make data-informed decisions

---

## Dataset
The dataset contains **20,765 entries and 22 features**, including:
- **id**: Unique identifier for each listing  
- **name**: Title of the Airbnb listing  
- **host_name**: Name of the host  
- **neighborhood_group**: Group (borough) where the listing is located  
- **latitude/longitude**: Geolocation of listings  
- **price**: Nightly rental price  
- **room_type**: Type of accommodation (e.g., entire home, private room)  
- **reviews_per_month**: Average monthly reviews for the listing  
- **availability_365**: Number of available days in the year  

---

##  Analysis Steps

###  1. Data Cleaning
- Removed null entries
- Converted dates (e.g. `last_review`) into `datetime`
- Capped extreme `price` values above 1000 to remove noise

###  2. Visual Exploration
- **Bar Charts**: Show room type and borough popularity
- **Histograms**: Display pricing distribution
- **Boxplots**: Spot outliers in listing prices
- **Pairplots & Heatmaps**: Understand relationships between key numerical features

---

##  Highlights

- **Entire homes/apts** dominate listings, especially in Manhattan
- **Price outliers** (e.g., $10,000/night listings) are present and need to be filtered
- **Listings with more reviews** tend to be more available and lower in price
- **Manhattan** is the most expensive borough; **Bronx** and **Staten Island** are cheaper
- Some hosts manage multiple listings, suggesting professional rentals

---

## Key Findings and Insights
1. **Price Trends**:  
   - **Manhattan** has the most expensive listings, followed by Brooklyn.  
   - **Entire homes/apartments** cost significantly more than private or shared rooms.  

2. **Room Type Distribution**:  
   - **Entire homes/apartments** are the most common, but **private rooms** offer budget-friendly options.

3. **Outliers in Price**:  
   - Few listings priced at **$10,000+** were detected, indicating the need to filter such extreme values.

4. **Availability Patterns**:  
   - Listings with **high availability** tend to have lower prices and more reviews, likely due to better guest experience.

5. **Host Behavior**:  
   - Some hosts manage **multiple listings**, indicating a trend toward professional hosting.

---

## How to Run This Project
1. Clone the repository:
   ```bash
   git clone https://github.com/najirh/Python-Project-P2-New-York-AirBnb-Listing-2024.git
   ```
2. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Run the **Jupyter notebook** or **Python script**:
   ```bash
   jupyter notebook day23_airbnb_eda.ipynb
   ```

---

## Recommendations
- **For Guests**: 
   - Look for listings with high availability and good reviews for a better experience.
   - **Private rooms** in Brooklyn offer affordable stays compared to Manhattan.

- **For Hosts**:  
   - Improve **availability** and **review response rates** to attract more bookings.
   - Manage pricing effectively to compete within the borough's market.

---

## Future Work
- Use **machine learning** to predict prices based on room type and location.
- Perform **sentiment analysis** on reviews to better understand guest experiences.
- Create an **interactive dashboard** using Plotly or Tableau for live monitoring.

---

## Conclusion
This project offers valuable insights into the New York Airbnb market, helping both guests and hosts make informed decisions. By using **EDA techniques**, we identified key trends and developed actionable recommendations. Future improvements can involve advanced analytics and predictive modeling to further enhance the findings.
