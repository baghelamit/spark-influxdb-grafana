# Spark InfluxDB Grafana
This repository contains JSON file exported from Grafana. This JSON file shows metrics collected by JVM Profiler. Below is the architecture diagram for Performance Monitoring System. Read the article at [InfoQ](https://www.infoq.com/articles/spark-application-monitoring-influxdb-grafana)

![Performance Monitoring System Architecture](https://github.com/baghelamit/spark-influxdb-grafana/blob/master/architecture.jpg)


This Performance Monitoring System is based on Uber JVM Profiler. `InfluxDBOutputReporter` has been merged with Uber code base and it is now  available [here](https://github.com/uber-common/jvm-profiler/tree/master/src/main/java_influxdb/com/uber/profiling/reporters). Use below command to build the `jvm-profiler.jar` with InfluxDBOutputReporter.

```
git clone https://github.com/uber-common/jvm-profiler.git

mvn -P influxdb clean package

```
