# AnsibleProject-NTP-Apache
Configuring Client With Services Through Master Using Ansible

First You need 2 VMs one to act as master and one to act as client

1)From client side :

• add master entry in /etc/hosts

• generate ssh key

• save and leave client machine open

2)From Master Side :

• add Client entry in /etc/hosts

• generate ssh key

• Exchange keys with client

• update os

• install python3,ansible,ansible-galaxy,git and epel-release

•	add key in /etc/ansible/key.pem

•	Create Directory for project having 2 roles (1 for ntp/chronny and 1 for apache) and 2 playbooks (1 for ntp/chronny and 1 for httpd)

•	Add client in /"Directory-name"/inventories/hosts 

[webservers]
Webserver1 ansible_host=Client-IP-Address ansible_user=Username-in-client-machine ansible_ssh_private_key_file=/etc/ansible/key.pem




