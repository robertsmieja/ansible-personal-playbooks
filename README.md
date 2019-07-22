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

## Linting

### Pre-requisites
 * A VirtualEnv

```
pip install -r requirements.txt
ansible-lint **/*.yml
```

## Running a playbook inside a container
```
docker run --rm -it -v "$(pwd):/ansible-personal-playbooks"  --workdir "/ansible-personal-playbooks" --workdir "/ansible-personal-playbooks" --name ansible quay.io/robertsmieja/ansible-fedora-30 bash
ansible-playbook **/*.yml # Replace with specific playbook
```
