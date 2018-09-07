# kafka-consumer-demo

<h2>Spring Boot with Kafka Consumer Example</h2>

This Project covers how to use Spring Boot with Spring Kafka to Consume JSON/String message from Kafka topics

<h2>Start Zookeeper</h2>
bin/zookeeper-server-start.sh config/zookeeper.properties

<h2>Start Kafka Server</h2>
bin/kafka-server-start.sh config/server.properties

<h2>Create Kafka Topic</h2>
bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Kafka_Example

bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Kafka_Example_json

<h2>Publish to the Kafka Topic via Console</h2>
bin/kafka-console-producer.sh --broker-list localhost:9092 --topic Kafka_Example

bin/kafka-console-producer.sh --broker-list localhost:9092 --topic Kafka_Example_json
