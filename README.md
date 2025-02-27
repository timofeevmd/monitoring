# monitoring

set up:

```bash
docker compose -f monitoring.yml up -d
```

connect prometheus db on grafana:

go to -> /connections/add-new-connection
select prometheus
hit add new data source btn
set http:127.0.0.1:9090 to the inputfield "Prometheus server URL *"

dashboards
- [cAdvisor](https://grafana.com/grafana/dashboards/14282-cadvisor-exporter/) : 14282 
- [node_exporter](https://grafana.com/grafana/dashboards/1860-node-exporter-full/) : 1860