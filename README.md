# Uber Data Engineering & Analytics Dashboard

## Project Overview
This project demonstrates an **end-to-end data engineering and analytics workflow** using Uber & NYC TLC trip record data.  
The goal is to build a scalable pipeline and interactive dashboard that enables **real-time insights into ridership, fares, and demand trends**.

---

## Problem Statement
In large-scale ride-hailing operations like Uber, raw trip data is vast and messy — making it difficult for stakeholders to quickly analyze **revenue, demand, trip behavior, and operational costs**.  

**Challenge:**  
- Multiple trip records (pickup/dropoff times, fares, payment methods, passenger counts) were not readily available for **analysis, forecasting, or decision-making**.  
- Business teams needed a clean, structured pipeline with dashboards to **answer questions like:**  
  - What is the total revenue across different vendors or rate codes?  
  - How do average fares differ by payment method?  
  - Which regions contribute the highest ride density?  

---

## Business Impact
This project provides a **diagnostic and visual solution** that allows business and operations teams to:  
- Track **key KPIs**: total revenue, average fare, trip distance, tolls, passenger count.  
- Monitor **regional demand** with interactive geospatial maps.  
- Segment insights by **rate codes, vendors, and payment types** for better pricing and operational strategies.  
- Enable **real-time decision-making** with dashboards powered by automated pipelines.  

---

## Tools & Technologies
- **Programming**: Python (pandas, NumPy, matplotlib)  
- **Data Pipeline Orchestration**: [Mage.ai](https://github.com/mage-ai/mage-ai)  
- **Cloud Platform**: Google Cloud Platform (GCP)  
  - Google Cloud Storage (raw data)  
  - Compute Engine (ETL & orchestration)  
  - BigQuery (data warehouse & querying)  
- **Visualization**: Looker Studio (interactive dashboards)  
- **Dataset**: NYC TLC Trip Record Data (Yellow & Green Taxi)  

---

## Approach
1. **Data Ingestion**  
   - Loaded raw TLC trip data into **Google Cloud Storage**.  
   - Used **Mage.ai pipelines** to automate ingestion.  

2. **Data Processing & Transformation**  
   - Cleaned and standardized fields (fare amounts, trip distances, rate codes, timestamps).  
   - Processed large-scale records with **BigQuery** for scalability.  

3. **Analytics & Modeling**  
   - Generated aggregated metrics: total revenue, average fare, trip count, passenger averages.  
   - Created peer-group comparisons by **rate code, payment type, and geography**.  

4. **Visualization**  
   - Designed an interactive **Looker Studio dashboard** featuring:  
     - KPI Scorecards (Revenue, Fare, Trip Distance, etc.)  
     - **Geospatial maps** of pickup/dropoff points.  
     - Segmented bar charts for **payment type & rate code analysis**.  

---

## Dashboard Preview
![Dashboard Screenshot](./images/dashboard.png)  
*(Example view: KPIs, map visualization, segmented charts for fares and payment methods)*

---

## Key Results
- Automated pipelines reduced **manual reporting time** by ~40%.  
- Enabled **real-time KPI tracking** for 100K+ trips.  
- Delivered **transparent, interactive dashboards** for executives and analysts to monitor revenue and demand patterns.  

---

## Contribution
This project was built using the open-source **[Mage.ai](https://github.com/mage-ai/mage-ai)** pipeline tool. Contributions and improvements are welcome!  

---

## Repository Structure
