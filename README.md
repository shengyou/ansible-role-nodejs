
Install nodejs [![Build Status](https://travis-ci.org/shengyou/ansible-role-nodejs.svg?branch=master)](https://travis-ci.org/shengyou/ansible-role-nodejs)
=========

install nodejs. (5, 6, 7, 8)

* Ubuntu 14.04, 16.04
* CentOS 6, 7

Requirements
------------

* ansible >= 2.4
* python >= 2.6

Role Variables
--------------

* nodejs_version (Default: 8)
* install_packages (非必填，如希望一併 global install nodejs package 才須設置。)

使用方式請參考範例。

Dependencies
------------

none.

Example Playbook
----------------

```
- name: ansibel-role-nodejs.yml
  hosts: your_host
  gather_facts: yes
  become: yes

  vars:
    nodejs_version: 6
    install_packages:
      - gulp
      - bower
      - laravel-echo-server

  roles:
    - ansibel-role-nodejs

```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
