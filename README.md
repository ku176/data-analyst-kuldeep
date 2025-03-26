Data Wrangling

Methodology

Step 1: Data Ingestion

Why I did it:
I performed this step to extract data from the operational environment of the City of Vancouver and move it to the data analytics platform for further processing.

How I did it:
I created an S3 bucket named inq-raw-kul and structured a path (inq-raw-kul/inquiry/animal-general-inquiry-list/year) to store the extracted data from the City of Vancouver’s website.

Screenshot of Data Ingestion

Step 2: Data Profiling

Why I did it:
This step was necessary to identify data issues in the extracted dataset from the ingestion process.

How I did it:
I used AWS DataBrew and created a project named bus-Inq-ani-list-prj-kul, linked to the dataset bus-Inq-ani-list-ds-kul, to check for anomalies. No data issues were found.

Screenshot of Data Profiling

Step 3: Data Cleaning

Why I did it:
Since no data issues were found in the profiling step, I only renamed invalid column names to valid ones for consistency. The cleaned files were stored in a new S3 bucket, inq-trf-kul, in both user-friendly and system-friendly folders.

How I did it:
I applied a renaming function to standardize column names.

Screenshot of Data Cleaning
Screenshot of Storing Cleaning Files in S3 Bucket

Step 4: Data Cataloging

Why I did it:
The objective was to convert CSV files from the transformation bucket into a structured data catalog for easier analysis.

How I did it:
Using AWS Glue Crawler, I created a database named inq-ani-data-catalog-kul, where I stored a table called inq-animal-trf-system for further queries.

Screenshot of Data Cataloging

Step 5: Data Summarization

Why I did it:
Summarizing the dataset helped extract meaningful insights and formulate descriptive analysis questions.

How I did it:
I executed an ETL job in AWS Glue, utilizing schema changes to remove unnecessary columns, filters to exclude redundant rows, and aggregation techniques to summarize the data. The summarized files were stored in the S3 bucket inq-cur-kul in designated system and user folders.

Screenshot of Data Summarization

Project Description: Data Wrangling for Customer Analytics at XYZ Company

Project Title:

Data Wrangling for Enhanced Customer Analytics at XYZ Company

Objective:

The goal of this project is to conduct comprehensive data wrangling to create a refined dataset for customer analytics at XYZ Company. This involves cleaning, transforming, and merging data from multiple sources to improve its accuracy and usability for analysis and reporting.

Background:

XYZ Company collects customer data from various channels, including sales transactions, customer service interactions, and marketing campaigns. However, data inconsistencies, missing values, and fragmentation present challenges in deriving insights. Proper data wrangling is essential for improving decision-making and optimizing marketing strategies.

Dataset:

This project utilizes multiple datasets, including:

Sales Data: Customer transactions, purchase amounts, product details, timestamps.

Customer Information: Demographics (age, gender, location, account creation date).

Customer Service Records: Logs of inquiries, complaints, and resolutions.

Marketing Data: Email and campaign response data (open rates, click-through rates).

Methodology

1. Data Collection

Gather data from internal databases, CRM systems, and third-party platforms.

Identify relevant datasets for a comprehensive customer profile.

2. Data Assessment

Assess data quality to identify missing values, duplicates, and inconsistencies.

Document data types, formats, and discrepancies.

3. Data Cleaning

Address missing values through imputation or exclusion.

Remove duplicates and standardize formats (e.g., dates, naming conventions).

Normalize categorical variables (e.g., standardizing "active/inactive" statuses).

4. Data Transformation

Convert data types for compatibility (e.g., strings to datetime objects).

Create new features (e.g., total purchases, purchase frequency, customer tenure).

Aggregate data for structured analysis (e.g., summarizing monthly sales per customer).

5. Data Consolidation

Merge datasets using unique identifiers (e.g., Customer ID).

Create a unified customer view by integrating sales, support, and marketing data.

6. Documentation and Validation

Document data sources, cleaning methods, and transformation techniques.

Perform Exploratory Data Analysis (EDA) to validate accuracy and completeness.

Tools and Technologies

Python (Pandas, NumPy) or R for data manipulation.

SQL for data extraction and assessment.

Jupyter Notebook or RStudio for interactive wrangling.

Matplotlib, Seaborn for visualization and quality checks.

Deliverables

A cleaned and transformed dataset ready for analysis in CSV or database format.

A detailed report documenting the data wrangling process, challenges, and results.

Visualizations illustrating key data insights and validation checks.

