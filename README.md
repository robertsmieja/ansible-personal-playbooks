# Ansible Personal Playbooks
 Collection of Ansible Playbooks to bootstrap machines
 Written for Fedora

## Pre-requisites
 * Ansible: `sudo dnf install ansible -y`

## Usage
 1. Clone Git repo: `git clone https://github.com/robertsmieja/ansible-personal-playbooks/`
 2. Run playbooks:
 ```
 cd ansible-personal-playbooks
 ansible-playbook python/fedora.yml
 ansible-playbook vscode/fedora.yml
 ```
