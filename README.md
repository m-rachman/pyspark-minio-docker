# Installation Spark and Jupyter notebook (spark 3.5.1 with bitnami version)

---


   * Run the following command to build the Docker image:
    ```bash
    make build
    ```
    or
    ```
    docker-compose build
    ```

   * After building the image,create docker-compose by the following command  :

     ```bash
     make up
     ```
     or
     ```bash
     docker-compose up -d
     ```
    * Get Jupyter notebook token
      ```bash
      docker logs spark-notebook
      ```

    * Open Jupyter notebook
      http://localhost:8888/lab?token=abcxyz

    Spark UI
    * Master: http://localhost:8080/
    * Jobs: http://localhost:4040/jobs/

    MinIO UI
    * http://localhost:9001/

    ## Authors
    The original repository is from [here] (https://github.com/ongxuanhong/de02-pyspark-optimization), and the content is from this [article:] (https://medium.com/@ongxuanhong/dataops-02-spawn-up-apache-spark-infrastructure-by-using-docker-fec518698993). I only updated the Spark version from 3.3.1 to 3.5.0 because the original URL link is out-of-date

