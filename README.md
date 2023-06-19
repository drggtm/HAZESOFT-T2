
# HAZESOFT-T2

This guide outlines the steps to build and run a Docker application using the provided Ansible playbook. The playbook is designed to run on an Ubuntu virtual machine (VM).

## Prerequisites
1. An Ubuntu virtual machine (VM) where the Docker application will be deployed.
2. Ansible installed on the host machine from which you'll execute the playbook.
3. Internet connectivity on the Ubuntu VM.

## Instructions
1. Copy the playbook content to a file named deploy.yml. along with inventory.ini

2. Modify the hosts field in the playbook to specify the target Ubuntu VM where you want to deploy the Docker application. For example: In my case i have used ubuntu_vm.
3. Execute the playbook using  command: $ ansible-playbook -i inventory.ini deploy.yml --ask-become-pass
4. You can now access the running Docker application by opening a web browser and navigating to http://<virtual_machine_ip>:9000/site/index.html

