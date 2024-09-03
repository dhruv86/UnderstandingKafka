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


Here are some of the important packages in the Kafka Java client library:

org.apache.kafka.clients.*: This contains the Producer, Consumer, and Admin API classes.

org.apache.kafka.connect.*: This is used to build source and sink connectors.

org.apache.kafka.streams.*: This is used to build stream processing applications.

org.apache.kafka.common.*: This deals with cross-cutting concerns like security, error handling, etc.

Let’s explore some of the classes/interfaces across some of these packages. You will see them in action throughout this course, and now is a good time to get familiar with them.




