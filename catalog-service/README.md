docker run -d --network ecommerce-network \
--name catalog-service \
-e "spring.cloud.config.uri=http://config-service:8888" \
-e "spring.rabbitmq.host=rabbitmq" \
-e "eureka.client.serviceUrl.defaultZone=http://discovery-service:8761/eureka/" \
-e "logging.file=/api-logs/catalogs-ws.log" \
kangjm2/catalog-service:1.0