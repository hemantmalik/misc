### Rough, very rough -  resource impact test on the machine for filebeat's event processing

#### Setup
- Filebeat 7.6.2
- input type - log : Input logfile: 10 GB, 10.3 Million documents
- vanilla defaults
- Monitoring enabled
Noticeable Machine Neighbors
- Elasticsearch 7.6.2 - 16 GB RAM Heap (1/4th of total Machine RAM)
Machine Details:
- Windows 10 Pro 64 bit
- Virtual Memory Disabled
- Intel Core i7-9850H@2.60 GHz
- 64 GB RAM
- NVMe SSD Disk (SAMSUNG MZVLB1T0HBLR-000L7 - Novabench Benchmark: Average sequential read speed 1777 MB/s Average sequential write speed 2541 MB/s)

#### Results
>**Time taken to process: ~78 Minutes**
![Kibana Discover](https://github.com/hemantmalik/misc/blob/master/filebeat-helloperfworld-run/images/discover-screenshot.png)

>**Machine Resources Impact**
![Kibana Dashboard](https://github.com/hemantmalik/misc/blob/master/filebeat-helloperfworld-run/images/cpu-memory.png)

>**Filebeat Monitoring Details**
![Kibana Stack Monitoring](https://github.com/hemantmalik/misc/blob/master/filebeat-helloperfworld-run/images/filbeat-monitoring-head.png)
![Kibana Stack Monitoring](https://github.com/hemantmalik/misc/blob/master/filebeat-helloperfworld-run/images/filebeat-monitoring.png)
