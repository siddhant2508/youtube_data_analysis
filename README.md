# 📊 YouTube Data Analysis using AWS & QuickSight

This project showcases an end-to-end pipeline for YouTube data analysis using AWS services with visualizations built in **Amazon QuickSight**.

---

## 🚀 Architecture Overview

- **Ingestion**: Source data pushed to Amazon S3
- **Transformation**: AWS Glue ETL scripts
- **Storage**: S3 (Raw → Cleansed → Reporting zones)
- **Query**: Amazon Athena
- **Visualization**: Amazon QuickSight
---

## 📈 Dashboard Overview

View the live dashboard on QuickSight:  
🔗 [YouTube Analytics Dashboard (QuickSight)]

(https://us-east-2.quicksight.aws.amazon.com/sn/accounts/654407503038/dashboards/611a6498-1d2e-4b72-8c99-4349d5d9aebd?directory_alias=Siddhant)

---

### Key Insights from Dashboard:
- **📌 Total Likes**: ~5.9 Billion
- **📌 Total Views**: ~225 Billion
- **📌 Total Comments**: ~622 Million
- **Top Snippet Categories by Likes**: People & Blogs, Music, Entertainment
- **Top Snippet Categories by Views**: Music dominates, followed by Entertainment and People & Blogs
- **Regional Insights**: US, GB, and CA contribute majorly to the views
- **Top Channels**: Channels like **xXxTentacion**, **Vevo**, and **T-Series** lead in viewership
- **Views vs Likes**: Strong positive correlation with some outliers

![QuickSight Dashboard]- https://us-east-2.quicksight.aws.amazon.com/sn/accounts/654407503038/dashboards/611a6498-1d2e-4b72-8c99-4349d5d9aebd?directory_alias=Siddhant

---

## 🧰 Technologies Used

- AWS S3
- AWS Glue
- Glue Data Catalog
- AWS Lambda
- Amazon Athena
- Amazon QuickSight
- AWS IAM, Step Functions, CloudWatch

---

## 📁 How to Reproduce

1. Upload sample json /CSV to S3
2. Run Glue job (`scripts/glue_job.py`)
3. Define tables using `scripts/athena_queries.sql`
4. Visualize via QuickSight connected to Athena

---

**Last updated:** June 5, 2025
