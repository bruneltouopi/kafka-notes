### Create a cluster cgp-exercise on gcp cloud
 ```
 confluent kafka cluster create cgp-exercise --cloud gcp --region us-west4 --environment env-227pp1
 ```
 
 ### Create a topic in a cluster with 2 partitions
 ```
 confluent kafka topic create test-1 --partitions 2 --cluster lkc-zgp2yy
 ```
