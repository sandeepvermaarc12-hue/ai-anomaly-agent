# AI Anomaly Agent

An automated business data monitoring tool built in Python — instead of analyzing data once like a typical EDA notebook, this project actively watches business metrics, detects unusual movement, explains it in plain English, visualizes it, and sends an alert.

## What It Does

1. **Reads** a business dataset (Revenue, Orders, Traffic, Conversion Rate, Cost, Refunds)
2. **Detects** anomalies using a 2-standard-deviation statistical rule, calculated individually per metric
3. **Explains** every detected anomaly in plain business language (not raw numbers)
4. **Visualizes** all six metrics with anomalies highlighted on a 6-panel chart
5. **Alerts** — generates a simulated email-style alert when anomalies are found
6. **Logs** every alert as a timestamped record for permanent history

## Why This Project

Most beginner portfolios include a standard EDA notebook — useful, but common. This project instead behaves like a real business tool: a manager doesn't need to check a dashboard every morning, because the system tells them the moment something needs attention.

## Results

Tested against a 90-day dataset with 4 deliberately planted anomalies (a revenue spike, a refund surge, a traffic crash, a cost blowout) — **all 4 were detected correctly**, along with a few statistically expected edge cases that are explained in the full report rather than treated as noise.

## Tech Stack

- Python (Pandas, NumPy, Matplotlib)
- Google Colab
- Statistical anomaly detection (2-std-dev threshold method)

## Files in This Repo

| File | Description |
|---|---|
| `AI_Anomaly_Agent.ipynb` | Full Colab notebook — all code, cell by cell |
| `business_data.xlsx` | Synthetic 90-day business dataset used for the project |
| `anomaly_charts.png` | 6-panel visualization of all metrics with anomalies highlighted |
| `alert_sample.txt` | Sample simulated email alert log |
| `AI_Anomaly_Agent_Final_Report.docx` | Full project report — every cell explained (Purpose, Code, Explanation, Output, Interpretation) |

## Author

Sandeep Verma — MBA (Business Analytics), IMS, University of Lucknow# ai-anomaly-agent
Automated business data monitoring tool with anomaly detection, plain-English summaries, visualization, and alert system
