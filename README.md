## Spring Kafka

This is a simple Spring Boot app to demonstrate sending and receiving of messages in Kafka using spring-kafka.

As Kafka topics are not created automatically by default, this application requires that you create the following topics manually.

Run these commands in opt/kafka/bin folder within kafka Docker container.

`$ ./kafka-topics.sh --create --zookeeper zookeeper:2181 --replication-factor 1 --partitions 1 --topic danielmisina`<br>
`$ ./kafka-topics.sh --create --zookeeper zookeeper:2181 --replication-factor 1 --partitions 5 --topic partitioned`<br>
`$ ./kafka-topics.sh --create --zookeeper zookeeper:2181 --replication-factor 1 --partitions 1 --topic filtered`<br>
`$ ./kafka-topics.sh --create --zookeeper zookeeper:2181 --replication-factor 1 --partitions 1 --topic greeting`<br>