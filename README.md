# Basics

### This file is mainly to understand the basic concepts in data science programming languagues like Python,R,Dask,PySpark etc.,

### **Setting Up Spark Environment**

Note: If you dont have Java Environment set up in your machine download JDK(13.0) from https://www.oracle.com/java/technologies/javase-downloads.html and set the path in environmental variables   ![image](https://user-images.githubusercontent.com/12963112/75122737-6935ae00-5666-11ea-9506-c4559d0eac0a.png)

1. Download spark-2.4.5-bin-hadoop2.7 from https://spark.apache.org/downloads.html
2. Download Hadoop 2.7 **WinUtils** from https://dzone.com/articles/working-on-apache-spark-on-windows
3. Set environmental variables for both spark and hadoop as SPARK_HOME and Hadoop_HOME and give the paths where you installed 
4. SPARK_HOME:  ![image](https://user-images.githubusercontent.com/12963112/75122903-499f8500-5668-11ea-9bbc-5a032eb9c95c.png)
5. HADOOP_HOME: ![image](https://user-images.githubusercontent.com/12963112/75122899-3db3c300-5668-11ea-8614-07b05953851a.png)
6. Set this environmental variable ![image](https://user-images.githubusercontent.com/12963112/75157855-9ae85c80-56da-11ea-8b45-77a4a77db304.png)  ---> PYSPARK_DRIVER_PYTHON
7. Add PATH VARIABLE: ![image](https://user-images.githubusercontent.com/12963112/75157968-ccf9be80-56da-11ea-8906-aff2295f67b1.png)
8. Set this environmental variable PYSPARK_DRIVER_PYTHON_OPTS  ![image](https://user-images.githubusercontent.com/12963112/75158016-ea2e8d00-56da-11ea-9c7a-a9aa40aa6920.png)
9. To start pyspark after setting environmental variables type the below command in CMD
 **pyspark --master local[2]** or I opened Jupter notebook and did the following commands
 By the above command you are starting pyspark on 2 cores
10. Once you open Jupyter note book 
![image](https://user-images.githubusercontent.com/12963112/75158350-8789c100-56db-11ea-8e18-121106df4b33.png)

or try this dummy commands to check spark working or not
**spark = SparkSession.builder.appName('abc').getOrCreate()**
**df=spark.read.csv('wx_pv_corr.csv',header=True)**


