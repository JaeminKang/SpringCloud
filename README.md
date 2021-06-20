# SpringCloud

* rabbitmq : 172.18.0.2/16 : 5671
* config-service : 172.18.0.3/16 : 8888
* discovery-service : 172.18.0.4/16 : 8761
* apigateway-service : 172.18.0.5/16 : 8000
* mariadb : 172.18.0.6/16 : 3306
* kafka-docker_zookeeper : 172.18.0.100/16 : 2181
* kafka-docker_kafka : 172.18.0.101/16 : 9092
* zipkin : 172.18.0.9/16 : 9411
* prometheus : 172.18.0.10/16 : 9090
* grafana : 172.18.0.11/16 : 3000
* user-service : - : - 
* order-service : - : -
* catalog-service : - : -

(1) mvn spring-boot:run -Dspring-boot.run.arguments=--spring.profiles.active=production
(2) java -Dspring.profiles.active=default XXXX.jar