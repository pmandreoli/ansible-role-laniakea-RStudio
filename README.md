Role Name
=========

Role to install rstudio-server  complete with Seurat packages on a Centos7 Virtual Machine

Requirements
------------
host need port 80 opened

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

---
- name: Deploy seurat-rstudio-server
  hosts: seurat-test
  become: yes
  roles:
    - { role: /path/to/role/rstudio-server-seurat }


License
-------

BSD

Author Information
------------------

Pietro Mandreoli
