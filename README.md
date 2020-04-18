Microservice Deposit
=====

**Stack del proyecto:**

* Spring Boot
* PostgreSQL
* Kafka
* Docker

## Pre-Requisitos

* Tener java configurado.
* Tener docker y docker-compose instalados.
* En PostgreSQL, crear una base de datos llamada **`db_account`**.

## Ejecución del proyecto en local

* Levantar los servicios externos ejecutando **`make up`** en linux y **`docker-compose up`** en windows.
* Realizar un depósito: **` Tipo POST - http://localhost:8006/v1/depositEvent`**.

~~~
{
	"amount": 100,
	"type": "depósito",
	"creationDate": "14/11/2020",
	"accoundId": 1
}
~~~
