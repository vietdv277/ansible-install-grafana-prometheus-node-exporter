Description
------------
Playbook for automatic install grafana, prometheus and node exporter to monitoring linux server

Notice
------------

```
Prometheus version: 2.7.0
Node exporter version: 0.17.0
Ansible version >= 2.7.0
```

Variables
------------
- Change variables following your system in `group_vars/all`
```
hostname: Hostname of host will be install node_exporter
address: Ip address of host will be install node_exporter
cpus: The number of cores cpu on prometheus server host
```
- Change the ip address following your system in `hosts` file

Run Playbook
==============
```
ansible-playbook main.yml -v -e@group_vars/all
```
