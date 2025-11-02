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
**Facebook Dashboard:**
- **Impressions:** 216K  
- **Clicks:** 25.4K  
- **CTR:** 11.76% *(above industry average)*  
- **Engagement Rate:** 13.56%  
- **Purchases:** 1.3K  
- **Conversion Rate:** 5.21%  
- **Purchase Rate:** 0.61%  
- **Total Budget:** 2.5M  
- **Average Budget/Campaign:** 50.7K  

**Instagram Dashboard:**
- **Impressions:** 123.8K  
- **Clicks:** 14.7K  
- **CTR:** 11.86%  
- **Engagement Rate:** 13.60%  
- **Purchases:** 708  
- **Conversion Rate:** 4.82%  
- **Purchase Rate:** 0.57%  
- **Total Budget:** 2.5M  
- **Average Budget/Campaign:** 50.7K  

> 💡 *These KPIs show both platforms deliver strong engagement, but Facebook performs slightly better in conversions.*

---

#### 2. **Gender-wise Engagement (Donut Chart)**
**Facebook:**  
- Female: **43%** engagement  
- Male: **22%**  
- Others: **35%**  

**Instagram:**  
- Female: **37%** engagement  
- Male: **26%**  
- Others: **37%**  

> 👉 On both platforms, female users engage more, but Instagram shows a slightly more balanced gender distribution.

---

#### 3. **Age Group Performance (Bar Chart)**
- Highest engagement: **18–30 age group** for both platforms  
- Engagement decreases steadily beyond age 35  
> 🎯 Focus on younger audiences for both Facebook and Instagram campaigns.

---

#### 4. **Geographic Distribution (Map View)**
**Facebook:** India, US, Brazil, Germany, UK  
**Instagram:** India, US, Indonesia, France, Canada  
> 🌎 Target India and US for scale; consider regional strategy differences across Europe and Asia.

---

#### 5. **Weekly Trend (Stacked Column Chart)**
Shows weekly engagement split by **Ad Type** across both platforms.  
> 📆 Engagement remains steady through the month with peak weeks aligning to campaign launches.

---

#### 6. **Hourly Engagement Trend (Area Chart)**
- Peak hours: **3 PM – 8 PM** for both platforms  
- Low activity: **0–5 AM**  
> ⏰ Optimal posting time for ad delivery is afternoon to evening for maximum impressions.

---

#### 7. **Calendar Heatmap (Monthly View)**
Highlights top-performing campaign dates across both platforms (e.g., 19–21, 25–27).  
> 📅 Consistent activity patterns indicate stable pacing and audience interest.

---

#### 8. **Ad Type Performance (Matrix Table)**
| Platform | Ad Type | Impressions | Clicks | CTR | Purchase Rate | Conversion Rate | Engagement Rate |
|-----------|----------|-------------|--------|-----|----------------|-----------------|-----------------|
| Facebook | Carousel | 48K | 6K | 11.7% | 0.59% | 5.1% | 13.4% |
| Facebook | Stories | 72K | 8K | 11.8% | 0.65% | 5.2% | 13.6% |
| Facebook | Video | 46K | 5K | 11.9% | 0.62% | 5.2% | 13.7% |
| Instagram | Carousel | 12.8K | 1.5K | 11.69% | 0.54% | 13.66% | 4.60% |
| Instagram | Image | 12.3K | 1.5K | 12.14% | 0.56% | 13.89% | 4.62% |
| Instagram | Stories | 12.4K | 1.4K | 11.23% | 0.61% | 12.94% | 5.46% |
| Instagram | Video | 3.3K | 0.4K | 11.88% | 0.66% | 13.71% | 5.56% |

> 🎥 **Video ads** lead in performance on both platforms, showing the highest engagement and conversion rates.

---

### 💼 Business Impact & Insights

1. **Strong Awareness & Engagement:**  
   CTR (11.76% Facebook, 11.86% Instagram) and Engagement Rate (~13.5%) show that both platforms are delivering excellent top-of-funnel performance.

2. **Conversion Opportunity:**  
   Facebook shows slightly better conversion (5.21%) than Instagram (4.82%), suggesting better retargeting potential on Facebook.

3. **Audience Strategy:**  
   Target **Females aged 18–30** on both platforms for optimal engagement.

4. **Ad Format Optimization:**  
   Continue focusing on **Video and Stories**, which perform best across platforms.

5. **Budget Strategy:**  
   Maintain balanced investment across Facebook and Instagram but allocate a slightly higher share to Facebook for conversion-driven campaigns.

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

## 🖼️ Screenshots of the Dashboards

Below are the visual previews of both **Facebook** and **Instagram** ad performance dashboards built in Power BI.  
Together, they provide a complete view of Meta’s ad ecosystem — tracking KPIs, engagement, and conversions separately for each platform.

### 📘 Facebook Dashboard
![Facebook Dashboard Screenshot](https://github.com/janhabi-priyadarshini/Meta-Ads-Performance-Analysis-Dashboard/blob/main/Snapshot%20of%20the%20Dashboard.png)

---

### 📸 Instagram Dashboard
![Instagram Dashboard Screenshot](https://github.com/janhabi-priyadarshini/Meta-Ads-Performance-Analysis-Dashboard/blob/main/Snapshot%20of%20Instagram%20Dashboard.png )

---

> 💡 *These dashboards together help compare performance between Facebook and Instagram ads — identifying which platform, audience, and ad type delivers the best ROI.*

---

## 🧠 Business Documents Included
- **Business Requirements Document (BRD):** Defines KPIs, metrics, and visual requirements.  
- **Domain Knowledge Document:** Explains table design and star schema relationships.  
- **Dashboard Insights:** Summarizes performance results, key takeaways, and recommendations.  
- **Project Explanation (Interview):** A step-by-step breakdown for interviews or presentations.  

---

## 🚀 Key Takeaways
- Facebook slightly outperforms Instagram in conversions.  
- Video and Story Ads dominate on both platforms.  
- Females aged 18–30 remain the most engaged audience.  
- Both dashboards offer unified insight into campaign efficiency and audience behavior.  

---

## 🪄 Future Improvements
- Integrate real-time campaign data via Meta Ads API  
- Add ROI, ROAS, and CPC metrics for financial insights  
- Include user retention and lifetime value (LTV) tracking  
- Automate data refresh and quality validation via Power BI Gateway  

---

⭐ **If you found this project insightful, don’t forget to star the repository!**  
📈 *This dashboard demonstrates how data storytelling transforms marketing performance into measurable business strategy.*
