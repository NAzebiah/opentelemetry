# Monitoring Microservices application using OpenTelemetry 
Reference Documentation: https://opentelemetry.io/docs/

# 1. Install and Configure Microservices Application:  

    cd opentelemetry-helm
    helm dependency update
    helm install opentelemetry-app charts/opentelemetry-app-*.tgz

# 2. Install and Configure Open Telemetry Collector:  

This will collect traces from application and captures at the collector port.

    helm install opentelemetry-collector charts/opentelemetry-collector-*.tgz

# 3. Install and Configure Jaeger:  

    helm install jaeger charts/jaeger-*.tgz

# 4. Install and Configure Prometheus:  

    helm install prometheus charts/prometheus-*.tgz

# 5. Install and Configure Grafana:  

    helm install grafana charts/grafana-*.tgz