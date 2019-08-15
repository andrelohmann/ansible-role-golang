golang
======

[![Build Status](https://travis-ci.org/andrelohmann/ansible-role-golang.svg?branch=master)](https://travis-ci.org/andrelohmann/ansible-role-golang)

Use this role to install the gophers golang repository on your ubuntu server.

Requirements
------------

This role requires ubuntu.

Role Variables
--------------

The default set of variables defines the golang installation and needs at best to be overwritten in group_vars/host_vars

    golang_version: '1.12'
    golang_gopath: go
    golang_additional_libraries:
    - golang.org/x/tools/cmd/goimports
    golang_users:
    - root

Example Playbook
----------------

    - hosts: golang
      roles:
         - andrelohmann.golang

License
-------

MIT

Author Information
------------------

https://github.com/andrelohmann
