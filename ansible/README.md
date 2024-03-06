# Ansible Project: DEPLOYING JOGET


## Description

This project is a playbook that installs JOGET on dev and prod environments.


## Requirements

List any prerequisites or requirements for using your Ansible project:

- Ansible (version 2.15.2)
- Python (version 3.11.5)

## Project Structure
```bash
├── Templates            # Stores Jinja2 templates for configuration.
│ ├── docker-compose.j2
│
└── Vars         # Holds variable files, like secrets, for Ansible playbooks.
|  └── envs.yaml
└─ playbook.yaml # Holds all the tasks to be run on host machines

```

## Install
```
sudo ansible-playbook playbook.yaml --tags start-joget

```
