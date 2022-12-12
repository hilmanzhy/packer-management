# deployment-netsight-project

### Configure
This configure to manage and deployment netsight project with Ansible.
```shell

ansible-playbook pip3.yml -t pip3
ansible-playbook package.yml -t package
ansible-playbook create_speed.yml -t create
ansible-playbook upload_speedtest.yml -t upload
ansible-playbook create_trace.yml -t create
ansible-playbook upload_trace.yml -t upload
ansible-playbook create_prometheus.yml -t create
ansible-playbook setup_prometheus.yml -t setup
ansible-playbook setup_ping_exporter.yml -t setup
ansible-playbook upload_pingtest.yml -t upload

```

This configure to install and deployment via docker
```shell

ping your server to know that's available or not "ansible -m ping your-host"
ansible-playbook pip3.yml -t pip3
ansible-playbook docker.yml
ansible-playbook package.yml -t package
ansible-playbook setup_docker.yml -t setup

```

With Ansible, everything is so easy to deploy and manage your server.
