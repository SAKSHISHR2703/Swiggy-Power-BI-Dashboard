# 🛵 Swiggy Power BI Dashboard

> **"Swiggy Karo, Phir Jo Chahe Karo!"** — A comprehensive end-to-end data analytics project built on Swiggy's food delivery dataset.

---

## 📌 Project Overview

This Power BI project analyzes Swiggy's food delivery operations across Indian cities, providing actionable insights into sales performance, user demographics, city-level trends, and food category preferences.

---

## 📊 Dashboard Pages

| Page | Description |
|------|-------------|
| **Overview** | High-level KPIs: Orders Count, Users Count, Sales by Food Type |
| **User Performance** | Demographics breakdown — age, gender, occupation, marital status |
| **City Overview** | Top N cities by sales with interactive slicer (Top 5, 10, 20, 30, 100) |
| **Sales Trends** | Year-over-year quantity and amount analysis (2017–2020) |

---

## 🗂️ Data Model

### Tables

| Table | Rows | Key Columns |
|-------|------|-------------|
| **Orders** | 297,154 | order_date, User_id, Restaurant_id, City, Type, Value, Year |
| **Menu** | 1,048,574 | Menu_id, Restaurant_id, Food_id, Cuisine, Price, FoodType |
| **Food** | — | Food_id, Item, Food_Type |
| **Users** | 100,000 | User_id, Name, Age, Gender, Marital Status, Occupation, Rank, Total_Sales |

### Relationships
- `Orders[User_id]` → `Users[User_id]`
- `Orders[Restaurant_id]` → `Menu[Restaurant_id]`
- `Menu[Food_id]` → `Food[Food_id]`

---

## 📈 Key KPIs

| Metric | Value |
|--------|-------|
| Total Orders | **149K** |
| Total Users | **100K** |
| Top 10% Customer Revenue | **724.92M** |
| Veg Sales | **122M** |
| Non-Veg Sales | **106M** |
| Others Sales | **24M** |

---

## 🏙️ Top Cities by Sales (Top 10)

1. Tirupati — **43M**
2. Electronic City, Bangalore — **29M**
3. Baner, Pune — **27M**
4. Raipur — **23M**
5. Malviya Nagar — **17M**
6. Sultanpur — **15M**
7. Vastrapur, Ahmedabad — **13M**
8. Indirapuram — **13M**
9. Navrangpura — **12M**
10. Rohini, Delhi — **12M**

---

## 🔑 Key Insights

- 📍 **Tirupati** leads in total order amount at ₹43M
- 🥗 **Vegetarian** food dominates with ₹122M (7.2% more than non-veg)
- 📅 **2018** saw a massive 356% sales spike vs. previous year
- 👨‍🎓 **Ages 21–25 students** are the highest ordering demographic
- 👑 **Top 10% customers** account for **80% of total sales**
- 🏙️ **Bikaner** has the highest user count, rating count, and order count

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Dashboard development & visualization |
| **DAX** | Custom measures and calculated columns |
| **Power Query (M)** | Data transformation and cleaning |
| **Data Modeling** | Star schema design |

---

## 📁 File Structure

```
Swiggy-PowerBI/
│
├── SWIGGY.pbix              # Main Power BI file
├── README.md                # Project documentation
├── data/
│   ├── orders.csv
│   ├── menu.csv
│   ├── food.csv
│   └── users.csv
└── docs/
    ├── project_overview.pdf
    ├── business_problem.pdf
    └── presentation.pptx
```

---

## 🚀 How to Run

1. Open `SWIGGY.pbix` in **Power BI Desktop** (version 2.x or later)
2. Refresh data connections if prompted
3. Navigate through dashboard pages using the left sidebar icons
4. Use the **Top N slicer** to filter city-level data (Default / Top 5 / 10 / 20 / 30 / 100)
5. Toggle between **Amount** and **Quantity** views in the Overview page

---

## 👤 Author

**Sakshi Sharma**  


