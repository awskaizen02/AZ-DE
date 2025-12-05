| Term                     | Simple Meaning                            | Why It Is Used                        | Real-Life Example                                  |
| ------------------------ | ----------------------------------------- | ------------------------------------- | -------------------------------------------------- |
| **ETL**                  | Extract → Transform → Load                | Clean & structure data before storing | Cleaning sales data then loading into warehouse    |
| **ELT**                  | Extract → Load → Transform                | Faster; uses warehouse compute power  | Load raw data to BigQuery/Snowflake then transform |
| **Data Warehouse**       | Organized data storage for analytics      | Fast reporting, BI dashboards         | Amazon Redshift, Snowflake                         |
| **Data Lake**            | Stores raw, unstructured data             | Cheap storage for huge datasets       | Store logs, images, raw files in S3                |
| **Data Lakehouse**       | Warehouse + Lake together                 | Unified storage + analytics           | Databricks Lakehouse                               |
| **Stream Processing**    | Process data live                         | Real-time analytics                   | Detect fraud instantly in bank                     |
| **Batch Processing**     | Process data periodically                 | Handle large historical data          | Nightly sales report                               |
| **Data Pipeline**        | Automated data movement                   | Reduces manual work                   | Daily pipeline moves CRM → Warehouse               |
| **Real-Time Processing** | Instant data calculation                  | Immediate action                      | Uber ride tracking                                 |
| **Data Modeling**        | Designing tables & relationships          | Clean structure & faster Data Engineering Termsqueries      | Fact and dimension tables                          |
| **OLTP**                 | Fast transactional system                 | Used for apps, websites               | ATM withdrawal, online order                       |
| **OLAP**                 | Analytics queries on large data           | Reporting, BI dashboards              | Monthly sales report                               |
| **Schema**               | Table structure definition                | Makes data consistent                 | Columns, types, constraints                        |
| **Star Schema**          | Fact table + dimension tables             | Faster analytics                      | Sales fact + customer dimension                    |
| **Snowflake Schema**     | Normalized star schema                    | Saves storage, clean design           | Country → State → City tables                      |
| **Distributed Systems**  | Multiple machines working together        | High availability, scalability        | Hadoop cluster, Kubernetes                         |
| **Message Queue**        | Temporary storage for messages            | Smooth communication between systems  | Kafka, SQS convey events                           |
| **Data Partitioning**    | Split big data into chunks                | Faster queries & processing           | Partition sales by date                            |
| **Data Sharding**        | Split database across servers             | Handle huge traffic                   | Instagram spreads users by shard                   |
| **Indexing**             | Quick lookup for data                     | Super fast search                     | Searching by username in DB                        |
| **Caching**              | Store frequently used data                | Faster response speed                 | Redis caching user sessions                        |
| **Orchestration**        | Manage multi-step tasks                   | Automate complex workflows            | Airflow DAG runs pipelines                         |
| **Workflow Scheduler**   | Run jobs at fixed time                    | Timed automation                      | Cron job at 2 AM                                   |
| **Fault Tolerance**      | System keeps working even when parts fail | High reliability                      | Replication across nodes                           |
| **Elasticity**           | Auto scale based on load                  | Efficient cost + performance          | Autoscaling in AWS EC2                             |
| **Scalability**          | Ability to handle more workload           | Handle growth                         | Add more nodes to cluster                          |
| **Data Governance**      | Rules & policies for data use             | Security, compliance                  | GDPR control, data access rules                    |
| **Data Quality**         | Check correctness, accuracy               | Better analytics decisions            | Removing duplicates, fixing nulls                  |
| **Data Lineage**         | Track data origin & transformations       | Auditing, debugging pipelines         | Trace data from CRM → ETL → Reports                |
| **Data Catalog**         | Central library of datasets               | Helps users search & understand data  | AWS Glue Data Catalog                              |
