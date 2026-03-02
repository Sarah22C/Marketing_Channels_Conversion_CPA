# Marketing_Channels_Conversion_CPA
This project analyzes marketing performance using SQL and Tableau to identify where small budget shifts could meaningfully reduce CPA. The focus is on segmentation, leverage, and controlled testing—not dramatic overhauls.

# Marketing Efficiency Optimization (SQL + Tableau Story)

## Overview
This project analyzes digital marketing performance to identify where budget shifts could improve efficiency. The data looks tightly clustered at first glance, so the goal was to go beyond surface-level channel comparisons and find where segmentation (age + funnel stage) reveals the strongest opportunity for measurable CPA improvement.

## Business Question
Where should leadership run a controlled budget reallocation test to reduce Cost Per Acquisition (CPA) without sacrificing conversion volume?

## Primary KPI
- CPA  = Total Spend / Conversions  
Supporting metrics:
- Conversion rate
- Customer counts / conversion volume

## Tools Used
- SQL (SQLite via DBeaver): data cleaning + summary views
- Excel: quick validation/pivot checks early in the process
- Tableau: story-based executive narrative

## Dataset Notes
This dataset is fictional, but the workflow is real-world: clean the data, validate metrics, segment intelligently, and turn findings into a decision-ready recommendation.

## What I Did
1. Cleaned and standardized fields (notably converting AdSpend from text/currency into numeric).
2. Created summary views in SQL to avoid recalculating metrics inconsistently in Tableau.
3. Compared performance at multiple levels:
   - Overall channel performance (tightly clustered)
   - Segment performance by Age Group
   - Efficiency differences by Campaign Type
   - Precision view: 35–44 + Conversion stage + Channel
4. Built a 4-point Tableau Story to present insights and recommendation clearly.

## Key Findings
- Channel performance alone is tightly clustered and doesn’t strongly differentiate efficiency.
- Age segmentation is more decision-relevant than gender for this dataset.
- The 35–44 segment stands out as a high-leverage area.
- Within 35–44, Conversion-stage campaigns have materially lower CPA than Awareness.
- Inside the Conversion stage, Social Media is the lowest CPA channel (with Referral also strong).

## Recommendation (Executive)
Run a controlled reallocation test within the 35–44 segment
- Shift incremental spend from Awareness and upper-funnel Email campaigns
- Toward Conversion-stage Social Media campaigns
- Monitor marginal CPA and conversion volume over 30–60 days to confirm performance stability.

## Deliverables
- Tableau Story
- SQL scripts used to clean + build views
- Exported view outputs (CSV) used in Tableau
