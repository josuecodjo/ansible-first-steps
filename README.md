# Ansible first Steps

## On the controller node

- `ssh-keygen -t rsa -b 4096`
- Copy the public key and paste it to authorized_keys on web01 and web02
- `sudo apt update && sudo apt install python3 python3-pip python3-venv`
- `python3 -m venv .venv`
- `source .venv/bin/activate`
- `pip3 install ansible`
- `ansible --version`
- Cloner le repository
- `cd ansible-first-steps`
- `ansible all -i inventory/hosts -m ping`
- `ansible-playbook -i inventory/hosts playbooks/os-update.yml`
- `ansible-playbook -i inventory/hosts playbooks/ufw.yml`