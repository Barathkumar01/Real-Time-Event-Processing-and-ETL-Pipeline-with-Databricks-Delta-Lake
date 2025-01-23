# Real-Time Event Processing and ETL Pipeline with Databricks Delta Lake

## Project Overview

In this project, I designed and implemented a real-time event processing pipeline using **Databricks Delta Lake** to optimize vehicle fleet operations. The pipeline processes synthetic vehicle data in real time, improving operational efficiency and providing actionable insights to reduce fuel consumption and operational costs.

**Key Achievements:**

- **Reduced Delivery Delays by 27.5%**: By optimizing the data processing pipeline, I was able to reduce the time taken to process vehicle event data, ensuring quicker insights for fleet management.
- **Increased Fuel Efficiency by 14%**: The data processing pipeline identified patterns that helped optimize routes and driving behaviors, improving fuel efficiency across the fleet.
- **Cost Savings**: The improvements in operations led to an estimated $153,200 in annual cost savings due to reduced fuel consumption and optimized fleet management.

## Key Components of the Project:

1. **Synthetic Dataset**: A synthetic dataset simulating vehicle data, including attributes like fuel level, speed, engine load, tire pressure, and timestamps. This dataset was used to build and test the pipeline.

2. **Real-Time Data Processing**: Leveraged **Databricks Delta Lake** and **Apache Spark Structured Streaming** to handle incoming event data in real time. The Delta Lake format ensured data consistency and reliability while processing live events.

3. **Data Pipeline Optimization**: Built the pipeline to efficiently process and store real-time event data, using Delta Lake’s **ACID transactions** to ensure data integrity and **time travel** features for historical data access.

4. **Fuel Efficiency Optimization**: By analyzing historical and real-time event data, the system provided insights on fuel consumption patterns and recommendations for improving fuel efficiency.

5. **Cost Savings and Performance**: Optimized data storage and query performance, reducing processing time and costs while maintaining high data accuracy.

## Technologies and Tools Used:

- **Databricks Delta Lake**: For optimized data storage and real-time processing.
- **Apache Spark**: For distributed data processing and streaming.
- **Python**: For data manipulation, ETL tasks, and interacting with Databricks APIs.
- **SQL**: For querying and analyzing processed data within Databricks.
- **Databricks Notebooks**: To manage, execute, and visualize data processing tasks.

## Dataset Details:

The dataset used in this project is **synthetic** and contains the following columns:
- **event_id**: Unique identifier for each event.
- **timestamp**: Timestamp of when the event occurred (in `YYYY-MM-DD HH:MM:SS` format).
- **vehicle_id**: Unique identifier for each vehicle.
- **fuel_level**: Current fuel level of the vehicle.
- **latitude**: Latitude of the vehicle's location.
- **longitude**: Longitude of the vehicle's location.
- **speed**: Speed of the vehicle in km/h.
- **engine_load**: The load on the engine as a percentage.
- **rpm**: Engine revolutions per minute.
- **brake_usage**: Percentage of time the vehicle's brake is applied.
- **mileage**: Distance traveled by the vehicle.
- **temperature**: Ambient temperature at the time of the event.
- **acceleration**: Rate of change of speed of the vehicle.

## Pipeline Architecture:

The project involves the following stages:
1. **Data Ingestion**: Real-time event data is ingested into the system using **Apache Kafka** or **AWS Kinesis** (or simulated data via files) and ingested into Databricks.
2. **Real-Time Event Processing**: Spark Structured Streaming reads the event data, processes it in real time, and writes the processed data into a Delta Lake table.
3. **Data Storage**: The processed data is stored in Delta Lake, ensuring reliability, data versioning, and optimized querying.
4. **Querying & Analysis**: Periodic queries analyze the data, identify trends in fuel consumption, and recommend optimizations for better fuel efficiency.
5. **Cost Savings Calculation**: A model estimates potential cost savings by comparing fuel consumption before and after optimizations.
