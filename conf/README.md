Ansible Repository for Session DB Evaluator
===========================================

This repository contains the ansible Playbooks for the Session DB Evaluator. Everything is configured to run with Ubuntu 16.04 LTS.

Setup
-----

###Every Host

Ensure that every host has Python installed since it is a requirement to let that host be configured by ansible

```bash
sudo apt install python -y
```

###Management Host / Config Server

Install ansible on the config server and link the hosts file.

```bash
sudo apt install ansible -y
#rm /etc/ansible/hosts #remove the old ansible hosts file if needed
sudo ln -s $FULL_PATH_TO_HOST_FILE /etc/ansible/hosts
```

Execute
-------

To configure the hosts just execute the following:

```bash
ansible-playbook site.yml
```

