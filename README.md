# 🍽️ Zomato Restaurant Data Analysis

An end-to-end data analysis project exploring **9,551 restaurants** across multiple countries using **SQL, Excel, and Power BI**. The project covers the full analytics workflow: database design and querying, exploratory analysis in Excel, and an interactive Power BI dashboard for visual storytelling.

## 📌 Project Overview

This project analyzes restaurant listing data (originally sourced from Zomato) to uncover patterns in cuisine popularity, pricing, ratings, delivery options, and geographic distribution. It's designed to demonstrate practical skills across the data analytics toolchain — from raw data to relational database to business-ready dashboard.

## 🛠️ Tools & Skills Used

| Tool | Purpose |
|---|---|
| **MySQL** | Relational schema design, primary/foreign key relationships, data querying |
| **Microsoft Excel** | Data cleaning, pivot tables, exploratory analysis |
| **Power BI** | Interactive dashboard and data visualization |

## 📂 Repository Structure

```
zomato-restaurant-analysis/
│
├── data/
│   ├── Zomato Dataset.xlsx        # Cleaned dataset with Calendar, Country, Currency dimension tables
│   └── Zomato data.sql            # SQL schema (restaurants + country tables, PK/FK relationships)
│
├── analysis/
│   └── zomato reataurants analysis in Excel (1).xlsx   # Excel-based exploratory analysis & pivot tables
│
├── dashboard/
│   └── ZOMATO DASHBOARD.pbix      # Interactive Power BI dashboard
│
├── assets/                        # Dashboard screenshots (add your own, see below)
│
└── README.md
```

## 🔎 Key Insights

- **9,551 restaurants** analyzed across **15 countries**, with **India** accounting for the vast majority (8,652 listings), followed by the United States, United Kingdom, UAE, and Brazil.
- **New Delhi, Gurgaon, and Noida** are the top three cities by restaurant count, reflecting the dataset's strong concentration in the Delhi NCR region.
- **North Indian (3,960), Chinese (2,735), and Fast Food (1,986)** are the most common cuisines on the platform.
- Only **~26% of restaurants** offer online delivery, and just **~12%** support table booking — highlighting the low digital adoption at the time the data was collected.
- The average restaurant rating across the dataset is **2.89 / 5**, with a full breakdown of rating distribution available in the dashboard.

## 🗃️ Database Design (SQL)

The SQL schema models restaurants and their attributes in a normalized structure:
- `sheet1` — core restaurant table (name, location, cuisine, cost, rating, votes, etc.)
- `sheet2` — country reference table
- A foreign key relationship links each restaurant to its country via `country_code`

## 📊 Dashboard

The Power BI dashboard (`ZOMATO DASHBOARD.pbix`) brings the analysis together into an interactive view covering:
- Restaurant distribution by country and city
- Cuisine popularity
- Price range and cost analysis
- Rating distribution
- Online delivery & table booking adoption

> 💡 **Tip:** Open the `.pbix` file in Power BI Desktop, then export a screenshot or short screen recording of the dashboard and drop it into the `assets/` folder. Add it to this README with:
> `![Dashboard Screenshot](assets/dashboard-screenshot.png)`
> A visual preview is one of the first things recruiters look at, so this is worth doing before sharing the link on LinkedIn.

## 🚀 How to Use

1. **SQL**: Import `data/Zomato data.sql` into MySQL to recreate the database and explore it with your own queries.
2. **Excel**: Open `analysis/zomato reataurants analysis in Excel (1).xlsx` to review the exploratory analysis and pivot tables.
3. **Power BI**: Open `dashboard/ZOMATO DASHBOARD.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free) to interact with the live dashboard.


