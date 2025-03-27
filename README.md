📞 Call Center Performance Dashboard – Power BI
📌 Project Overview
This Power BI dashboard provides a comprehensive analysis of call center performance, including customer satisfaction, agent performance, and call trends. It helps identify bottlenecks, improve response times, and enhance customer experience.

🎯 Key Insights & Metrics
✔ Customer Satisfaction % – Measures overall satisfaction based on surveys & feedback.
✔ Total Calls Answered & Abandoned – Tracks agent efficiency & service quality.
✔ Average Speed of Answer – Evaluates response times.
✔ Call Trends (Hourly, Daily, Weekly, Monthly) – Identifies peak periods & workload distribution.
✔ Agent Leaderboard – Highlights top 5 performing agents based on key metrics.
✔ Call Topics & Resolution Rates – Analyzes issue types & resolution efficiency.

🛠 Techniques & Tricks Used in Power BI
📊 Data Modeling & Transformations
✅ Power Query Editor – Cleaned, transformed, and structured data for better insights.
✅ Custom Columns – Created calculated fields like Weekday, Hour of Call, and Resolution Status.
✅ Merged Queries – Combined multiple data sources to establish relationships.

📈 Visualization & UX Enhancements
✅ KPI Cards – Used to display key performance indicators (Satisfaction %, Calls Answered, etc.).
✅ Gauge Chart – Visualized customer satisfaction against a set target (e.g., 80%).
✅ Trend Line (Line Chart) – Showed satisfaction trends over time.
✅ Heatmap (Matrix Visual) – Displayed call trends by Day & Hour to detect peak periods.
✅ Scatter Plot (Agent Performance) – Used quadrant analysis to categorize agents into:

Top Performers (High Calls, Low Handle Time)

Efficiency Check Needed (High Calls, High Handle Time)

Potential Improvement (Low Calls, Low Handle Time)

Coaching Opportunity (Low Calls, High Handle Time)

🔍 Filters & Interactive Features
✅ Slicers – Enabled filtering by Date, Agent, Call Type, and Resolution Status.
✅ Drill-through Pages – Created a detailed Agent Performance View (Right-click → Drill-through).
✅ Conditional Formatting – Highlighted high abandoned call rates & poor customer satisfaction.
✅ Tooltips – Added insights when hovering over visual elements.
✅ Bookmark - To hide and display the slicers

🧠 DAX (Data Analysis Expressions) Measures
✅ Total Calls Answered:

DAX
Total Calls Answered = COUNTROWS(FILTER(CallData, CallData[Answered] = "Y"))
✅ Abandoned Call %:

DAX
Abandoned Call % = DIVIDE([Total Calls Abandoned], [Total Calls], 0)
✅ Average Speed of Answer:

DAX
Avg Speed of Answer = AVERAGE(CallData[Speed of Answer])
✅ Top 5 Agents (Leaderboard using Top N Filter):

Used Top N filter on -Resolved Calls (50%) → Higher is better.
                     -Customer Satisfaction % (30%) → Higher is better.
                     -Speed of Answer (20%) → Lower is better (so we reverse rank it).

📈 Key Insights
1️⃣ Customer Satisfaction & Call Volume
Customer Satisfaction = 55.19% (Needs improvement).

Total Calls Answered = 4054 | Calls Abandoned = 946 (18.92%)

Avg Speed of Answer = 54.75 sec (If too high, may lead to customer frustration).

2️⃣ Agent Performance (Top 5 Agents)
  Ranked based on    -Resolved Calls (50%)
                     -Customer Satisfaction % (30%)
                     -Speed of Answer (20%)
Top Agent: Dan (0.83 final score) | Lowest: Greg (0.45).

Performance gaps indicate the need for agent training and best practice sharing.

3️⃣ Resolution Analysis
Only 27% of issues are unresolved (1354 unresolved vs. 3646 resolved).

Common unresolved topics:

Streaming (73% resolved)

Technical Support (72% resolved)

Unresolved issues could be due to lack of expertise or poor ticket follow-ups.

4️⃣ Call Trends (Time & Day Analysis)
Peak hours: 10 AM - 5 PM (High call volume, needs more staff).

Monday sees the most calls (629) → Possible backlog from weekends.

🚀 Recommendations for Improvement
✅ Improve Call Resolution Rate:

Provide specialized agent training for unresolved topics (Streaming & Tech Support).

Introduce callback systems for unresolved queries.

Expand self-service resources to reduce unnecessary calls.

✅ Reduce Call Abandonment Rate:

Optimize IVR (Interactive Voice Response) for better call routing.

Ensure more agents are online during peak hours.

Implement chatbots or knowledge bases for faster resolutions.

✅ Enhance Agent Performance:

Conduct mentorship programs for lower-performing agents.

Introduce performance-based incentives to boost agent efficiency.

✅ Monitor CSAT Trends & Customer Feedback:

Investigate why CSAT % fluctuates and its correlation with unresolved calls.

Conduct customer surveys to improve service quality.

📎 How to Use This Dashboard?
1️⃣ Download the .pbix file and open it in Power BI Desktop.
2️⃣ Use slicers to filter data by Agent, Date, and Topic.
3️⃣ Hover over charts for tooltips with extra insights.
4️⃣ Click on Drill-through pages for in-depth agent performance analysis.

📂 Project Files
📌 call_center_dashboard.pbix – Power BI project file
📌 Call_Center_Dataset.xlsx – PwC Forage program.
📌 README.md – Project documentation

🚀 Next Steps & Improvements
🔹 Deploy to Power BI Service for real-time updates.
🔹 Implement AI-driven insights using Power BI Copilot.
🔹 Automate data refresh for live reporting.
🔹 Integrate with other sources (CRM, customer feedback platforms).

🎯 Conclusion
This Power BI dashboard helps monitor call center performance, optimize operations, and improve customer experience. By leveraging data visualization, DAX, and interactive features, we can make data-driven decisions to enhance efficiency.

📩 Feel free to contribute or reach out for suggestions!

