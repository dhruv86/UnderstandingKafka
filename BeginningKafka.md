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

**Invoking the Producer CLI**

```
cd /app/confluent-7.3.1/bin

./kafka-console-producer --bootstrap-server localhost:9092 --topic test

```
You should see a > prompt when the producer is ready. Enter the messages you want to send to the topic (press the “Enter” key after each message).

Go back to the consumer terminal to verify that the messages were received.

The Kafka Java client library allows JVM-based applications to interact with the Kafka cluster. Let’s look at the package structure, along with the key classes/interfaces.


**Packages in the Kafka Java client library**

<img width="1351" alt="image" src="https://github.com/user-attachments/assets/2639307e-883e-4d20-9b0c-73bb4189e3f0">





