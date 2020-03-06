# Confluent-Kafka

Testing purpose docker compose file has been created.

Pre-Req:-
---------
Step 1:- Create 6 instances from cloud with centos7 and install docker pkgs on it.
Pre-Req:-
--------
#yum install yum-utils -y && yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo && yum install docker-ce docker-ce-cli containerd.io docker-compose -y
#systemctl start docker && systemctl enable docker && systemctl status docker

Step2:- Create a docker-compose file and make it up.

[deepuf5@ansi-contorlnode confluent-kafka]$ docker-compose ps
              Name                             Command               State                 Ports
---------------------------------------------------------------------------------------------------------------
confluentkafka_ansi-client2_1       /usr/local/bin/zk-docker.sh      Up
confluentkafka_ansi-client3_1       /usr/local/bin/kafka-docker.sh   Up      0.0.0.0:19092->19092/tcp, 9092/tcp
confluentkafka_ansi-client4_1       /usr/local/bin/kafka-docker.sh   Up      0.0.0.0:29092->29092/tcp, 9092/tcp
confluentkafka_ansi-client5_1       /usr/local/bin/kafka-docker.sh   Up      0.0.0.0:39092->39092/tcp, 9092/tcp
confluentkafka_ansi-client_1        /usr/local/bin/zk-docker.sh      Up
confluentkafka_ansi-contorlnode_1   /usr/local/bin/zk-docker.sh      Up
[deepuf5@ansi-contorlnode confluent-kafka]$
