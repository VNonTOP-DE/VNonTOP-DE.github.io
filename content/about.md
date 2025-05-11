---
title: "About Me"
---

## From Problem Solver to Data Engineer
Hey there! I'm Tuan, and I've always loved solving problems. Back in high school, my friends and I would brainstorm fixes for everyday headaches like traffic jams, elevator efficiency, or parking chaos—like it was our little mission to make life better. But it's not just the big stuff that grabs me; I'm just as hooked on tackling challenges closer to home.


Take my mom's Ao Dai shop, for instance. She runs this cool little business selling these gorgeous traditional dresses, but with so many styles and sizes, keeping track of inventory is a total nightmare. She's the only one who knows where everything is, and if she's not around, we're all stuck—no one else can step in to help customers. It's been a puzzle I've wanted to crack for a while.


Then I discovered data engineering, and it was like a lightbulb went off. I realized I could use data to organize her inventory, track what's selling, and maybe even predict what customers might want next. It was the perfect way to mix my passion for problem-solving with something that means a lot to me. The more I dug into it, the more excited I got—working with data is like cracking a code, and I'm all about that challenge.


That's why I'm so pumped to apply for this fresher data engineer position. I might be new to the field, but I bring a ton of enthusiasm and a fresh perspective. I've seen how data can solve real problems—like making my mom's shop run smoother—and I'm eager to jump in, learn everything I can, and help your team tackle some awesome challenges. I'd love to bring my problem-solving passion and curiosity to the table!


## Technical Skills

### Databases

#### Structured Data

**PostgreSQL**
- Designed and optimized relational schemas with proper normalization (3NF)
- Implemented table partitioning (RANGE, LIST, HASH) for large datasets
- Created advanced indexes (B-tree, GIN, BRIN) to optimize query performance

#### Semi-structured Data

**Graph Database (Passion)**
- Designed comprehensive data models with graph structures, including nodes, relationships, testing, and refactoring
- Optimized query performance using intermediate nodes and specific relationships
- Added flexible labels to adapt to various purposes and use cases

**MongoDB**
- Designed document schemas with optimal embedding and referencing strategies
- Implemented sharding for horizontal scaling using hashed and ranged shard keys
- Configured replica sets for high availability with automatic failover

**Snowflake**
- Designed schemas combining structured tables and VARIANT columns for semi-structured data
- Implemented zero-copy cloning for efficient testing environments
- Configured automatic clustering for large JSON datasets
- Processed semi-structured data using LATERAL FLATTEN, PARSE_JSON, and dot notation
- Built continuous data pipelines with Snowpipe
- Transformed JSON data using JavaScript UDFs

#### Unstructured Data
- Stored in S3 with lifecycle policies for efficient management
- Extracted text using AWS Textract and Tesseract
- Indexed in Elasticsearch with metadata tagging for searchability
- Processed via Spark on EMR for binary decoding
- Stored parsed data in Parquet format and raw data in S3

### ETL Processes

#### Extract

**Scrapy (Proficient)**
- Built Crawl Spiders for rule-based scraping, handling pagination and category traversal
- Created API Scrapers to extract JSON data from XHR requests
- Designed Recursive Crawlers for deep website traversal
- Wrote custom pipelines for deduplication (hash-based filtering), data validation (checking missing fields), and exporting to CSV, JSON, and databases
- Implemented anti-scraping techniques: User-Agent rotation, proxies, request throttling (AutoThrottle), and CAPTCHA handling with 2CAPTCHA

#### Transform

**PySpark (Proficient)**

*Spark Core (RDD)*
- Set up RDDs and imported big data from various sources (text, key-value, lists)
- Applied transformations using map, reduce, and other lambda functions
- Used UDFs in Python/Scala for custom logic
- Handled millions of rows for data cleaning, checking for missing fields (name, age, email), invalid ages (<0 or >120), and malformed emails

*SparkSQL*
- Set up dataframes with complex nested schemas
- Applied SQL queries for data analysis (count, tokenize, average)
- Cleaned and filtered messy date data

#### Load

**Apache Spark for Batch Processing (Proficient)**
- Read from diverse sources (e.g., Parquet, JDBC) with commands like df = spark.read.format("parquet").load("s3://path")
- Handled schema inference and manual schema definition
- Processed terabyte-scale datasets with partitioning (repartition, coalesce)

**Apache Kafka**
- Set up producers with high throughput (100K+ messages/sec) by tuning batch.size and linger.ms
- Used formats like Avro (with Schema Registry), JSON, and Protobuf
- Configured consumer groups for parallel processing with exactly-once semantics
- Managed replication (3x replica factor) and partitioning (100+ partitions) for high availability and scalability
- Monitored lag (consumer offsets) and broker metrics (JMX/Prometheus)

### Orchestration

**Apache Airflow (Proficient)**

*Workflow Design*
- Built DAGs with Python to manage task sequences
- Defined task dependencies using >> (e.g., extract_task >> transform_task >> load_task)
- Used dynamic DAG generation for parameterized workflows

*Operators & Integrations*
- Utilized BashOperator (shell commands), PythonOperator (Python functions), KubernetesPodOperator (containers), and Sensors (external conditions)

*Key Features*
- Configured retries (e.g., retries=3) and Slack alerts on failure
- Performed backfilling for historical data reprocessing
- Used XComs to share data between tasks

### AI for Automation

**N8n**
- Built end-to-end automations using over 300 pre-built nodes
  - Trigger Nodes: Webhooks, Cron, Email, Telegram
  - Action Nodes: HTTP Requests, SQL Queries, Slack/Teams notifications
  - Logic Nodes: IF/Switch conditions, Merge, Wait
- Integrations
  - Connected to databases (PostgreSQL, MongoDB)
  - Automated SaaS tools (HubSpot, Salesforce)
  - Processed files with S3 and Google Drive


 

## Education
- Bachelor Degree in [Economics]
- University of Economics Ho Chi Minh City

## Social Media
- [LinkedIn](https://www.linkedin.com/in/tuan-nguyen-hoang-139b5b249/)
- [GitHub](https://github.com/VNonTOP-DE)