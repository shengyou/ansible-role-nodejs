
Install nodejs
=========

install nodejs.

* Ubuntu 14.04, 16.04
* CentOS 6, 7

Requirements
------------

* ansible >= 2.4
* python >= 2.6

Role Variables
--------------

* nodejs_version (Default: 7)
* install_packages


Dependencies
------------

none.

Example Playbook
----------------

```
- name: install_nodejs.yml
  hosts: myhost
  gather_facts: yes
  become: yes

  vars:
    nodejs_version: 6
    install_packages:
      - gulp
      - bower
      - laravel-echo-server

  roles:
    - install_nodejs

```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
