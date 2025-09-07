# Налаштування GitOps-інфраструктури
![img.png](img.png)
Налаштовано та розгорнуто GitOps-інфраструктуру з наступним стеком:
* minikube
* VictoriaMetrics
* Grafana
* Application

## Prerequisites
| Технологія         | Version                       |
|--------------------|-------------------------------|
| minikube           | v1.36.0                       |
| kubectl client     | v1.32.2                       |
| kubectl server     | v1.33.1                       |
| helm               | v3.18.6                              |
| VictoriaMetrics    | victoriametrics/victoria-metrics:latest |
| Grafana            | grafana/grafana:latest        |
| vmagent            | victoriametrics/vmagent:latest        |
| kube-state-metrics | bitnami/kube-state-metrics:latest        |
| Application        | andriiuni/spam2000:1.1394.355           |
## Запуск кластера
Після підняття minikube кластера інфраструктура розгортається однією командою:
```bash
helm install <realease_name> .\Application\