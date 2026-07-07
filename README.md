# win-lgtm
### LGTM Observability Stack for Windows Server

This Docker Compose stack was created to demonstrate an LGTM stack on Windows Server 2022. It can be run on Linux but you have to reformat the bind mounts. I used the following tools:
- WSL
- Docker
- Python
- Docker Compose
- GitHub Desktop
- Docker Desktop

The LGTM stack includes 5 containers:
- Loki for log storage
- Grafana for visualization
- Tempo for trace storage
- Prometheus for metric storage
- Cadvisor for container metrics

Cadvisor captures performance metrics of other containers. Prometheus has a scrape config to automatically capture all of the metrics. A dashboard is included in this repo to observe the containers right out of the box.

### Deploy this stack

There are two steps to deploy win-lgtm from a powershell prompt:
1 git clone https://github.com/CloudEric/win-lgtm
2 docker compose up