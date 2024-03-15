# City Synapse: Real-Time Urban Data Integration

## Overview
"City Synapse: Real-Time Urban Data Integration" is an end-to-end real-time data streaming pipeline designed to simulate and analyze data from a vehicle traveling from London to Birmingham. The project leverages a range of technologies including IoT devices, Apache Zookeeper, Apache Kafka, Apache Spark, Docker, Python, AWS Cloud (AWS S3, AWS Glue, AWS Athena, AWS IAM, AWS Redshift), and PowerBI for data visualization.

## Architecture
The system architecture consists of the following components:
- **IoT Devices**: Simulate the vehicle, GPS, weather, traffic, and emergency incident data.
- **Apache Zookeeper & Kafka**: Manage and stream data from IoT devices.
- **Apache Spark**: Process and analyze the streamed data in real-time.
- **Docker**: Containerize the services for easy deployment and scaling.
- **AWS Services**: Store, process, and analyze the data using AWS S3, AWS Glue, AWS Athena, and AWS Redshift.
- **PowerBI**: Visualize the data stored in AWS Redshift.

## Setup and Installation
1. **Docker**: Ensure Docker is installed on your machine. If not, download and install Docker from [Docker's official website](https://www.docker.com/).
2. **Clone the Repository**: Clone this repository to your local machine using `git clone https://github.com/your-username/smart-city-streaming.git`.
3. **Build and Run Docker Containers**: Navigate to the project directory and run `docker-compose up --build` to set up the Apache Zookeeper, Kafka, and Spark containers.
4. **Configure AWS Services**: Set up AWS S3, Glue, Athena, and Redshift with the necessary permissions and configurations.

## Running the Simulation
1. **Start Producers**: Run the IoT data producers to simulate vehicle, GPS, weather, traffic, and emergency incident data.
2. **Stream Data to Kafka**: The simulated data is streamed to Kafka topics.
3. **Process Data with Spark**: Apache Spark processes and analyzes the data in real-time.
4. **Store Data in AWS S3**: The processed data is stored in an AWS S3 bucket.
5. **Catalog Data with AWS Glue**: Use AWS Glue to catalog the data for easier querying.
6. **Query Data with AWS Athena**: Analyze the data using SQL queries in AWS Athena.
7. **Load Data into AWS Redshift**: Transfer the data to AWS Redshift for further analysis and visualization.
8. **Visualize with PowerBI**: Connect PowerBI to AWS Redshift to create dashboards and visualizations.


## Acknowledgements
Special thanks to Yusuf Ganiyu for the comprehensive video tutorial that guided the development of this project.
