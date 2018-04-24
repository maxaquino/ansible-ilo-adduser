# ansible-ilo-adduser

## Overview

This solution uses Ansible to automate the creation of an ilo user through OneView

## Requirements
[Ansible Modules for HPE OneView](https://github.com/HewlettPackard/oneview-ansible)

## Setup
To run the ansible modules provided you should execute the following steps:

### 1. Clone the repository

Run:

```bash
$ git clone https://github.com/maxaquino/ansible-ilo-adduser
```

### 2. Create the configuration files:

Create a json file named **oneview_config.json** with the credentials as follow:
```
{
  "ip": "192.168.0.100",
  "credentials": {
    "userName": "Administrator",
    "password": "yourpassword"
  },
  "api_version": 300
}
```

## 3. Run the playbook
To run the playbook, just type the following command on your ansible machine:

```
ansible-playbook -i hosts ilo-add-user.yml
```


## ToDo

