# Gathering Data

## Identifying Data for Analysis

- **Understanding the Problem and Desired Outcome**
    - Identify current state and target state.
    - Define measurable metrics.
- **Determining the Information to Collect**
    - Decide on specific data needed.
    - Identify potential data sources.
    - Align data with goals.
- **Example Use Case: Targeted Marketing Campaigns**
    - Collect customer profile, purchase history, location, age, education, profession, income, marital status.
    - Collect customer complaint data and service survey ratings.
    - Collect social media interaction data.
- **Defining a Data Collection Plan**
    - Establish timeframe for data collection (ongoing vs. specific period).
    - Determine sufficient data volume for credible analysis.
    - Define dependencies, risks, and mitigation plans.
- **Data Collection Methods**
    - Identify methods based on data type, timeframe, and volume.
    - Sources: internal systems, social media, third-party providers.
- **Implementing Data Collection Strategy**
    - Execute the plan and collect data.
    - Update the plan as needed based on evolving conditions.
- **Quality, Security, and Privacy Considerations**
    - Ensure data is error-free, accurate, complete, relevant, and accessible.
    - Define quality metrics and checkpoints.
    - Address data governance: usability, integrity, availability.
    - Ensure compliance with security regulations and privacy mandates.
- **Data Governance and Privacy**
    - Plan for confidentiality, usage licenses, and regulatory compliance.
    - Maintain an auditable trail for validations and checks.
    - Avoid penalties and maintain credibility by ensuring trustworthy data.
- **Importance of Identifying the Right Data**
    - Ensures multiple perspectives on the problem.
    - Provides credible and reliable findings.

## Data Sources

1. **Types of Data Sources**
    - **Internal or External**
    - **Primary, Secondary, or Third Party**
2. **Primary Data**
    - Directly obtained by the user from the source.
    - Internal sources: organizational data, CRM, HR, workflow applications.
    - Methods: surveys, interviews, discussions, observations, focus groups.
3. **Secondary Data**
    - Retrieved from existing sources.
    - External databases, research articles, publications, training material, Internet searches, financial records.
    - Data from externally conducted surveys, interviews, discussions, observations, focus groups.
4. **Third Party Data**
    - Purchased from data aggregators.
    - Comprehensive datasets from various sources for commercial sale.
5. **Examples of Data Sources**
    - **Databases**: Primary, secondary, third party.
        - Internal applications for managing processes, workflows, customers.
        - External databases (subscription or purchase).
    - **Cloud**: Source for real-time information and on-demand insights.
    - **Web**: Publicly available data (free or commercial use).
        - Textbooks, government records, papers, articles.
        - Social media: Facebook, Twitter, Google, YouTube, Instagram.
        - Used for quantitative and qualitative insights on customers.
    - **Sensor Data**: Wearable devices, smart buildings, smart cities, smartphones, medical devices, household appliances.
    - **Data Exchange**: Third party data through voluntary sharing.
        - Data providers and consumers include individuals, organizations, governments.
        - Data from business applications, sensor devices, social media, location data, consumer behavior.
6. **Methods of Data Collection**
    - **Surveys**: Questionnaires distributed to selected groups.
        - Example: gauging customer interest in an updated product.
        - Can be web or paper-based.
    - **Census Data**: Household data (wealth, income, population).
    - **Interviews**: Gathering qualitative data (opinions, experiences).
        - Example: understanding challenges faced by a customer service executive.
        - Methods: telephonic, web, face-to-face.
    - **Observation Studies**: Monitoring participants in specific environments or tasks.
        - Example: observing users on an e-commerce site to assess usability.
7. **Types of Data in Methods**
    - Primary, secondary, third party data from surveys, interviews, observation studies.
8. **Evolution of Data Sources**
    - Dynamic and diverse, continuously evolving.
    - Combining primary, secondary, and third party data for comprehensive analysis.

## How to Gather and Import Data

1. **Gathering Data from Different Sources**
    - Databases, the web, sensor data, data exchanges, etc.
    - Importing data into various data repositories.
2. **SQL (Structured Query Language)**
    - Querying language for relational databases.
    - Commands for retrieval, grouping, sequencing, and limiting query results.
    - Non-relational databases can use SQL or SQL-like tools (e.g., CQL for Cassandra, GraphQL for Neo4J).
3. **APIs (Application Programming Interfaces)**
    - Extract data from databases, web services, data marketplaces.
    - Validate data (e.g., postal addresses, zip codes).
4. **Web Scraping**
    - Download specific data from web pages (text, contact info, images, videos, podcasts, product items).
5. **RSS Feeds**
    - Capture updated data from online forums and news sites.
6. **Data Streams**
    - Aggregate constant data streams (instruments, IoT devices, applications, GPS data, social media).
7. **Data Exchange Platforms**
    - Facilitate data exchange with defined standards, protocols, and formats.
    - Ensure security, governance, data licensing, de-identification, legal frameworks, quarantined analytics.
    - Examples: AWS Data Exchange, Crunchbase, Lotame, Snowflake.
8. **Specific Data Needs**
    - Marketing trends and ad spending: Forrester, Business Insider.
    - Strategic and operational guidance: Gartner, Forrester.
    - User behavior data, mobile/web usage, market surveys, demographic studies.
9. **Importing Data into Repositories**
    - Combine data from different sources for a unified interface.
    - Tools and methods vary by data type, volume, and destination repository.
10. **Data Repositories and Data Types**
    - **Relational Databases**: Store structured data (OLTP systems, spreadsheets, online forms, sensors, logs).
    - **NoSQL Databases**: Store structured and semi-structured data.
    - **Semi-Structured Data**: Emails, XML, zipped files, binaries, TCP/IP protocols (stored in NoSQL clusters).
    - **Unstructured Data**: Web pages, social media feeds, images, videos, documents, media logs, surveys (stored in NoSQL databases, Data Lakes).
    - **Data Lakes**: Accommodate all data types and schemas.
11. **ETL Tools and Data Pipelines**
    - Automate the process of importing data.
    - Tools: Talend, Informatica.
    - Programming languages and libraries: Python, R.

# Wrangling Data

## What is Data Wrangling?

- **Data Wrangling Overview**
    - Iterative process involving data exploration, transformation, validation, and preparation for analysis.
    - Prepares raw data from various sources in a data repository.
- **Four Phases of Data Wrangling**
    - **Discovery (Exploration) Phase**
        - Understand data for specific use cases.
        - Clean, structure, organize, and map data.
    - **Transformation Phase**
        - Structuring: Change form and schema of data.
            - Merge data from different formats (e.g., relational databases, Web APIs).
            - Use joins and unions to combine data (columns vs. rows).
        - Normalization: Clean database, reduce redundancy (transactional data).
        - Denormalization: Combine data for faster querying (reporting).
        - Cleaning: Fix irregularities (inaccurate, missing, biased, outliers).
            - Example: sourcing missing demographic data for accurate analysis.
    - **Enrichment Phase**
        - Enhance analysis by adding relevant data points.
        - Supplement datasets with external or public data.
        - Insert metadata to improve context (sentiment scores, weather data, publication details).
    - **Validation Phase**
        - Check data quality post-transformation, cleaning, and enrichment.
        - Ensure consistency, quality, and security with validation rules.
    - **Publishing Phase**
        - Deliver transformed, validated data for downstream project needs.
        - Include metadata about the dataset.
- **Documentation Importance**
    - Document all steps and considerations.
    - Ensure replicability and revisiting of decisions during data wrangling.
- **Iterative Nature**
    - Each phase is iterative to refine data for credible and meaningful analysis.

## Tools for Data Wrangling

- **Excel Power Query / Spreadsheets**
    - Includes Microsoft Excel and Google Sheets.
    - Offers built-in formulas and features for data identification, cleaning, and transformation.
    - Add-ins allow importing data from various sources and processing as needed.
- **OpenRefine**
    - Open-source tool supporting TSV, CSV, XLS, XML, JSON formats.
    - Menu-driven operations, no need for command memorization.
    - Enables data cleaning, format transformation, and integration with external data.
- **Google DataPrep**
    - Cloud-based service for structured and unstructured data preparation.
    - Managed service with automated schema detection and anomaly detection.
    - Provides step-by-step suggestions for data cleaning and transformation.
- **Watson Studio Refinery**
    - Available via IBM Watson Studio for data discovery and transformation.
    - Transforms raw data into quality information for analytics.
    - Automatically detects data types and applies data governance policies.
- **Trifacta Wrangler**
    - Cloud-based service for interactive data cleaning and transformation.
    - Cleans real-world data for export to Excel, Tableau, and R.
    - Supports collaborative features for team-based data preparation.
- **Python**
    - Utilizes libraries like Numpy and Pandas for powerful data manipulation.
    - **Numpy**
        - The most basic package that Python offers
        - It is fast, versatile, interoperable, and easy to use
        - It provides support for large multi-dimensional arrays and matrices, and high-level mathematical functions to operate on these arrays.
    - **Pandas**
        - Designed for fast and easy data analysis operations
        - Allows complex operations such as merging, joining, and transforming huge chunks of data using simple, single-line commands
        - Helps prevent common errors that result from misaligned data coming in from different sources
    - Jupyter Notebook for interactive data cleaning, transformation, and visualization.
- **R**
    - Libraries such as Dplyr, Data.table, and Jsonlite for data wrangling.
    - **Dplyr**
        - A powerful library for data wrangling with a precise and straightforward syntax.
    - **Data.table**
        - Helps aggregate large data sets quickly
    - **Jsonlite**
        - A robust JSON parsing tool, great for interacting with web APIs.
    - Supports investigation, manipulation, and analysis of data, especially from web APIs.
- **Decision Criteria**
    - Choose tools based on data size, structure, cleaning, and transformation needs.
    - Consider infrastructure requirements, ease of use, and learning curve.

## Data Cleaning

- **Data Quality Impact**
    - Poor data quality undermines business objectives and competitive advantage.
    - Issues like missing, inconsistent, or incorrect data lead to flawed conclusions and costly decisions.
- **Data Issues in Datasets**
    - Data sourced from disparate sources may have missing values, inaccuracies, duplicates, inconsistent records, and formatting errors.
    - Data wrangling tools and scripts help automate correction or removal of irreparable data.
- **Data Cleaning vs. Data Wrangling**
    - Data cleaning is a subset of data wrangling focused on transforming and verifying data integrity.
    - Typical workflow includes inspection, cleaning, and verification phases.
- **Inspection and Data Profiling**
    - Identify data issues using rules, constraints, data profiling, and visualization.
    - Detect anomalies such as null values, duplicates, and outliers using statistical methods.
- **Common Data Cleaning Techniques**
    - Address missing values through filtering, sourcing, or imputation based on statistical methods.
    - Remove duplicate data points and irrelevant data not pertinent to the analysis.
- **Data Standardization and Type Conversion**
    - Standardize data formats (e.g., dates, units) and convert data types to ensure consistency.
    - Clean syntax errors like extra spaces or inconsistent formats (e.g., state names).
- **Handling Outliers**
    - Identify outliers that skew analysis results and decide whether to include or correct them based on the use case.
- **Verification and Documentation**
    - Verify data quality post-cleaning to ensure accuracy and effectiveness.
    - Document all changes made during the data cleaning process, reasons for changes, and current data quality status.

## Viewpoints: Data Preparation and Reliability

- **Data Gathering and Preparation:**
    - Data professionals emphasize the significant role of gathering, cleaning, and preparing data for analysis.
    - This process is essential despite support from proficient data engineering teams, ensuring understanding and addressing potential data issues.
- **Importance in Financial Analysis:**
    - For CPAs, approximately 30% of the job involves laying out financial data accurately from general ledger systems.
    - Ensuring completeness and accuracy of financial statements is crucial before diving into analytical tasks.
- **Steps for Ensuring Data Reliability:**
    - Running summary statistics on individual data columns to verify consistency with real-world expectations.
    - Ensuring financial data reliability through accuracy, lack of bias, and error-free attributes.
- **Logic Checks for Data Integrity:**
    - Conducting logic checks before detailed analysis to validate data coherence.
    - Addressing basic data integrity questions such as correct sources and query periods before deeper analysis.
- **Conclusion and Analysis:**
    - Once data reliability is confirmed, professionals proceed with detailed analysis to draw conclusions about financial performance or other analytical goals.