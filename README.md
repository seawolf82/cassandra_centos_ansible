# cassandra_centos_ansible


This script install cassandra on Redhat based Distributions.

Tested on:

- Almalinux 8
- Almalinux 9
- RockyLinux 8
- RockyLinux 9
- Centos 7

Tested on:

- 2.14 Ansible version


To install cassandra on Redhat based Distributions run:

ansible-playbook -i hosts site.yaml

To uninstall cassandra on Redhat based Distributions run:

ansible-playbook -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade
package
cassandra
ntp

For example, to launch only task regarding upgrade os, run:
 
ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
