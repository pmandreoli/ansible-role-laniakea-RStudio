Role Name
=========

Role to install rstudio-server on a Centos7 Virtual Machine and create a new user.
tested using ansible 2.3 on CentOS7.

Requirements
------------
ansible > 2.3

Role Variables
--------------

``username:`` rstudio user username (default: ``studio``) 

``install_Seu:`` bool, if true install R Seurat package (default: ``false``)

``rstudio_port:`` port to expose rstudio on http: (default:``8080``)

``R_VERSION:`` version of R to install (default: ``4.0.0``)

``role_debug:`` debug (default: ``false``)

Dependencies
------------
ansible version 2.3

Example Playbook
----------------
testing playbook ``test.yml`` present under test directory.

command:

``ansible-playbook test.yml -e ansible_python_interpreter=/usr/bin/python`` 

```
---
- name: Deploy seurat-rstudio-server
  hosts: localhost
  become: yes
  vars:
    - username: user4
  roles:
    - role: ansible-role-laniakea-RStudio 

```

License
-------

BSD

Author Information
------------------

Pietro Mandreoli
email: pietro.mandreoli@unimi.it 

