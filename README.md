# Ansible first Steps

## On the controller node

- `ssh-keyben -t rsa -b 4096`
- Copy the public key and paste it to authorized_keys on web01 and web02
- `apt update && apt install python3 python3-pip`
- `pip3 install ansible`

- `ansible all -i inventory/hosts -m ping`
- `ansible-playbook -i inventory/hosts playbooks/os-update.yml`
- `ansible-playbook -i inventory/hosts playbooks/ufw.yml`