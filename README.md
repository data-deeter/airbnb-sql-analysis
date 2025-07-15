# Airbnb NYC Listings – SQL Data Exploration

## 📊 Overview
This project uses SQL to explore and analyze a dataset of Airbnb listings in New York City. The goal is to uncover insights about pricing, availability, and listing trends by neighborhood.

Dataset: [NYC Airbnb Open Data](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data)

## 🔧 Tools Used
- SQL (Mode/SQLite/PostgreSQL)
- Basic aggregation and filtering
- GitHub for project documentation

## 🔍 Key Questions Answered
- What is the average price per night across neighborhoods?
- Which neighborhoods have the most listings?
- What types of listings are most common?
- How do review counts vary by listing type?

## 📁 Files
- `queries.sql`: The SQL queries used to analyze the dataset
- `summary.md`: Notes and summaries of key findings
- `screenshots/`: Optional visual exports from Mode or DB Browser

## 📌 Example Query
```sql
SELECT neighborhood_group, AVG(price) AS avg_price
FROM airbnb_listings
GROUP BY neighborhood_group
ORDER BY avg_price DESC;
