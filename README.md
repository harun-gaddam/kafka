# kafka
Here's a guide on how to install and run Kafka on both Mac and Windows:

## Mac Installation Steps:
1. Download Kafka binary from the [Kafka download page](https://kafka.apache.org/downloads).
2. Unzip Kafka by running the following command in the terminal: `tar -xzf kafka_2.13-3.0.0.tgz`
3. Navigate to the Kafka folder: `cd kafka_2.13-3.0.0`
4. Start ZooKeeper: `bin/zookeeper-server-start.sh config/zookeeper.properties`
5. Start Kafka Server in another terminal: `bin/kafka-server-start.sh config/server.properties`

For detailed instructions and screenshots, you can refer to this link: [Install Kafka on Mac](https://hevodata.com/learn/install-kafka-on-mac/)

## Windows Installation Steps:
1. Download the Kafka binary file for Windows.
2. Extract the file and move the extracted folder to your preferred directory.
3. Copy the path of the Kafka folder. Open the `zookeeper.properties` file located in the `config` folder. Paste the copied path after `dataDir`, adding `/zookeeper-data` to the path.
4. In the same `config` folder, open `server.properties`. Scroll down to `log.dirs` and paste the Kafka folder path. Add `/kafka-logs` to the path.
5. Open the command prompt and navigate to the Kafka folder. Start ZooKeeper using the following command:
   `.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties`

6. Open another command prompt and navigate to the Kafka folder. Run Kafka Server using the command:
   `.\bin\windows\kafka-server-start.bat .\config\server.properties`

For detailed instructions and screenshots, you can refer to this link: [Install Kafka on Windows](https://www.geeksforgeeks.org/how-to-install-and-run-apache-kafka-on-windows/)

These instructions provide a simplified overview of the installation process for Kafka on Mac and Windows. For more detailed instructions, please refer to the official Kafka documentation.
