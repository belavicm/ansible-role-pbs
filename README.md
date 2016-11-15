[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Build Status](https://travis-ci.org/grycap/ansible-role-torque.svg?branch=master)](https://travis-ci.org/grycap/ansible-role-torque)

SLURM cluster Role
=======================

Install [Torque cluster](http://www.adaptivecomputing.com/products/open-source/torque).  
Role to be used with [EC3](http://servproject.i3m.upv.es/ec3/).

Role Variables
--------------

The variables that can be passed to this role and a brief description about them are as follows.
```
  # Type of node to install: front or wn
  torque_type_of_node: front
```

Example Playbook
----------------

This an example of how to install a Torque cluster:
```
  - roles:
  - { role: 'grycap.torque', torque_type_of_node: 'front' }
```
```
  - roles:
  - { role: 'grycap.slurm', slurm_type_of_node: 'wn' }
```
Contributing to the role
========================
In order to keep the code clean, pushing changes to the master branch has been disabled. If you want to contribute, you have to create a branch, upload your changes and then create a pull request.  
Thanks
