## Automating API war backup

- Requires Ansible 1.2 or newer


These playbooks take the backup of war file to the destination,
version 9. To use them, first edit the `hosts` inventory file to contain the
hostnames of the machines on which you want take backup, and edit the 
roles/defaults/main.yaml  file to set  configuration parameters you need.

Then run the playbook, like this:

	ansible-playbook  backup_playbook.yaml