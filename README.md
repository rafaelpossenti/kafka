# kafka

	• Download: 
	https://kafka.apache.org/downloads
	
	• Rodar Kafka localmente: 
	bin/zookeeper-server-start.sh config/zookeeper.properties
	bin/kafka-server-start.sh config/server.properties
	
	• Criar novo tópico:
	bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic LOJA_NOVO_PEDIDO
	
	• Listar tópicos:
	bin/kafka-topics.sh --list --bootstrap-server localhost:9092
	
	• Produzir mensagens:
	bin/kafka-console-producer.sh --broker-list localhost:9092 --topic LOJA_NOVO_PEDIDO
	
	• Consumir mensagens: bin/kafka-console-consumer.sh  --bootstrap-server localhost:9092 --topic LOJA_NOVO_PEDIDO --from-beginning
