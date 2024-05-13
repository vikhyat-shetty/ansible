# Install Prometheus and Grafana to a VM using Ansible Playbook

## Step 1:
[Clone the repository into a machine]

## Step 2:
[Run the following playbook using the below command to enable jmx exporter]

```sh
ansible-playbook -i hosts ./playbooks/enable_jmx_exporter.yml
```
Note: This playbook works only if CP ansible is installed in the system and ansible-inventory.yml is the inventory file for CP Ansible.

## Step 3:
[Run the CP Ansible playbook with the below command to update the cluster with the new setting]

```sh
ansible-playbook -i ansible-inventory.yml confluent.platform.all
```
Note: The command could vary according to your setup

## Step 4:
[Run the following playbook using the below command to install prometheus and Grafana]

```sh
ansible-playbook -i hosts ./playbooks/install_prometheus_grafana.yml
```
