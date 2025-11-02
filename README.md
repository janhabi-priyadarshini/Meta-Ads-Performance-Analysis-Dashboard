# 📊 Meta Ad Performance Dashboard  

**A Power BI dashboard that analyzes paid ad campaigns on Facebook & Instagram — from impressions to purchases — using Excel for data prep, SQL for modeling, DAX for measures, and Power BI for interactive visualization.**

---

## 📝 Short Description / Purpose
This project presents an end-to-end **Meta Ad Performance Dashboard** that helps marketing teams measure **reach, engagement, conversions, and budget utilization** for paid campaigns on Facebook and Instagram.  
It converts raw event-level data into business-ready KPIs, provides **demographic, geographic, and time-based analysis**, and surfaces actionable insights to improve **ROI and marketing efficiency**.  

---

## 🛠️ Tech Stack
- **Power BI** – Dashboard creation and interactive visualization  
- **DAX (Data Analysis Expressions)** – Used to create custom KPIs such as CTR%, Engagement Rate%, Conversion Rate%, and Purchase Rate%  
- **SQL** – For data modeling, joins, KPI validation, and data quality checks  
- **Excel** – Used for raw data cleaning, preprocessing, and transformation before Power BI import  
- **Data Modeling** – Implemented **Star Schema** (Fact table + Dimension tables) for optimized performance  
- **Documentation Tools** – Used for creating BRD, Domain Knowledge, Dashboard Insights, and Interview Explanation PDFs  

---

## 📂 Data Source
The dataset used in this project is sourced from **Kaggle**:

> 📊 **Dataset:** [Social Media Advertisement Performance](https://www.kaggle.com/datasets/alperenmyung/social-media-advertisement-performance)  
> 👤 **Author:** [Alperen Myung](https://www.kaggle.com/alperenmyung)  
> 🗂️ **Platform:** Kaggle  
> 🧱 **Structure:** The dataset follows a **Star Schema** with four tables — `ad_events`, `ads`, `campaigns`, and `users`.  
> 🧩 **Description:** This dataset represents simulated performance data for paid social media ads, covering impressions, clicks, purchases, demographics, and budget details. It is ideal for marketing analytics, KPI tracking, and dashboard visualization projects.  

| Table | Type | Description |
|--------|------|-------------|
| `ad_events` | Fact | Event-level data (Impressions, Clicks, Shares, Comments, Purchases) |
| `ads` | Dimension | Ad-level details (ad_type, platform, target_gender, target_age_group) |
| `campaigns` | Dimension | Campaign-level details (budget, start/end date, duration) |
| `users` | Dimension | User demographics (age, gender, country, interests) |

---

## 🌟 Features and Highlights

### 🧩 Business Problem
Marketing teams often run multiple ad campaigns across Facebook and Instagram but struggle to identify which platform, format, or audience segment performs best.  
Without consolidated tracking, **budget allocation becomes inefficient**, and conversion rates remain low despite high engagement.

---

### 🎯 Goal of the Dashboard
To build an **interactive performance tracking dashboard** that:
- Monitors the full **marketing funnel** — from Impressions → Clicks → Purchases  
- Identifies top-performing **platforms, age groups, countries, and ad formats**  
- Enables **data-driven decisions** for ad budget optimization and audience targeting  

---

### 📊 Walkthrough of Key Visuals

#### 1. **Top KPI Summary Tiles**
Display overall performance metrics:
- **Impressions:** 216K  
- **Clicks:** 25.4K  
- **CTR:** 11.76% *(above industry average)*  
- **Engagement Rate:** 13.56%  
- **Purchases:** 1.3K  
- **Conversion Rate:** 5.21%  
- **Purchase Rate:** 0.61%  
- **Total Budget:** 2.5M  
- **Average Budget/Campaign:** 50.7K  

> 💡 *These KPIs provide a snapshot of campaign efficiency, showing strong awareness but weak lower-funnel conversions.*

---

#### 2. **Gender-wise Engagement (Donut Chart)**
- Female: **43%** engagement  
- Male: **22%**  
- Others: **35%**  
> 👉 Females engage significantly more — suggesting ad creatives resonate better with female audiences.

---

#### 3. **Age Group Performance (Bar Chart)**
- Highest engagement: **18–30 age group**  
- Sharp decline after 35+  
> 🎯 Focus campaigns on young adults for higher ROI.

---

#### 4. **Geographic Distribution (Map View)**
- **Top Engaged Countries:** India, US, Brazil, Germany, UK  
> 🌎 Target India & Brazil for engagement volume, Germany & UK for premium conversions.

---

#### 5. **Weekly Trend (Stacked Column Chart)**
- Visualizes weekly ad engagement split by **Ad Type**.  
> 📆 Shows consistent weekly engagement and identifies stable pacing.

---

#### 6. **Hourly Engagement Trend (Area Chart)**
- Peak hours: **3 PM – 8 PM**  
- Low activity: **0–5 AM**  
> ⏰ Schedule ad delivery in afternoons/evenings for maximum results.

---

#### 7. **Calendar Heatmap (Monthly View)**
- Highlights dates with high activity (e.g., **19–21, 25–27**)  
> 📅 Identifies spikes caused by campaign launches or promotions.

---

#### 8. **Ad Type Performance (Matrix Table)**
| Ad Type | Impressions | Clicks | CTR | Purchase Rate | Conversion Rate | Engagement Rate |
|----------|-------------|--------|-----|----------------|-----------------|-----------------|
| Carousel | 48K | 6K | 11.7% | 0.59% | 5.1% | 13.4% |
| Image | 51K | 6K | 11.7% | 0.57% | 4.9% | 13.5% |
| Stories | 72K | 8K | 11.8% | 0.65% | 5.2% | 13.6% |
| Video | 46K | 5K | **11.9%** | **0.62%** | **5.2%** | **13.7%** |

> 🎥 **Video ads** perform the best, followed by **Stories**, while Image and Carousel have moderate conversions.

---

### 💼 Business Impact & Insights

1. **Strong Awareness & Engagement:**  
   CTR (11.76%) and Engagement Rate (13.56%) indicate top-performing creatives and audience targeting.  

2. **Weak Conversion Funnel:**  
   Purchase Rate (0.61%) reveals users drop off after engagement — optimize landing pages and retargeting campaigns.  

3. **Audience Strategy:**  
   Focus on **Females aged 18–30**, primarily in **India & Brazil**, for maximum reach and conversion potential.  

4. **Ad Format Optimization:**  
   Shift more budget toward **Video & Story** ads — proven highest ROI formats.  

5. **Timing Optimization:**  
   Deliver ads during **afternoon and evening hours** to leverage peak activity.  

---

## ⚙️ How to Run / Reproduce

1. **Prepare Data:**
   - Place your cleaned CSVs in a `/data` folder:
     ```
     ad_events.csv
     ads.csv
     campaigns.csv
     users.csv
     ```
   - Connect them in Power BI or import into SQL Server/PostgreSQL.

2. **Open Power BI File:**
   - Launch `Meta_Ad_Performance.pbix`  
   - Refresh data connections  
   - Verify KPIs, relationships, and visuals  

3. **Validate Metrics:**
   - Run SQL scripts (included) to verify deduplication, unique user counts, and attribution logic.  

---

## 📁 Repository Structure
