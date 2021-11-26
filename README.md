# Ansible ELK Playbook
 
This playbook is for setting up version 7.x of the ELK Stack on a remote server. 

## Notes and requirements

 - The playbook was built and tested on Ubuntu 20.04 VMs (Vagrant) 
 - You will need Ansible installed and running
  
 ## Instructions
 
 1. In the terminal on the machine hosting Ansible, clone this repo.
 2. `cd <directory>`
 3. `vagrant up`
 4. `ansible-playbook site.yml`
 
 The plays in the playbook will run on the target server, installing ELK 

You can now configure your `/etc/hosts` 

```shell
192.168.11.26 kibana.local
``` 

and open it with your browser `http://kibana.local`


**Disclaimer:**

This is heavyly inspired from: 
https://github.com/DanielBerman/ansible-elk-playbook/blob/master/site.yml and
https://www.digitalocean.com/community/tutorials/how-to-install-elasticsearch-logstash-and-kibana-elastic-stack-on-ubuntu-20-04
