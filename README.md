# kafka-notes
## Start kafka in the wsl2 docker in ubuntu
To start kafka broker in the wsl2 in ubuntu, hostname is not yet well fixed so you need to use 
this command to get the IP of your hostname <br/>
`$ ip addr | grep "eth0"` <br/>
172.x.y.z <br/>
`docker run --name kafka -p 9092:9092 -e KAFKA_ZOOKEEPER_CONNECT=172.261.32.14:2181 -e KAFKA_ADVERTISED_LISTENERS=PLAINTEXT://172.261.32.14:9092
-e KAFKA_OFFSETS_TOPIC_REPLICATION_FACTOR=1 confluentinc/cp-kafka`
