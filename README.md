Role Name
=========

Ansible role to install ansible on ansible control machine.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

ansible_version_wanted: what verion to installed, default is '1.9.4'
install_temp_folder: where to save download fild, default to '/var/tmp'

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

```
SYDC02PQ08NG8WN:garyjyao1 jyao1$ cat test-ansible-role-rm.yml
    - hosts: all
      sudo: yes
      roles:
        - { role: ansible-role-cm }
ansible-playbook -i vagranthost test-ansible-role-rm.yml -vvvv
```
License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
