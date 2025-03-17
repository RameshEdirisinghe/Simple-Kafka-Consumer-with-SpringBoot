# Spring Boot with Kafka Consumer Example

This Project covers how to use Spring Boot with Spring Kafka to Consume JSON/String message from a Kafka topic

### Below are the command for Linux/Mac and Windows

## Start Zookeeper
- `.\bin\windows\zookeeper-server-start.bat config\zookeeper.properties`

## Start Kafka Server
- `.\bin\windows\kafka-server-start.bat config\server.properties`

## Create Kafka Topic
- `.\bin\windows\kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic NewTopic`

## Consume from the Kafka Topic via Console
- `.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic NewTopic --from-beginning`

## Enable Kafka Topic
- `.\bin\windows\kafka-console-producer.bat --broker-lost localhost:9092 --topic NewTopic`
