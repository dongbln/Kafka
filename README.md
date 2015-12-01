# Kafka
Apache Kafka.
If you want to use Kafka with Scala, you must make sure the version of your Scala match with Kafka you are going to install.
## Installation
1. Download Kafka
2. mkdir ```myKafka```
3. cd myKafka
4. ```cp ~/Downloads/kafka_2.11-0.9.0.0.tgz .```
5. ```tar xzf kafka_2.11-0.9.0.0.tgz ```
6. Make DIR for logs of Kafka  for e.g., two Kafka brokers in the same machine ```mkdir kafka-log1 ```, ``` mkdir kafka-log2 ```
7. Configure Kafka ``` vi config/server.properties ```
8. Make sure broker.id is unique
9. Specify the log path in the log section e.g., ```log.dirs=~/dev/myKafka/kafka-log1/kafka-logs ```
10. Specify your Zookeeper url if you have already installed on your organization
11. Save the config and quit
12. Start Zookeeper (Do not do this in production) ```bin/zookeeper-server-start.sh config/zookeeper.properties  & ```
13. Start Kafka Broker 1 ```bin/kafka-server-start.sh config/server.properties & ```
14. 






