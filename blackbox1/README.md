# Iniciar/ejecutar proyecto


docker build -t prometheus_simple .

docker run -p 9090:9090 prometheus_simple
