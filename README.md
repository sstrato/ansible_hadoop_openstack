Ansible Playbooks to construct HDFS/YARN Cluster
==================================================

Prepare Machines for deployment 

$ cp group_vars/openstack_instances.example group_vars/openstack_instances  <br />
$ vi group_vars/openstack_instances # and edit with your openstack credentials  <br />
$ vi ./openstack_hosts # change hostname, flavor and other things  <br />
$ ansible-playbook -i nova.py site.yml  <br />

if you changed hostname edit those files 
$ vi ./hosts # change hostname <br />
$ vi ./roles/common/files/hosts.default  # change hostname and ip <br />


Actual Cluster setup 
documents: http://dobachi.github.io/ansible-hadoop/

.. vim: ft=rst tw=0
