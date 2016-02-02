Ansible SINOPIA NPM SERVER Ubuntu/Debian
========================================
This playbook installs a NPM repository using sinopia (https://github.com/rlidwka/sinopia).
Versions of the applications used could be modified but they're not tested!
Tested versions are:
    . debian: 7.8
    . node: 0.10.33
    . nginx: 1.8.0
    . sinopia: 1.4.0

## Prerequisites
### Install Ansible (tested with 1.9.4 and in Ubuntu)
```sh
$ sudo apt-get update && sudo apt-get install python-software-properties
$ sudo apt-add-repository -y ppa:ansible/ansible
$ sudo apt-get update
$ sudo apt-get install ansible
```
In other OS use the guide from http://docs.ansible.com/ansible/intro_installation.html

### Get Ansible Configuration
```sh
$ git clone THIS_PROJECT
```

### Use your own host info
```sh
$ vi hosts
```

## Launch ansible script
```sh
$ ansible-playbook -i hosts main.yaml
```

## Appendix
### Install sshpass (for --askpass option in ansible)
```sh
$ sudo apt-get install sshpass
```
