# kafka-practice
The application includes a Kafka producer that sends messages to a Kafka topic, and a Kafka consumer that reads messages from the same topic.

## Getting Started

To run this application, you will need to have the following prerequisites:

- Apache Kafka 
- Zookeeper

Follow these steps to get started:

1. Follow the [Apache Kafka Quickstart](https://kafka.apache.org/quickstart) guide to download, install, and start a Kafka broker and ZooKeeper instance on your local machine.
2. Clone this repository to your local machine.
3. Open a new terminal window and run the following command to start the Kafka consumer:
`kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic new --from-beginning`
   This command will start the Kafka console consumer and subscribe to the "new" topic to consume messages from it.
4. Run the KafkaApplication class from within IntelliJ.
5. Once the application is running, you can send a POST request to http://localhost:8080/api/v1/messages with the following JSON payload to send a message to Kafka:
```json
   {
      "message": "api with Kafka Hooray"
   }
```

