# Viridian consumer

### Requisitos previos
- Tener zookeper y kafka corriendo en las direcciones por defecto

`  http://localhost:2181 (zookeeper)`

`  http://localhost:9092 (kafka)`

- Tener un topic con el nombre "viridian-test"

` bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic viridian-test`

Para ejecutar el proyecto seguir los siguientes pasos:

1. Clonar el proyecto 

	`git clone https://github.com/patrickqsos/viridian-consumer.git`

2. Entrar a la carpeta del proyecto clonado

	` cd viridian-consumer`
3. Ejecutar el  proyecto

	` dotnet run`

El proyecto estara en ejecucion y mostrara en consola lo que se vaya insertando al topic

# Librerias usadas

- Confluent.Kafka Version "0.11.5": Libreria para interactuar con kafka
