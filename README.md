## node exporter service
If you want to let just specific IPs can see the node exporter port: change `whitelist_port` variable to `true` in `main.yml`

run:
```
ansible-playbook -i path/to/inventory main.yml
```

## node exporter docker
If you want to run node exporter in a container just run this command:
```
docker run -d --name node_exporter -p 9100:9100 prom/node-exporter:latest
```