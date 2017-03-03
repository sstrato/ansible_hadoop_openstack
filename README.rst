Ansible Playbooks to construct HDFS/YARN Cluster
==================================================

Prepare Machines for deployment 

$ cp group_vars/openstack_instances.example group_vars/openstack_instances
$ vi group_vars/openstack_instances # and edit with your openstack credentials
$ vi ./openstack_hosts # change flavor and other things 
$ ansible-playbook -i nova.py site.yml

Actual Cluster setup 
documents: http://dobachi.github.io/ansible-hadoop/

vim: ft=rst tw=0
