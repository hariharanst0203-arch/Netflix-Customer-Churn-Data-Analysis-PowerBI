# 📊 Netflix User Data Analysis Dashboard – Power BI

## 📌 Project Overview

**Netflix User Data Analysis** is an interactive **Power BI dashboard** designed to analyze Netflix user activity, viewing behavior, ratings, content performance, subscription patterns, and geographic trends.

The dashboard converts user-level viewing data into business-friendly visual insights using interactive filters, KPI cards, charts, and multiple analytical pages.

The project focuses on answering questions such as:

- How many users and titles are represented in the dataset?
- How much total viewing activity is recorded?
- Which genres and countries show higher activity?
- How does watch time vary by rating, age category, content type, and subscription plan?
- How are ratings distributed across users, countries, genres, directors, and cast?
- How does content volume vary by month?
- Which customer segments and content categories require further attention?

---

## 🎯 Business Objective

The primary objective is to build a **self-service analytical dashboard** that helps stakeholders understand Netflix-style user and content performance.

The dashboard can support analysis of:

- User engagement
- Watch-time behavior
- Content consumption
- Rating patterns
- Subscription performance
- Country-level performance
- Genre performance
- Age-category behavior
- Monthly content trends

---

## 🛠️ Tools & Technologies

| Tool / Technology | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard development and data visualization |
| **Power Query** | Data cleaning and transformation |
| **DAX** | Measures, KPIs, calculations, and analytical logic |
| **Data Modeling** | Structuring data for interactive analysis |
| **Excel / CSV Dataset** | Source data, where applicable |

---

## 📂 Dashboard Structure

The report contains multiple interactive analytical pages.

### 1. Executive Overview

The overview page provides a high-level summary of Netflix user and content activity.

### Key KPIs displayed

- **20K** – User Count
- **50M** – Total Views
- **60K** – Total Rating
- **13K** – Shows Watched
- **20K** – Total Titles

### Key Visuals

- Shows Watched by User Type
- Subscription Type by Country
- Watch Time by Rating
- Average Rating by Type
- Total Rating by Country
- Average Rating by User Type

This page is designed to provide a quick executive-level understanding of overall platform activity.

---

### 2. Content & User Analysis

This page focuses on content consumption and user behavior.

### Key Visuals

- Shows Watched and Total Views by Genre
- Watch Time by Show Type
- Country by Subscription Plans
- Watch Time by Title
- User Ratings by Rating Stars
- Year-based filtering

### Observations from the dashboard

- Viewing activity is distributed across multiple genres including **Romance, Action, Horror, Fantasy, Thriller, Sci-Fi, Documentary, and Drama**.
- User ratings are distributed from **1 to 5 stars**, with the dashboard showing the highest displayed count for **5-star ratings at approximately 21K**.
- Watch time varies across individual titles and content types.
- Subscription-plan activity can be compared across countries.

---

### 3. Geographic, Rating & Subscription Analysis

This page provides deeper analysis of ratings, genres, subscription behavior, and monthly title patterns.

### Key Visuals

- Average Rating by Director
- Average Rating by Content Type
- Average Rating by Country
- Average Rating by Genre
- Subscription by Genre
- Title Count by Month

### Dashboard highlights

- The displayed average rating for the top directors ranges from approximately **2.80 to 4.25**.
- Average ratings across the displayed countries are approximately **3**.
- Average ratings across the displayed genres are also approximately **3**.
- Monthly title counts shown on the dashboard range from approximately **1.6K to 1.75K**, depending on the month.

---

### 4. Audience & Performance Analysis

This page focuses on audience segments and country-level performance.

### Key Visuals

- Rating by Month
- Watch Time by Age Category
- Rating by Country Performance
- Rating by Cast
- Rating by Country & Genre
- Watch Time by Subscription Type

### Audience categories

The dashboard analyzes watch time across:

- Teen
- Young Adult
- Middle Age
- Adult
- Senior Citizen

### Dashboard highlights

The displayed watch-time values by age category are approximately:

- **Senior Citizen – 15M**
- **Adult – 11M**
- **Middle Age – 10M**
- **Young Adult – 9M**
- **Teen – 4M**

Among the displayed subscription types, **Standard** shows the highest watch-time bar, followed by **Basic** and **Premium**.

---

## 🎛️ Interactive Features

The dashboard includes interactive slicers for:

- **Genre**
- **Country**
- **Rating**
- **Year**

Users can combine these filters to dynamically explore the data.

For example:

> Select a country → choose a genre → filter by rating → select a year → analyze the resulting watch time, ratings, subscription behavior, and content performance.

The navigation buttons also provide a multi-page dashboard experience.

---

## 📈 Key Analytical Areas

### 👥 User Analysis
- User count
- User type
- Age category
- User rating behavior
- Viewing activity

### 🎬 Content Analysis
- Total titles
- Shows watched
- Content type
- Genre performance
- Title-level watch time
- Monthly title distribution

### ⭐ Rating Analysis
- Rating by month
- Rating by country
- Rating by genre
- Rating by director
- Rating by cast
- User rating distribution

### 🌍 Geographic Analysis
- Country-level ratings
- Subscription plans by country
- Country and genre performance
- Total ratings by country

### 💳 Subscription Analysis
- Basic
- Premium
- Standard
- Watch time by subscription type
- Subscription distribution by country and genre

---

## 💡 Business Insights

Based on the dashboard visuals, several useful analytical observations can be made:

1. **User engagement is substantial**, with the dashboard displaying approximately **20K users** and **50M total views**.

2. **Watch time differs considerably by audience segment**, with Senior Citizens showing the highest displayed watch time among the age categories.

3. **Standard subscription users show the highest displayed watch time** compared with Basic and Premium users.

4. **5-star ratings have the highest displayed rating count**, at approximately **21K**, indicating strong representation of highly rated viewing activity.

5. **Average ratings are relatively consistent across the displayed countries and genres**, generally around **3**.

6. **Director performance varies**, with the displayed average ratings ranging from approximately **2.80 to 4.25**.

7. **Content volume remains relatively consistent across months**, with displayed monthly title counts generally between **1.6K and 1.75K**.

8. **Genre-level analysis provides an opportunity to identify content categories with stronger viewing and rating activity**, which can support content planning and recommendation strategies.

> **Note:** These insights are based on the values and visual patterns displayed in the Power BI dashboard. They should not be interpreted as official Netflix business statistics.

---

## 🧮 Example Power BI Measures

The dashboard can be supported by DAX measures such as:

```DAX
User Count =
DISTINCTCOUNT('Netflix'[User_ID])
```

```DAX
Total Views =
SUM('Netflix'[Total_Views])
```

```DAX
Total Rating =
SUM('Netflix'[Rating])
```

```DAX
Shows Watched =
COUNTROWS('Netflix')
```

```DAX
Average Rating =
AVERAGE('Netflix'[Rating])
```

> Measure names and column names should be adjusted to match the actual dataset/model used in the `.pbix` file.

---

## 🔄 Data Analysis Workflow

The project follows a typical data analytics workflow:

```text
Raw Dataset
     ↓
Data Cleaning & Transformation
     ↓
Data Modeling
     ↓
DAX Measures & KPIs
     ↓
Interactive Visualizations
     ↓
Dashboard Analysis
     ↓
Business Insights
```

### Data Preparation

Typical Power Query preparation includes:

- Removing unnecessary columns
- Handling missing values
- Correcting data types
- Standardizing categorical values
- Creating calculated/derived fields
- Preparing date and categorical fields for analysis

### Data Modeling

The model is structured to support:

- User analysis
- Content analysis
- Rating analysis
- Country analysis
- Subscription analysis
- Time-based analysis

### Visualization

Power BI visuals are used to transform the prepared data into:

- KPI cards
- Bar charts
- Donut charts
- Line charts
- Area charts
- Treemaps / categorical visuals where appropriate
- Interactive slicers

---

## 📸 Dashboard Preview

### Executive Overview

![Netflix Dashboard – Overview](screenshots/overview.png)

### Content & User Analysis

![Netflix Dashboard – Content Analysis](screenshots/content-analysis.png)

### Geographic & Rating Analysis

![Netflix Dashboard – Geographic Analysis](screenshots/geographic-analysis.png)

### Audience & Performance Analysis

![Netflix Dashboard – Audience Analysis](screenshots/audience-analysis.png)

> Create a `screenshots` folder in the GitHub repository and upload the corresponding dashboard images using the filenames above.

---

## 📁 Recommended GitHub Repository Structure

```text
Netflix-User-Data-Analysis/
│
├── README.md
│
├── PowerBI/
│   └── Netflix_User_Data_Analysis.pbix
│
├── Dataset/
│   └── netflix_user_data.csv
│
├── Screenshots/
│   ├── overview.png
│   ├── content-analysis.png
│   ├── geographic-analysis.png
│   └── audience-analysis.png
│
└── Documentation/
    └── project-notes.md
```

If the original dataset is not licensed for redistribution, **do not upload the raw dataset**. Instead, mention the dataset source or provide instructions for obtaining it.

---

## 🚀 How to Use the Dashboard

1. Download or clone this repository.
2. Open the `.pbix` file using **Power BI Desktop**.
3. If required, update the dataset/source path.
4. Refresh the data.
5. Use the **Genre, Country, Rating, and Year** slicers to interact with the report.
6. Navigate between pages using the dashboard navigation buttons.
7. Hover over visuals to view detailed values and comparisons.

---

## 🎓 Skills Demonstrated

This project demonstrates practical skills in:

- Power BI Dashboard Development
- Power Query / ETL
- DAX
- Data Cleaning
- Data Modeling
- KPI Development
- Data Visualization
- Interactive Filtering
- Exploratory Data Analysis
- Business Intelligence
- User & Content Analytics
- Geographic Analysis
- Trend Analysis
- Insight Generation

---

## 📌 Project Outcome

The final dashboard provides a centralized analytical view of user engagement, content consumption, ratings, subscription behavior, demographic segments, and geographic performance.

It demonstrates how raw data can be transformed into an **interactive Business Intelligence solution** that supports data-driven analysis and decision-making.

---

## 👤 Author

**Hariharan S.**

**Aspiring Data Analyst | MCA Graduate**

**Skills:** Power BI • SQL • Excel • Python • Tableau • Data Analysis

---

## ⭐ Project Highlights

**Domain:** Entertainment / Streaming Analytics  
**Project Type:** Business Intelligence & Data Visualization  
**Primary Tool:** Microsoft Power BI  
**Focus:** User Engagement • Content Analytics • Ratings • Subscription • Geographic Analysis

---

## 📄 Disclaimer

This is an **analytical/portfolio project** created for learning and demonstration purposes. The numbers and insights presented in the dashboard represent the underlying project dataset and should not be considered official Netflix corporate statistics.
