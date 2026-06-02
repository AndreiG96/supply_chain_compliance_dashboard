# 🚚 Global Transportation Compliance and Performance Analysis

## 📌 Project Overview
This project showcases a Power BI dashboard designed to analyze transportation compliance and delivery performance across logistics operations.

The solution transforms raw shipment data into actionable insights, enabling stakeholders to monitor on-time performance, identify delays, and evaluate carrier and lane efficiency.

---

## 🎯 Objectives
- Track **On-Time Delivery (OTD)** performance
- Identify **non-compliant shipments and delay patterns**
- Analyze **carrier and lane performance**
- Highlight **regional discrepancies**
- Provide **actionable insights for operational improvement**

---

## 📊 Key Metrics
- On-Time Delivery %
- Average Delay (days)
- Delay Distribution
- Compliance Rate
- Shipments Volume
- Performance by Carrier / Region / Mode

---

## 🧠 Data Model
The dashboard follows a **star schema** design:

### Fact Table
- `Fact_Shipments`

### Dimension Tables
- `Dim_Date`
- `Dim_Origin`
- `Dim_Destination`
- `Dim_Carrier`
- `Dim_Product`
- `Dim_Equipment`

### Key Calculations (DAX)
- `delay_days = actual_delivery_date - planned_delivery_date`
- `is_compliant = IF(delay_days <= 0, "Y", "N")`

---

## 📈 Dashboard Features

### 🔹 Overview
- Executive-level snapshot of transportation compliance performance
- Regional comparison of On-Time Delivery against defined target thresholds
- Product category analysis highlighting delay drivers across key segments
- Shipment volume distribution by destination region to contextualize performance
- Identification of underperforming carriers contributing to compliance gaps
- Combines KPI monitoring with comparative analysis to enable fast, data-driven decision making

### 🔹 Compliance
- Focused analysis of transportation compliance against target performance thresholds
- Regional benchmarking of On-Time Delivery to identify underperforming geographies
- Identification of critical trade lanes contributing to total delay accumulation
- Breakdown of delay impact through Total Delay Days and Delay per Shipment metrics
- Enables root cause analysis by linking regional performance to specific origin–destination routes
- Supports prioritization of corrective actions by quantifying operational impact at lane level

### 🔹 Trends
- Time-series analysis of On-Time Delivery performance across months
- Monitoring of compliance stability and identification of seasonal or structural shifts
- Correlation between On-Time Delivery rates and total delay volume over time
- Detection of performance degradation periods and recovery patterns
- Supports proactive decision-making by highlighting emerging risks and trends
- Enables longitudinal analysis to assess the impact of operational change


### 🔹 Shipments
- Operational view enabling granular shipment-level analysis
- Regional distribution of total and non-compliant shipments
- Identification of high-risk regions contributing to delays
- Trade lane analysis (Origin → Destination) with full route visibility
- Drill-down capability to investigate shipment patterns and operational drivers

### 🔹 Bottlenecks
- Identification of critical inefficiencies driving non-compliance across the logistics network
- Ranking of top non-compliant trade lanes based on total delay impact
- Isolation of routes contributing disproportionately to overall delay accumulation
- Evaluation of least performing carriers based on On-Time Delivery metrics
- Enables prioritization of improvement initiatives by highlighting the highest-impact operational constraints
- Supports targeted intervention by linking performance degradation to specific carriers and trade lanes

### 🔹 Delivery by Mode
- Performance comparison across transportation modes (Air, Road, Rail, Ocean)
- On-Time Delivery % by mode
- Average delay analysis by mode
- Trend analysis to highlight seasonal or operational variation

### 🔹 Delivery by Category
- Performance breakdown by product category
- Identification of categories with higher delay risk
- Comparison of compliance rates across product segments
- Support for identifying category-driven operational issues


---

## 🎨 UI/UX Design
- Modern **dark mode theme**
- Clean and minimal layout
- Consistent color logic:
  - 🟢 > 85% → #34D399 (High Performance)
  - 🟡 80–85% → #F59E0B (Moderate Performance)
  - 🔴 < 80% → #F87171 (Low Performance)

- Interactive slicers for filtering:
  - Destination (Region + Country)
  - Carrier
  - Mode
  - Delivery Date

---

## ⚙️ How to Use

1. Open the `.pbix` file in **Power BI Desktop**
2. Use slicers to filter data by:
   - Region
   - Carrier
   - Time period
3. Navigate between pages using:
   - Buttons
   - Overview dashboard shortcuts
4. Analyze:
   - Top delays
   - Performance drivers
   - Compliance trends

---

## 🛠️ How to Set Up (Local)

### Requirements
- Power BI Desktop
- Excel (or CSV dataset)

### Steps
1. Download the repository
2. Open the `.pbix` file
3. Update data source:
   - Go to **Transform Data → Data Source Settings**
   - Replace file path with your local dataset
4. Refresh the model

---

## 🔐 Data Disclaimer
This project uses **anonymized / synthetic data** for demonstration purposes only.  
No real company data is exposed.

---

## 🚀 Skills Demonstrated
- Data Modeling (Star Schema)
- DAX Calculations
- Data Visualization & Storytelling
- UI/UX Dashboard Design
- Business Problem Framing
- Performance Optimization

---

## 💡 Business Value
This dashboard enables:
- Faster identification of operational inefficiencies
- Improved carrier and route performance tracking
- Data-driven decision making in logistics operations

---

## 📷 Dashboard Preview
<img width="634" height="357" alt="image" src="https://github.com/user-attachments/assets/1229f573-b142-4151-a2c8-d86a0e78d25e" />

---

## 📬 Contact
If you’d like to discuss this project or collaboration opportunities, feel free to connect.
