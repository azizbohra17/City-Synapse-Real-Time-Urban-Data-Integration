Smart City Streaming

Overview

"Smart City Streaming" is a real-time data processing project that simulates a smart city environment. It utilizes IoT devices, Apache Zookeeper, Apache Kafka, Apache Spark, Docker, Python, AWS Cloud services, and PowerBI to cover each phase from data ingestion to processing and finally storage and visualization.

System Architecture

The project architecture involves several components working together to simulate and process real-time data from a smart city:

IoT Devices: Generate simulated data for various city aspects, including vehicle movements, GPS coordinates, traffic conditions, weather updates, and emergency incidents.
Apache Zookeeper & Apache Kafka: Manage and stream data between different components.
Apache Spark: Process the streaming data in real-time.
Docker: Containerize the services for easier deployment and management.
AWS Services: Store processed data (AWS S3), manage access (AWS IAM), catalog data (AWS Glue), query data (AWS Athena), and data warehousing (AWS Redshift).
PowerBI: Visualize the processed data stored in Redshift.
Setup and Installation

Detailed setup and installation instructions can be found in the Project Setup section.

Project Setup

Docker Containers Setup: Set up Docker containers for Zookeeper, Kafka, and Spark.
IoT Services Producer: Simulate IoT data for vehicles, GPS, traffic, weather, and emergency incidents.
Producing IoT Data to Kafka: Stream the simulated data to Kafka topics.
AWS S3 Setup: Configure S3 buckets for storing processed data.
AWS IAM Roles and Credentials Management: Set up IAM roles and policies for secure access to AWS services.
Apache Spark Realtime Streaming from Kafka: Process the streaming data using Spark structured streaming.
AWS Glue Crawlers: Catalog the processed data in Glue for easier querying.
Working with AWS Athena: Query the cataloged data using Athena.
Loading Data into Redshift: Store the processed data in Redshift for analytics and visualization.
Connecting and Querying Redshift: Use DBeaver to connect and query the Redshift data warehouse.
Connecting Redshift to AWS Glue Catalog: Integrate Redshift with the Glue Data Catalog.
Visualizing Data with PowerBI: Connect PowerBI to Redshift and create dashboards for data visualization.
