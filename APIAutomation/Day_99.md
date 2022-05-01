## Learning Goal
Testing simple kafka message

### Problem statement
You need to test if a kafka message published by a producer is received by two clients.

### Steps to automate:
1. Install kafka and start the kafka browser and zookeeper(you can use docker)
2. Start consumer1 who is listening to a particular topic say "TOPIC 1"
3. Start the producer and publish a message "Hello" to the same topic "TOPIC 1"
4. Validate the consumer 1 received the message "Hello" from topic "TOPIC 1"
5. Start consumer2 who is listening to same topic  "TOPIC 1"
6. Validate the consumer 2 also received the message "Hello" published on topic "TOPIC 1"
