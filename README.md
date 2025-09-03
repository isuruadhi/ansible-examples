# ansible-examples

This repo is a beginner’s guide to Ansible, showing how to use it for automation with simple examples.

Ansible is an open-source IT automation tool used to configure systems, deploy applications, and manage infrastructure — all without needing an agent installed on managed hosts.

## Why Ansible?
- Agentless  →   No need to install software on managed nodes  
- Simple     →   Playbooks written in human-readable YAML  
- Powerful   →   Manage servers, switches, firewalls, containers, and cloud infra  
- Scalable   →   Works for 1 host or 1000+  
<br>

## Repository Structure

<image>

<br>

## What are these files?

`ansible.cfg`
- Tells Ansible how to behave.
- Defines default inventory file, remote user, and other options.
<br>

`inventory.ini`
- A list of hosts (servers, switches, firewalls, etc.) Ansible manages.
<br>

`playbooks (*.yml)`
- Main logic of automation (written in YAML).
- Define tasks to run on hosts.
<br>

## Running Ansible
1. **Test Connection**
Ping all hosts in your inventory:
```bash
ansible all -m ping -i inventory.ini
```
<br>

2. **Run a Playbook**
Execute a playbook on your inventory:
```bash
ansible-playbook playbooks/example.yml -i inventory.ini
```
<br>

3. **Run with Custom Config**
If your `ansible.cfg` is in the repo, Ansible will auto-detect it.
Otherwise, specify manually:
```bash
ANSIBLE_CONFIG=./ansible.cfg ansible-playbook playbooks/example.yml
```
<br>

##  Learn More
- [Installing Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
- [Ansible Documentation](https://docs.ansible.com/)
- [Ansible Galaxy (modules & roles)](https://galaxy.ansible.com/)
<br>

## 🤝 Contributing
Feel free to fork this repo, improve the examples, and create pull requests.  

