FROM nginx

# Descargar e instalar el NGINX Prometheus Exporter
RUN apt-get update && apt-get install -y wget && \
    wget https://github.com/nginxinc/nginx-prometheus-exporter/releases/download/v1.3.0/nginx-prometheus-exporter_1.3.0_linux_amd64.tar.gz && \
    tar -xvf nginx-prometheus-exporter_1.3.0_linux_amd64.tar.gz && \
    mv nginx-prometheus-exporter /usr/local/bin/ && \
    rm -f nginx-prometheus-exporter_1.3.0_linux_amd64.tar.gz
    
COPY nginx.conf /etc/nginx/nginx.conf
