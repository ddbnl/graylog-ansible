# graylog-ansible
Ansible playbook(s) for Graylog server setup and configuration. Will be added to the Graylog marketplace after more testing and improved documentation/instructions.

## graylog_install
Simple script that follows the basic installation guide for Graylog running on Ubuntu (http://docs.graylog.org/en/2.4/pages/installation/os/ubuntu.html).
- Installs  Prequisites
- Installs MongoDB, Elasticsearch and Graylog and configures their services
- Generates password secret
- Hashes the password you choose and generates a password secret
- Sets your chosen IP or the default system IP in the Web and API URI's


## graylog_install_advanced
Todo. Advanced script for configuring a fully functional Graylog node (including cluster setup, smtp configuration, etc.).
