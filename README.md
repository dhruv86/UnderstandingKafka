# Understanding Kafka
Understanding Apache Kafka

**Start the topic**

```
cd /app/confluent-7.3.1/bin

./kafka-topics --bootstrap-server localhost:9092 --create --partitions 2 --replication-factor 1 --topic test

```

**Start the Consumer CLI**

```
cd /app/confluent-7.3.1/bin

./kafka-console-consumer --bootstrap-server localhost:9092 --topic test

```
