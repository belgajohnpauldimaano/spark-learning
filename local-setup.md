#### Download applications
- java11 using brew
- python3
- spark from official website

#### Setup spark
1. create directory in home dir `mkdir ~/spark`
2. move spark from Downloads to `~/spark`, `mv ~/Downloads/spark.... ~/spark`
3. extract spark using `tar -zxvf spark....`

#### Setup home variables
add this to your `.zshrc`
```
export JAVA_HOME=/usr/local/Cellar/openjdk@11/11.0.20
export SPARK_HOME=/Users/<user>/spark/spark-3.4.1-bin-hadoop3
export PATH=$PATH:$SPARK_HOME/bin
```

#### Start pyspark
```
  pyspark --driver-memory 2G
```