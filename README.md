# kubernetes-via-Ansible-on-ubunut18.04

- This is a repository to build 3 nodes k8s cluster with 1 master node and 2 worker nodes.

## Pre-requisite
- 3 VMs with ubuntu 18.04
- 1 machine with ansible installed and sshpass installed


## Steps
* clone the repository
* update the inventory file as per your VMs
* Run the below command -> This command will configure all 3 nodes with common packages and setup
```
ansible-playbook common.yml -i inventory
```
* Run below command to setup the worker nodes
```
ansible-playbook nodes.yml -i inventory
```
