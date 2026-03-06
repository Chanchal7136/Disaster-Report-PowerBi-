#  Global Disaster Response Analysis (Power BI Dashboard)
Global Disaster Response Analysis Dashboard built in Power BI to analyze disaster trends, response performance, economic losses, and aid distribution (2018–2024).

## 📊 Project Overview
The **Global Disaster Response Analysis Dashboard** is an interactive Power BI project designed to analyze worldwide disaster events and evaluate response performance, recovery efficiency, and aid distribution.

This dashboard helps identify patterns in disaster impact, response efficiency, funding allocation, and recovery timelines. It provides meaningful insights that can help policymakers, humanitarian organizations, and analysts make data-driven decisions during disaster management.

---

## 🎯 Objectives
- Analyze disaster trends across **regions and countries**
- Evaluate **response performance and efficiency**
- Understand **casualties and economic losses**
- Examine **aid and funding distribution**
- Forecast future disaster trends and recovery patterns

---

## 🗂 Dataset Description
The dataset includes global disaster data from **2018 to 2024**, containing information such as:

- Disaster Type
- Date and Time
- Country and Region
- Casualties and Affected Population
- Economic Loss
- Response Time
- Recovery Duration
- Aid Amount
- Efficiency Score
- Geographic Coordinates (Latitude, Longitude)

---

# 📑 Dashboard Pages

## 1️⃣ Global Overview
This page provides a high-level overview of global disaster events.

**Visuals Included**
- KPI Cards
  - Total Disasters
  - Total Casualties
  - Total Economic Loss
  - Average Response Time
- Disaster Trend by Year (Line Chart)
- Disaster Distribution by Type (Donut Chart)
- Economic Loss by Region (Bar Chart)
- Global Map of Disaster Events

---

## 2️⃣ Regional & Country Analysis
This page focuses on disaster impact at regional and country levels.

**Visuals Included**
- Region/Country Filtered KPI Cards
- Bubble Map  
  - Bubble Size → Casualties  
  - Color → Average Efficiency Score
- Stacked Bar Chart  
  - Disaster Type vs Count and Economic Loss
- Matrix Table  
  - Year × Disaster Type  
  - Casualties and Economic Loss with Conditional Formatting

---

## 3️⃣ Response Performance
This page analyzes the effectiveness of disaster response.

**Visuals Included**
- KPI Cards
  - Average Response Time
  - Median Response Time
  - % Responses Within SLA (≤ 72 Hours)
- Scatter Plot
  - X → Response Time
  - Y → Recovery Duration
  - Bubble Size → Economic Loss
  - Color → Efficiency Score
- Box Plot
  - Response Time by Region and Disaster Type
- Timeline Chart
  - Average Efficiency Score
  - Aid Amount Over Time

---

## 4️⃣ Aid & Funding Analysis
This page examines how disaster aid is distributed and utilized.

**Visuals Included**
- KPI Cards
  - Total Aid
  - Aid per Casualty
  - Aid per Disaster
- Waterfall Chart
  - Aid Sources vs Aid Uses
- Treemap
  - Aid by Donor Country / Organization
- Map Visualization
  - Aid per Affected Person

---

## 5️⃣ Recovery & Forecasting (What-If Analysis)
This page focuses on recovery timelines and predictive insights.

**Visuals Included**
- Recovery Duration KPI by Disaster Severity
- Decomposition Tree
  - Key Drivers of Recovery Duration
- Forecasting Line Chart
  - Disaster Counts or Economic Loss Forecast
- Scenario Analysis
  - Impact of Faster Response Time on Recovery Duration

---

# 🛠 Tools & Technologies
- **Power BI**
- **Data Modeling**
- **DAX (Data Analysis Expressions)**
- **Data Cleaning & Transformation**
- **Forecasting & What-If Analysis**

---

# 🔄 Data Preparation Steps
The following preprocessing steps were performed:

1. Data cleaning and handling missing values
2. Changing column data types
3. Creating calculated columns
4. Creating a **Date Table**
5. Building relationships between tables
6. Creating DAX measures for KPIs

Example Date Table:

```DAX
DateTable =
ADDCOLUMNS(
    CALENDAR(MIN(Data[date]), MAX(Data[date])),
    "Year", YEAR([Date]),
    "Month", FORMAT([Date], "MMM"),
    "MonthNo", MONTH([Date])
)
```

---

# 📈 Key Insights
- Certain regions experience **higher disaster frequency**
- Faster response times significantly reduce **recovery duration**
- Economic loss varies significantly depending on **disaster type**
- Aid distribution is uneven across regions

---

# 🚀 How to Use
1. Download the `.pbit` or `.pbix` file
2. Open it using **Power BI Desktop**
3. Refresh the dataset if needed
4. Interact with filters and slicers to explore insights

---



---

# 📬 Contact

**Chanchal Vijay Bhangale**

📧 Email: your-email@example.com  
🔗 LinkedIn: https://www.linkedin.com/  
💻 GitHub: https://github.com/Chanchal7136

---

⭐ If you found this project useful, consider giving it a **star on GitHub!**
