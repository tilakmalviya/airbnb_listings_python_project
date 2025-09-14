### Airbnb Listings EDA – New York 2024

---

## Project Overview

This is my personal data analysis project where I perform **Exploratory Data Analysis (EDA)** on New York Airbnb data. The goal is to explore patterns in listings, analyze prices, understand host behaviors, and gain insights into the Airbnb market using **Python libraries such as Pandas, Numpy, Matplotlib, and Seaborn**.

![](assets/nyc.jpg)  
![](assets/airbnb.jpg)

---

## Objective

The main objectives of this project are:

1. Explore **room types, prices, and availability** across boroughs.
2. Analyze **host behavior and listing patterns**.
3. Detect **outliers** in price data.
4. Provide **actionable recommendations** for both guests and hosts.

---

## Dataset

The dataset contains **20,765 entries and 22 features**, including details such as:

- **id**: Unique identifier for each listing
- **name**: Title of the Airbnb listing
- **host_name**: Name of the host
- **neighborhood_group**: Borough of New York where the listing is located
- **latitude/longitude**: Geolocation of listings
- **price**: Nightly rental price
- **room_type**: Type of accommodation (e.g., entire home, private room)
- **reviews_per_month**: Average monthly reviews
- **availability_365**: Days available in a year

Dataset source: [Inside Airbnb](http://insideairbnb.com/get-the-data/)

---

## Project Structure

```
airbnb_listings_python_project/
│
├── data/                # Raw dataset files
├── notebooks/           # Jupyter notebooks for EDA
├── scripts/             # Python scripts (data cleaning, visualization)
├── images/              # Visualizations and plots
├── assets/              # Project-related images (e.g., nyc.jpg, airbnb.jpg)
├── README.md            # Project documentation
└── requirements.txt     # Dependencies
```

---

## Steps and Workflow

### 1. Data Cleaning

- Handled missing values in `price`, `neighborhood`, and `beds` columns.
- Converted `last_review` into a proper **datetime** format.
- Managed extreme outliers (e.g., listings above $1,000/night).

### 2. Exploratory Data Analysis

- **Room Type Distribution**: Bar plots to visualize the popularity of different room types.
- **Neighborhood Insights**: Compared average prices across boroughs.
- **Availability Trends**: Used heatmaps to check correlations among availability, price, and reviews.
- **Price Distribution**: Histograms to analyze how most listings are priced.
- **Host Analysis**: Boxplots to identify hosts managing multiple listings.

### 3. Data Visualization

- **Histograms & Boxplots**: To check price distributions and detect outliers.
- **Heatmaps**: To understand feature correlations.
- **Bar Charts**: To show counts of room types and neighborhoods.
- **Pair Plots**: To visualize relationships between reviews, availability, and price.

---

## Key Insights

1. **Manhattan** has the most expensive listings, while **Brooklyn** offers more affordable stays.
2. **Entire homes/apartments** dominate the market but **private rooms** are budget-friendly.
3. Outliers exist with listings priced extremely high (e.g., $10,000+).
4. Listings with higher availability tend to receive more reviews, likely due to more guest exposure.
5. Certain hosts manage multiple properties, showing a shift towards professional hosting.

---

## How to Run This Project

1. Clone the repository:
   ```bash
   git clone https://github.com/tilakmalviya/airbnb_listings_python_project.git
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Run the notebook or script:
   ```bash
   jupyter notebook airbnb_eda.ipynb
   ```

---

## Recommendations

- **For Guests**: Look at availability and reviews before booking. Private rooms in Brooklyn are a great budget option.
- **For Hosts**: Keep listings available consistently and maintain good review scores to attract more bookings.

---

## Future Work

- Use **machine learning** models to predict prices.
- Perform **sentiment analysis** on guest reviews.
- Build an **interactive dashboard** with Streamlit or Plotly.

---

## Conclusion

This project highlights trends in the Airbnb market for New York, offering insights that benefit both hosts and guests. Through EDA, we uncovered patterns in room types, pricing, and availability. Future enhancements could make this analysis more predictive and interactive.

---

## License

This project is open-source and licensed under the [MIT License](https://opensource.org/licenses/MIT).

---

## Contact

- **GitHub**: [tilakmalviya](https://github.com/tilakmalviya)
- **LinkedIn**: [Tilak Malviya](https://www.linkedin.com/in/tilak-malviya-6596512b8/)
