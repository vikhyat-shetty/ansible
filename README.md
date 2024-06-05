# Install Prometheus, Grafana and Node Exporter to targeted machines using Ansible Playbook

## Step 1:
[Clone the repository into a machine]

## Step 2:
[Populate the invventory file with the hostnames of the targeted machines for each of the respctive services]

## Step 3:
[Run the following playbook using the below command to enable jmx exporter]

```sh
ansible-playbook -i inventory/ansible-inventory_copy.yml deploy.yml
```

## Links for downloading tar files manually

Node Exporter

```sh
https://github.com/prometheus/node_exporter/releases/download/v{{ node_exporter_version }}/node_exporter-{{ node_exporter_version }}.linux-amd64.tar.gz
```

Prometheus

```sh
https://github.com/prometheus/prometheus/releases/download/v{{ prometheus_version }}/prometheus-{{ prometheus_version }}.linux-amd64.tar.gz
```

Grafana

```sh
https://dl.grafana.com/oss/release/grafana-{{ grafana_version }}.linux-amd64.tar.gz
```