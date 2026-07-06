# win-lgtm
### LGTM Observability Stack for Windows Server

This Docker Compose stack was created to demonstrate an LGTM stack on Windows Server 2022 with the following components:
- WSL
- Docker
- Python
- Docker Compose
- GitHub Desktop
- Docker Desktop

The LGTM stack includes the following containers:

- Loki for log storage
- Grafana for visualization
- Tempo for trace storage
- Prometheus for metric storage

While, LGTM implies using Mimir for metrics, it's based on Prometheus and is more widely supported.


### Storage requirements for production
This deployment uses a regular file system for the databases. According to documentation, this is not suitable for production deployments. The ideal configuration is to use object storage such as S3 or Azure Blob Storage.