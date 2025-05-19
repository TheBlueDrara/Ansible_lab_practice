# Ansible Script Distribution

## Overview
Dear tech priest, this repository contains the knowledge to distribute a shell script to all of your Class A titans and toasters.

You will find a playbook that distributes a script from the master host to all the slaves in the network.

## Prerequisites

- Before running the playbook, you need to run an Ansible Docker compose lab and clone the repository into the Ansible host container.

- You can find the lab [here](https://gitlab.com/vaiolabs-io/ansible-shallow-dive)

```
docker compose up -d
docker exec -it docker-ansible-host-1 /bin/bash
git clone https://github.com/TheBlueDrara/Ansible_lab_practice.git
```

## Running the Playbook

```
cd Ansible_lab_practice
ansible-playbook playbook.yaml
```

## Features

- Ignore the SSH error – added a config to ansible.cfg
- Check if the directory exists before distributing the script
- Escalate privileges if needed


Daily WarHammer Qoute
```
The burden of immortality is the price of duty.

  Venerable Brother Atheos, Ultramarines
```
