\# PRDA-02: Customer Satisfaction (CSAT) Analytics



A two-page Power BI dashboard analysing 32,941 customer-support contacts from October 2020. This project explores contact volume, CSAT scores, contact reasons, channels, states and response-time categories.



Developed as part of the Certified Data Analyst (CDA) capstone project.



\## Dashboard Preview



\### Page 1: Executive Overview



!\[Executive Overview](Screenshots/CSAT\_Executive\_Overview.png)



\### Page 2: CSAT Analysis



!\[CSAT Analysis](Screenshots/CSAT\_Analysis.png)



\## Project Objective



Analyse customer support performance and satisfaction across contact reasons, channels, states and response-time categories, while documenting what the available data can and cannot establish.



\## Key Findings



| Metric | Value |

|---|---:|

| Total contacts | 32,941 |

| Records with CSAT = 0 | 20,670 (62.7%) |

| Average CSAT, all records | 2.07 |

| Average CSAT, non-zero scores | 5.55 |

| Non-zero score rate | 37.3% |

| Scores ≥ 7 (% of all records) | 12.9% |

| Average contact duration | 25.0 minutes |

| Share labelled Within SLA | 62.6% |

| Bill Question share of contacts | 71.2% |



\## Business Insights



1\. \*\*Zero scores:\*\* 62.7% of records have a CSAT score of zero. The meaning of zero is not documented or verified.

2\. \*\*Contact reasons:\*\* Bill Question accounts for approximately 71.2% of all contacts.

3\. \*\*Non-zero CSAT:\*\* Average scores are 5.62 Above SLA, 5.56 Below SLA and 5.53 Within SLA.

4\. \*\*Daily volume:\*\* Approximately 1,045–1,170 contacts per day during the displayed October period.

5\. \*\*Contact duration:\*\* Average contact duration is approximately 25 minutes.



The full written insights are available in `insights/insights.pdf`.



\## Dashboard Pages



\- \*\*Executive Overview:\*\* KPI cards, daily contact trend, channel mix, contact reasons, state distribution, CSAT by response time and CSAT score distribution.

\- \*\*CSAT Analysis:\*\* Average CSAT by contact reason, channel and state; contact volume by response time; channel slicer; key insights and data notes.



\## Dataset

The original dataset contains 32,941 customer-support records covering October 2020, with 13 fields related to customer interactions, satisfaction scores, contact reasons, channels and response times.

The raw dataset is not included in this public repository to protect customer privacy. time, contact duration and call centre.



\## Methodology and Definitions



\- \*\*Average CSAT (Non-Zero):\*\* Average of `csat\_score` where the score is greater than zero.

\- \*\*Non-Zero Score Rate:\*\* Records with a non-zero CSAT score divided by all records. This is not a confirmed survey response rate.

\- \*\*Scores ≥ 7:\*\* Records with a CSAT score of 7 or higher divided by all records.

\- \*\*Within SLA Share:\*\* Records labelled Within SLA divided by all records. Original source labels are retained.

\- \*\*State Comparisons:\*\* CSAT comparisons exclude states with fewer than 100 contacts. Overall state contact distribution includes all states.

\- \*\*Daily Trend:\*\* 31 October, which contains only one record, is excluded from the daily trend visual.



\## Limitations



\- The meaning of a zero CSAT score is not documented or verified.

\- Exact SLA thresholds and category definitions were not provided.

\- State-level CSAT averages use non-zero scores, so the scored samples are smaller than total contact counts.

\- Differences in average CSAT across categories are small.

\- Findings are descriptive and do not establish causation.

\- The dataset covers October 2020 only.



\## Repository Structure

```text
PRDA-02-CSAT-Analytics/
├── README.md
├── insights/
│   └── insights.pdf
├── Powerbi/
│   └── PRDA-02_CSAT_Dashboard.pbix
├── Presentation/
│   └── PRDA-02_CSAT_Capstone_Presentation.pptx
└── Screenshots/
    ├── CSAT_Analysis.png
    └── CSAT_Executive_Overview.png

```



\## How to Open the Dashboard


1. Download `Powerbi/PRDA-02_CSAT_Dashboard.pbix`.
2. Open it using Microsoft Power BI Desktop.
3. If the original data source is unavailable, provide an authorized anonymized copy of the dataset.
4. Update the data source path through Home → Transform data → Data source settings.

\## Tools and Skills Demonstrated


\- SQL – Dataset extraction and export

\- Microsoft Power BI – Dashboard development and visualization

\- DAX – Measures and KPI calculations

\- Data validation and interpretation

\- Dashboard design

\- Business insights and presentation



\---



\*\*Project:\*\* PRDA-02 CSAT Analytics  

\*\*Category:\*\* Data Analytics  

\*\*Course:\*\* Certified Data Analyst (CDA)

