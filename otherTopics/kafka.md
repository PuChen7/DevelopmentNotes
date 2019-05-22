# Kafka
- [Intro](#intro)
- [Kafka Topic](#Kafka-Topic)
- [Kafka Broker](#Kafka-Broker)
- [Kafka topic partition](#Kafka-topic-partition)

### Intro
- Kafka: a publish-subscribe-based durable messaging system that is exchanging data between processes, applications, and servers.
- A messaging system lets you send messages between processes, applications, and servers. 
- Apache Kafka is a software where `topics` can be defined (think of a topic as a category) to where applications can add, 
process and reprocess data (messages). Applications may connect to this system and transfer a message onto the topic.

### Kafka Topic 
- A `Topic` is a `category`/`feed` name to which messages are stored and published. 
- Messages are `byte arrays` that can store any object in any format. All Kafka `messages` are organized into `topics`.
- If you wish to send a message you send it to a specific topic and if you wish to read a message you read it from a specific topic.
- `Producer` applications write data to topics and `consumer` applications read from topics.

### Kafka Broker 
- A Kafka cluster consists of one or more servers (Kafka brokers), which are running Kafka. 
- Producers are processes that publish data (push messages) into Kafka topics within the broker. 
- A consumer of topics pulls messages off a Kafka topic. 
- `Replication` is implemented at the partition level. 

### Kafka topic partition 
- Kafka topics are divided into a number of `partitions`, which contains messages in an `unchangeable` sequence.
- Each message in a partition is assigned and identified by its unique `offset`.
