# Netflix Top 10 English Films Analysis  
*Yipit Data Assessment Project – Data Cleaning, Analysis, and Visualization*

## Description
This project replicates a **Yipit Data Support Specialist** assessment, analyzing Netflix Top 10 English films and reviewing a subscriber trends chart.  

**Part 1** uses **web-scraped Netflix viewership data** combined with **IMDb ratings** to:  
- Identify the film with the most Top 10 appearances and its average weekly hours viewed.  
- Find the lowest-rated English film and its average weekly hours viewed.  

**Part 2** reviews a Netflix subscriber joins vs cancels chart to detect potential errors (e.g., axis mismatches, missing data) and assess whether the trends reflect positively or negatively on Netflix, with recommendations for improvement.  

The dataset excludes the week of **May 22, 2022** due to incomplete `weekly_hours_viewed` data. The analysis demonstrates skills in **data cleaning, exploratory analysis, visualization, and data storytelling**—applicable across analytics, business intelligence, and investment research roles.  

---

## Background
**Yipit Data** is the on-demand data team for leading institutional investors, identifying, licensing, cleaning, and analyzing alternative datasets to generate actionable insights.  

Netflix, Inc. is an American streaming and production company that publishes its **Top 10 titles weekly**. These are split into:  
- Films (English)  
- Films (Non-English)  
- TV (English)  
- TV (Non-English)  

Yipit Data scrapes Netflix’s Top 10 weekly and supplements it with IMDb ratings, enabling deeper analysis into questions such as:  
- Is Netflix producing engaging content?  
- Are investments in new genres/geographies generating significant viewership?  
- How are viewership trends influencing subscriber numbers?  

---

## Part 1 – Analysis & Results

### Q1: Film with the Most Appearances (English Films)
- **Title:** *Sonic the Hedgehog*  
- **Number of Weeks in Top 10:** 7  
- **Average Weekly Hours Viewed:** ~8.55 million  

### Q2: Film with the Lowest IMDb Rating (English Films)
- **Title:** *365 Days: This Day*  
- **IMDb Rating:** 2.5  
- **Average Weekly Hours Viewed:** ~38.70 million  

---

## Part 2 – Chart Review & Insights
![Subscriber Trends Chart Review](https://github.com/Nandini2233/YipitData_Netflix_Project/blob/main/Chart%20for%20Q%233.png)
### Issues Identified
1. **Tooltip vs Y-Axis Mismatch** – Plotted lines don’t align with their tooltip values.  
2. **Suspicious Zero Values** – Dec 2024 shows 0 joins/cancels, likely due to missing data.  
3. **Dual Y-Axis Misleading** – Different scales distort visual comparisons.  
4. **Missing Time Periods** – Gaps reduce reliability of trends.  

### Overall Reflection for Netflix
Despite the chart flaws, joins consistently outpaced cancels in mid/late 2023, indicating **positive subscriber growth**.  

### Recommendations
- Align plotted values with tooltips.  
- Replace zero placeholders with missing data indicators.  
- Use a single normalized Y-axis.  
- Add a net growth trend line.  

---

## Visualizations

### 1. Top 10 English Films by Avg Weekly Hours Viewed
![Top 10 English Films by Avg Weekly Hours Viewed](https://github.com/Nandini2233/YipitData_Netflix_Project/blob/main/Top%2010%20films%20SS.png)

---

## Methodology
1. **Data Loading & Validation** – Loaded Excel file with separate sheets for Netflix Top 10 and IMDb ratings; validated critical columns.  
2. **Cleaning & Filtering** – Removed outage week (2022-05-22), filtered IMDb ratings to 1–10, optimized data types.  
3. **Merging Datasets** – Joined Netflix Top 10 and IMDb ratings for combined analysis.  
4. **Analysis** – Calculated frequency of appearances, average weekly hours viewed, and lowest ratings.  
5. **Visualization** – Created bar charts with IMDb ratings as color hue to highlight quality vs popularity.  
6. **Chart Audit** – Reviewed subscriber trends chart for accuracy and visual clarity.  


