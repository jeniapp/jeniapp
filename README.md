# Steps for Accessing the Cluster

1. Check if 'data228project' is listed:
```bash
gcloud projects list
```
2. Log in to your Google Cloud:
```bash
gcloud auth login
```
3. Set your active project to 'data228project':
```bash
gcloud config set project data228project-443300
```
4. Log in to the Master node (SSH into the cluster):
```bash
gcloud compute ssh stock-cluster-m --zone=us-central1-b
```
5. Passkey: 12345
6. You can run this code, and find that our data is in HDFS:
```bash
hdfs dfs -ls /user/stock_market_data/stock_market_data
```
## How to use Spark
7. Start PySpark on the Cluster after you log in to the master node:
```bash
pyspark --master yarn --deploy-mode client
```
8. Use Spark to read the dataset from HDFS (this is an example of just reading only 'forbes2000' files):
```bash
from pyspark.sql import SparkSession

spark = SparkSession.builder.appName("Stock Market Analysis").getOrCreate()

# define HDFS path
forbes2000_path = "hdfs://stock-cluster-m/user/stock_market_data/forbes2000/csv"

# read only Forbes2000 csv files
forbes2000_df = spark.read.csv(forbes2000_path, header=True, inferSchema=True)

# show preview
forbes2000_df.show(5)
```


