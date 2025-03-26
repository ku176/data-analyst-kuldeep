Project Title: Animal Inquiry Data Analysis for the City of Vancouver

Project Description

This project focuses on analyzing animal-related inquiry data from the City of Vancouver using AWS services. The goal is to extract, process, clean, and catalog the data to derive meaningful insights for better decision-making.

Objective

The objective of this project is to build an efficient data pipeline that allows for the extraction, profiling, cleaning, cataloging, and analysis of animal inquiry data. The analysis aims to identify trends, anomalies, and key insights regarding public animal-related concerns.

Dataset

The dataset consists of animal-related inquiry records obtained from the City of Vancouver’s website. The data includes information such as inquiry type, location, date, and additional details relevant to public interactions regarding animals.

Methodology

1. Data Collection and Preparation

Data Ingestion: Extracted data from the operational environment and stored it in an Amazon S3 bucket (inq-raw-kul) with a structured path for ease of access.

Data Profiling: Used AWS Glue DataBrew to detect inconsistencies, missing values, and potential errors in the dataset.

Data Cleaning: Renamed invalid column names and stored the transformed files in a separate S3 bucket (inq-trf-kul).

Data Cataloging: Created an AWS Glue database (inq-ani-data-catalog-kul) and used a Glue Crawler to extract metadata and structure the data into a queryable format.

2. Descriptive Statistics

Analyzed key attributes such as the number of inquiries per year, most frequent inquiry types, and distribution of cases across different locations.

Generated summary statistics to understand data trends and patterns.

3. Data Visualization

Created visual representations using AWS QuickSight and other visualization tools.

Used bar charts, heatmaps, and trend graphs to illustrate inquiry trends over time and across regions.

4. Survival Analysis

Analyzed trends in animal inquiries over different time periods.

Examined the persistence and recurrence of certain types of inquiries.

5. Insights and Findings

Identified the most common types of animal-related inquiries.

Observed seasonal trends and geographic concentration of inquiries.

Provided insights on public concerns and response efficiency.

6. Conclusion

Established a structured pipeline for processing and analyzing inquiry data.

Delivered actionable insights for city authorities to improve response strategies and resource allocation.

Tools and Technologies

AWS S3 for data storage

AWS Glue DataBrew for data profiling and cleaning

AWS Glue Crawler for data cataloging

AWS QuickSight for data visualization

Python/Pandas for statistical analysis

Deliverables

Data Pipeline Documentation: Detailed steps for ingestion, profiling, cleaning, and cataloging.

Descriptive Statistical Report: Key metrics and summary statistics.

Visual Reports: Charts and graphs illustrating trends in animal inquiries.

Final Analysis Report: A comprehensive document outlining insights, findings, and recommendations.

This project demonstrates how AWS services can be leveraged to process and analyze large datasets efficiently, ensuring structured data management and valuable insights.


