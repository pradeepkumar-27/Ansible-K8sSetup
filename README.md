# Ansible-K8sSetup
Ansible role and playbook to launch EC2 instances on AWS  and configure them to create a Kubernetes cluster

#aws-play.yml
A playbook to launch to launch 3 EC2 instances on AWS a master and 2 slave nodes

#Role - k8s-master
Ansible role to configure master. The default pod-network-cidr is 10.244.0.0/16 but can be changed as per requirement by overriding the value of variable "cidr" under the role

#Role - k8s-slave
Anible role to configure slave nodes

#k8s-play.yml 
A playbook to implement the above roles and for the slave nodes to join the master cluster
