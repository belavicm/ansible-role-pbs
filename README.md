[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Build Status](https://travis-ci.org/grycap/ansible-role-torque.svg?branch=master)](https://travis-ci.org/grycap/ansible-role-torque)

Torque cluster Role
=======================

Install [Torque cluster](http://www.adaptivecomputing.com/products/open-source/torque).  
Role to be used with [EC3](http://servproject.i3m.upv.es/ec3/).

Role Variables
--------------

The variables that can be passed to this role and a brief description about them are as follows.
```
  # Type of node to install: front or wn
  torque_type_of_node: front
  # PBS server configuration
  pbs_server_conf: ""
  # Max number of nodes for the cluster
  number_of_nodes: 1
  # Script telling if the cluster finished the configuration
  is_cluster_ready_script: ""
  # Prefix applied to the cluster nodes
  vnode_prefix: "wn"

```

Example Playbook
----------------

This an example of how to install a Torque cluster:
```
  - roles:
    - { role: 'grycap.torque', torque_type_of_node: 'front' }
```
Contributing to the role
========================
In order to keep the code clean, pushing changes to the master branch has been disabled. If you want to contribute, you have to create a branch, upload your changes and then create a pull request.  
Thanks
