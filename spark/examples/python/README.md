# Apache Spark demo example (Python)
This is a starter app for the Apache Spark Python template.

## Running the application on a Spark standalone cluster via Docker

To run the application, execute the following steps:

1. Setup a Spark cluster as described on https://github.com/ngocvien21/RideInsight-Scalable-Big-Data-Analytics-Platform/edit/main/spark by just running: 
    ```bash
    git https://github.com/ngocvien21/RideInsight-Scalable-Big-Data-Analytics-Platform.git
    cd docker-spark
    docker-compose up -d
    ```
2. Build the Docker image:
    ```bash
    bash build.sh python-example examples/python
    ```
3. Run the Docker container:
    ```bash
    docker run --rm --network dockerspark_default --name pyspark-example bde2020/spark-python-example:3.3.0-hadoop3.3
    ```
