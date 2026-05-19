🏥 Hospital Emergency Room Dashboard — Power BI
> An interactive 4-page Power BI dashboard analyzing Emergency Room operations across **19 months (April 2023 – October 2024)** covering **9,216 unique patients**.
---
📸 Dashboard Preview
Page 1 — Monthly View
<img width="1217" height="787" alt="image" src="https://github.com/user-attachments/assets/16b1ac2f-3b35-4c2d-bc4f-30775d963fee" />

Page 2 — Consolidated View
<img width="1222" height="795" alt="image" src="https://github.com/user-attachments/assets/604d8b3e-06dd-4ee2-975a-28720fe2db98" />

Page 3 — Patient Details
<img width="1215" height="795" alt="image" src="https://github.com/user-attachments/assets/cba361f0-3e7d-4291-98d3-5e513fe9e0d0" />

Page 4 — Key Takeaways
<img width="1217" height="797" alt="image" src="https://github.com/user-attachments/assets/9ae90599-cd6a-4a60-9957-4ef358ffcaa6" />

---
📊 Project Overview
This dashboard was built in Power BI Desktop to provide real-time, data-driven insights into hospital emergency room operations. It enables hospital administrators and medical staff to monitor patient flow, track satisfaction, analyze peak hours, and make informed staffing decisions.
---
🔢 Key Metrics (Consolidated: Apr 2023 – Oct 2024)
Metric	Value
📋 Total Patients	9,216
⏱️ Avg Wait Time	35.3 Minutes
⭐ Patient Satisfaction Score	4.99 / 10
🔁 Patients Referred	3,816
✅ Admitted	4,612 (50.04%)
❌ Not Admitted	4,604 (49.96%)
🎯 Seen Within 30 Min (Target Met)	59.32%
---
📌 Dashboard Pages

📅 Page 1 — Monthly View
Snapshot of a single month with dynamic filters for Year and Month.
KPI cards: Patients, Wait Time, Satisfaction, Referrals
Patient Admission Status table
Patients by Age Group (bar chart)
% Patients Seen Within 30 Minutes (donut chart)
Patients by Gender (donut chart)
Department Referral breakdown (bar chart)
Patient Race distribution (bar chart)
Day & Hour Heatmap for peak ER traffic

📈 Page 2 — Consolidated View
Aggregated trends across the full 19-month dataset (Apr 2023 – Oct 2024).
Same KPI cards with full-period totals
Date range slider for flexible filtering
Trends across all charts with higher patient volumes
Heatmap showing busiest times (Sat 03-04: 128 patients peak)

🧾 Page 3 — Patient Details
Granular row-level data for all patients.
Searchable/scrollable table with columns:
Patient ID, Name, Gender, Age
Admission Date, Race, Wait Time
Department Referral, Admission Status
Date range filter (Apr 2023 – Oct 2024)

💡 Page 4 — Key Takeaways
Descriptive analysis summarizing the full dataset findings.
Category	Finding
⏳ Wait Time	Avg 35.3 min — needs improvement for better patient flow
😊 Satisfaction	4.99/10 — moderate; improvement areas identified
🏥 Top Referrals	General Practice (1,840), Orthopedics (995), Physiotherapy (276)
📅 Busiest Days	Saturday (1,377), Thursday (1,332), Tuesday (1,318)
🕐 Busiest Hours	11 AM, 7 PM, 1 PM, 11 PM
👥 Top Age Group	30–39 Years (1,200 patients)
🌍 Top Race Group	White (2,571), African American (1,951), Multiracial (1,557)
🔄 Admission Split	Nearly equal — 4,612 admitted vs 4,604 not admitted

---
🛠️ Tools & Technologies
Tool	Purpose
Power BI Desktop	Data modeling, visualization, dashboard design
DAX	Custom KPI measures, time intelligence, % calculations
Power Query	Data cleaning and transformation
Data Modeling	Star schema — Date Table + Hospital ER_Data
---
📁 Data Model
```
Date Table                    Hospital ER_Data
├── Date                      ├── Patient ID & Name
├── Day Name                  ├── Patient Gender / Age / Race
├── Month & Year              ├── Admission Date & Hour
├── Month Name                ├── Admission Status
├── Month Number              ├── Avg Wait Time
├── Week Day                  ├── Department Referral
└── Year                      ├── No. of Patients
                              └── Patient Satisfaction Score
```
---
🚀 How to Use
Clone this repository:
```bash
   git clone https://github.com/rjharshpatel/hospital-er-dashboard.git
   ```
Open the file:
Open `Hospital.pbix` in Power BI Desktop (free).
Explore the dashboard:
Use the Year / Month slicers on Monthly View
Use the date range slider on Consolidated & Patient Details pages
Navigate using side buttons or bottom page tabs
---
💡 Key Insights & Recommendations
Staffing: Increase staff on Saturdays and during 11 AM, 7 PM, 11 PM shifts
Wait Times: 35.3 min average suggests need for triage process improvements
Referrals: ~5,400 patients needed no referral — possible cases for urgent care redirection
Demographics: Adults 30–39 are the most frequent ER visitors — targeted outreach opportunity
Satisfaction: Score of 4.99/10 highlights experience gaps worth investigating
---

---
🙋 Author
Harsh Raj
💼 Linkedin www.linkedin.com/in/harshpatel2510

---
📜 License
This project is for educational and portfolio purposes. The dataset used is sample/synthetic hospital ER data.
