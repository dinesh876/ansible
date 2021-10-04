## Standalone Tomcat Deployment

- Requires Ansible 1.2 or newer
- Expects CentOS/RHEL 7.x hosts

These playbooks deploy a very basic implementation of Tomcat Application Server,
version 9. To use them, first edit the `hosts` inventory file to contain the
hostnames of the machines on which you want Tomcat deployed, and edit the 
roles/defaults/main.yaml  file to set any Tomcat configuration parameters you need.

Then run the playbook, like this:

	ansible-playbook --ask-become-pass tomcat9_playbook.yaml

When the playbook run completes, you should be able to see the Tomcat
Application Server running on the ports you chose, on the target machines.
