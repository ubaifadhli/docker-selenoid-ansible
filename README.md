# Ansible scripts to install Docker and Selenoid

## Prerequisites
- Ansible installed on your host machine
- SSH key of your remote machine

## Usage Guide
1. Clone the repo
2. Put the remote machine's SSH key into the repo folder
3. Change `private_key_file` value in `ansible.cfg` according to your SSH key's filename
4. Change `remote_user` value in `ansible.cfg` according to your remote machine's username
5. Run `ansible-playbook install_docker.yml` to install Docker
6. Run `ansible-playbook install_selenoid.yml -K` to install Selenoid
> `-K` parameter is used to let you provide your remote machine's user password
