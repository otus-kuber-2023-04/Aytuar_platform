Запускаем манифесты последовательно


- **01-config-map-nginx.yml** - ConfigMap для хранения конфигурации nginx

- **02-nginx-service.yml** - Service ClusterIP для nginx на портах 80 и 8080

- **03-nginx-service-monitor.yml** - ServiceMonitor для nginx

- **04-nginx-exporter-service.yml** - Service ClusterIP для exporter на порту 9113

- **05-nginx-deployment.yml** - сервис nginx с конфигурацией из 01-config-map-nginx.yml

- **06-exporter-deployment.yml** - сервис nginx-exporter для prometheus