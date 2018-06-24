# graylog-ansible
Ansible playbooks for Graylog server setup and configuration.
If you are not familiar with Ansible and just want to quickly deploy 
a Graylog node, see the instructions below.

## Playbooks:
### graylog_install
Simple playbook that follows the basic installation guide for Graylog running on Ubuntu (http://docs.graylog.org/en/2.4/pages/installation/os/ubuntu.html).
- Installs  Prequisites;
- Installs MongoDB, Elasticsearch and Graylog and configures their services;
- Generates password secret;
- Hashes the password you choose and generates a password secret;
- Sets your chosen IP or the default system IP in the Web and API URI's;
- Optionally changes memory commited to Graylog and Elasticsearch processes.


### graylog_install_advanced
Todo. Advanced script for configuring a fully functional Graylog node (including cluster setup, smtp configuration, etc.).

## Instructions for running a playbook locally on Ubuntu:
This installs and runs Ansible from a virtual environment:

1. sudo apt-get update
2. sudo apt-get install python2.7 python-pip
3. sudo pip2 install virtualenv
4. cd /path/where/playbooks/are
5. python2 -m virtualenv .venv
6. source .venv/bin/activate
7. sudo pip install ansible
8. ansible-play -i hosts playbook_name
9. rm -rf /path/where/playbooks/are (if you don't need Ansible after this)
