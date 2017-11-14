# Install-Docker
Installs Docker using ansible playbooks. 

Create a host file in the project folder i.e. outside of the roles folder. Specify the ip address under the groups name 'docker'and the ansible_ssh_user (and private key path if key not added). Make the following enteries like below

[docker]
ip_address ansible_ssh_user=ec2-user

To run the playbook type the following command
ansible-playbook -i hosts docker-runner.yml 

Supported OS and tried on: 
- RHEL 7.3
- RHEL 7.4
- Ubuntu 16.04



