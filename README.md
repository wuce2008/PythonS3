# JupyterPySpark

Implement Jupyter in Docker

Read json files from AWS S3

# Prerequistes

MacOS

Docker (version 19.03.13)

download hadoop-aws jar https://mvnrepository.com/artifact/org.apache.hadoop/hadoop-aws

and aws-java-sdk-core jar https://mvnrepository.com/artifact/com.amazonaws/aws-java-sdk-core/1.11.954

# Step 1

Implement Jupyter Spark image in Docker.

run following shell command

```shell
docker pull jupyter/all-spark-notebook
```

# Step 2

Run container using port 8888:8888 (-p), name the container as jupyter-all-spark (-name), remove container after exit (-) 

run following shell command

```shell
docker run -p 8888:8888 --name jupyter-all-spark --rm jupyter/all-spark-notebook
```

# Step 3

While running container jupyter-all-spark, the shell show your message of the url to open jupyter. 

```
To access the notebook, open this file in a browser:
  file:///home/jovyan/.local/share/jupyter/runtime/nbserver-6-open.html
Or copy and paste one of these URLs:
  http://host:8888/?toek=abc
or http://host:port/?token=abc
```

Copy the url http://host:port/?token=abc. Open it in browser to open Jupyter notebook.

# Step 4

Make sure 











