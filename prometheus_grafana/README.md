<!-- Prometheus -->
<!-- https://prometheus.io/docs/prometheus/latest/installation/ -->

docker run -d -p 9090:9090 \
    --network ecommerce-network \
    --name prometheus \
    -v /Users/jaemin/Desktop/working/SpringCloud/prometheus_grafana/prometheus.yml:/etc/prometheus/prometheus.yml \
    prom/prometheus

<!-- Grafana -->
<!-- https://grafana.com/grafana/download?pg=get&plcmt=selfmanaged-box1-cta1&platform=docker -->

docker run -d -p 3000:3000 \
    --network ecommerce-network \
    --name=grafana grafana/grafana