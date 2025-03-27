Descriptive Analysis

Step 05 - Data Summarization

Why I Did It

I performed data summarization to extract meaningful insights from the dataset stored in the catalog. This process was essential for generating descriptive analysis questions based on summarized data.

How I Did It

I ran an ETL job in AWS Glue, applying schema changes to remove unnecessary columns and using filters to eliminate redundant rows. Additionally, I implemented grouping and aggregation operations to effectively summarize the dataset. The summarized data was stored in a new S3 bucket named inq-cur-kul, organized into System and Users folders separately. The summarized tables were also registered in the AWS Glue Data Catalog, which is referenced in the Data Cataloging step.

Screenshots of Data Summarization

(Screenshots to be attached here)

Final Summarized Table

Channel

avg(numberofrecords)

Report Date

Social Media

1.64

2025-03-02 16:24:00

Chat

11.77

2025-03-02 16:24:00

E-mail

4.85

2025-03-02 16:24:00

Phone

42.21

2025-03-02 16:24:00

Mail

17.50

2025-03-02 16:24:00

Descriptive Analysis Questions Generated

Which communication channel has the highest average number of records for animal general inquiries?

Which channel has the lowest average number of records, and what does this suggest about its usage?

How does the average number of records compare between digital channels (Social Media, Chat, E-mail) and traditional channels (Phone, Mail)?

Business Questions in AWS Athena

Business Question 1

(Specific query and findings to be inserted here)

Business Question 2

(Specific query and findings to be inserted here)

Business Question 3

(Specific query and findings to be inserted here)

Explanation

To extract business insights, I executed SQL queries in AWS Athena against structured data stored in Amazon S3. Using AWS Glue, I registered schemas and normalized SQL queries for meaningful insights, such as computing the biid_avg, min biid_avg, and biid_avg by channel. The queries were executed in the Athena console, and the results were verified and stored for future reference. This approach enabled scalable and cost-effective data-driven decision-making.

Project Description

Project Title

(Insert project title here)

Objective

(Define project objectives here)

Dataset

(Provide details about the dataset used)

Methodology

Data Collection and Preparation:

(Describe data sources and preparation steps)

Descriptive Statistics:

(Summarize key statistical insights)

Data Visualization:

(Mention visual tools or methods used)

Survival Analysis:

(Explain any survival analysis techniques applied)

Insights and Findings:

(Highlight key takeaways from the analysis)

Conclusion:

(Summarize the final outcomes and their implications)

Tools and Technologies

AWS Glue

AWS Athena

Amazon S3

SQL

Data Cataloging

Deliverables

Summarized dataset stored in Amazon S3

AWS Glue Data Catalog with structured tables

SQL queries and results from AWS Athena

Descriptive and business analysis questions

Insights derived from the summarized data

