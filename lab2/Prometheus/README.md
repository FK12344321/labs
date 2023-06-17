# Prometheus 
## Description:
Prometheus is a tool that collects and stores the metrics from the application 
## Purpose and benefits:
The purpose of the Prometheus is to increase an observability of an IT system my collecting and processing the metrics with an opportunity to visualize these metrics and to trigger some alerts in some predetermined cases 
## Key features and functionalities: 
Prometheus is able to pull metrics from the target application, it lets the admin to connect to its dashboard and using special query language PromQL access the collected metrics in a processed format. It also allows other applications such as Grafana to query these collected data
## Use cases and examples: 
We can use prometheus if we have an application and we want to keep track of its stability. In this case we can install the exporter for some specific framework you are using that will allow the prometheus to fetch the metrics in a special format. 

We can monitor the operating system usage of resources. We need to install Node exporter that will collect linux metrics and pass them to prometheus, so we can see how much disk space left, we can monitor the CPU load and etc
