# Introduction

This is a Ansible playbook for create a Mongodb replicaset on Ubuntu 18.

## Configuration

*hosts*:

```
[mongo_servers]
ubuntu-node-01
ubuntu-node-02

[mongo_main_server]
ubuntu-node-01

[mongo_secondaries_servers]
ubuntu-node-02
```

## Execute

Inside of playbook path, execute: 

```
# ansible-playbook -i hosts site.yml --ask-become-pass -k
```

This above command ask for password. If you don't need password, remove -k parameter.


