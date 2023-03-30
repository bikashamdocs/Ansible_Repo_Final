# Ansible Playbook: Install Nginx on Ubuntu Local Machine
This Ansible playbook installs and configures Nginx on an Ubuntu local machine.

# Project Structure

1. ansible.cfg: is the configuration file for Ansible. It contains settings such as the location of the inventory file and SSH options.
2. inventory/host.ini: is the inventory file that defines the hosts that Ansible will manage. It lists the IP addresses or domain names of the hosts and groups them into categories.
3. roles/: is a directory that contains all the roles for the Ansible project. In this project, there's only one role named nginx.
4. site.yml: is the main playbook that will be executed for the entire Ansible project. It includes the nginx role.


# Requirements
1. Ansible 2.10 or later
2. Ubuntu operating system (tested on Ubuntu 20.04)
3. Role Variables- You can modify these Role variables in the vars/main.yml file to customize the Nginx installation.

# Dependencies
NA

# Usage

1. Clone the repository to your local machine:

```bash
git clone https://github.com/bikashamdocs/Ansible_Repo_Final.git
```
2. Change directory to the cloned repository:

```bash
cd my-playbook
```

3. Modify the inventory file host.ini to specify the target host or group of hosts to install Nginx on.

4. Run the playbook to install Nginx:

```bash
ansible-playbook site.yml
```

# Testing
1. This role includes a tests directory with a sample inventory and test playbook. You can run the tests using the following command:

```bash
ansible-playbook tests/test.yml -i tests/inventory
```

# License

NA


# Author Information
This role was created by Bikash.
