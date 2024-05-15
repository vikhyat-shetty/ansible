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
