1.	Objective 
The objective of this project is to analyze accident data to identify key patterns, risk factors, and trends that contribute to road accidents. By utilizing data analytics and visualization techniques, the project aims to uncover insights related to accident frequency, severity, location, and contributing factors such as weather conditions, time of day, and road infrastructure. These findings will help inform data-driven decision-making for policymakers, traffic management authorities, and public safety organizations to implement effective measures that enhance road safety, reduce accident occurrences, and improve emergency response strategies.
2.	Scope
This project aims to analyze accident data to identify patterns and contributing factors affecting road safety. By examining variables such as time, location, weather conditions, and driver behavior, the study seeks to provide insights that enhance traffic management and public safety policies. The findings will support data-driven decision-making to reduce accident rates, improve infrastructure planning, and optimize emergency response strategies.
3.	Architecture
This structured architecture allows for the efficient handling of the data. It outlines the efficient collection, processing, analysis, and visualization of US accident data, providing valuable insights for stakeholders and decision-makers.
 
a)	Data Source & Extraction – Kaggle
•	The primary data source for the project is Kaggle, which hosts datasets related to US accidents.
•	The project utilizes Kaggle's data available for extraction to gather necessary information for analysis.
b)	Data Staging Layer – AWS S3:
•	Raw data is initially stored in an Amazon S3 bucket, serving as the staging layer.
•	This step allows for secure and scalable storage of the unprocessed data before further processing.
c)	Data Orchestration – AWS Glue:
•	AWS Glue is used for Extract, Transform, Load (ETL) processes.
•	It facilitates data transformation and integrates various data sources, streamlining the preparation of data for analysis.
d)	Processed Zone – S3 Bucket:
•	After ETL processes, the processed data is stored in a designated S3 bucket for further access.
•	This layer ensures that clean and structured data is readily available for querying.
e)	Data Storage – Amazon Redshift:
•	Amazon Redshift serves as the data warehouse solution, enabling efficient querying and data management.
•	The processed data is housed here, structured for optimized performance during analysis.
f)	Data Visualization – Power BI:
•	Power BI is leveraged for data visualization, allowing the creation of interactive dashboards and reports.
•	This tool enables stakeholders to visualize insights and findings effectively, facilitating better decision-making.
