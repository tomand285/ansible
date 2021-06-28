# ansible

The master repo of all of my Ansible playbooks.

# CREATE SSH KEY

`ssh=keygen -t ed25519 -C "<My comment>"`

# SETUP

To add the ssh key to the remote server, do the following command

`ssh-copy-id -i ~/.ssh/id_ed25519.pub <server ip>`

# TO RUN

`ansible-playbook -u root --private-key ~/.ssh/id_ed25519 bootstrap.yml`
`ansible-playbook <playbook.yml>`
