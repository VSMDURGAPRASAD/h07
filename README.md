# H07 - Getting Started with Apache Kafka

Denise Case 
Northwest Missouri State University
44-564 Design of Data Intensive Systems

## Overview

Short introduction to the Kafka distributed streaming platform

We will:

1. Start ZooKeeper (clientPort=2181)
2. Start Kafka (connects to ZK)
3. Create a topic ("bearcat_messages")
4. List topics (to verify)
5. Run a producer. Send messages on our topic. 
6. Run a consumer. Get messages on our topic.

## Getting Started

- Import this repo to your Bitbucket.
- Clone from your Bitbucket down to your local computer, e.g. C:\44564\kafka\h07.

## Start ZooKeeper on port 2181

In Windows File Explorer:
- Navigate to your h07 folder.
- Right-click on your kafka_2.11-0.10.2.0 folder and "Open Command Window Here as Administrator". 

Run the batch file start_zookeeper.

```
> start_zookeeper
```



## Start Kafka 

In Windows File Explorer:
- Navigate to your h07 folder.
- Right-click on your kafka_2.11-0.10.2.0 folder and "Open Command Window Here as Administrator". 

Run the batch file start_kafka.

```
> start_kafka
```

Kafka will start and connect to ZooKeeper


## Create topic (bearcat_messages)

In Windows File Explorer:
- Navigate to your h07 folder.
- Right-click on your kafka_2.11-0.10.2.0 folder and "Open Command Window Here as Administrator". 

Run the batch file create_topic.

```
> create_topic
```

This will create a new topic named bearcat_messages.

Run the batch file list_topics to see all topics (including your new bearcat_messages).

```
> list_topics
```




## Create producer (on port 9092)

In Windows File Explorer:
- Navigate to your h07 folder.
- Right-click on your kafka_2.11-0.10.2.0 folder and "Open Command Window Here as Administrator". 

Run the batch file run_producer to start the producer.  
While the producer is running, add some messages on the topic.

```
> run_producer
  Message 1 - Go Bearcats!
  Message 2 - Forever green!!
```




## Create consumer (listening on port 9092)

In Windows File Explorer:
- Navigate to your h07 folder.
- Right-click on your kafka_2.11-0.10.2.0 folder and "Open Command Window Here as Administrator". 

Run the batch file run_consumer to start a consumer to get messages on our topic.

```
> run_consumer
```





## Resources and References

Apache Kafka https://kafka.apache.org/


Quickstart https://kafka.apache.org/quickstart


How to add "Open Command Window Here as Administrator" to context menu:
https://www.sevenforums.com/tutorials/47415-open-command-window-here-administrator.html

Verify Mrakdown with http://dillinger.io/