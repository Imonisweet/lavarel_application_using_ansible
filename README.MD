### Ansible Role to setup php,composer and laravel application

This code is tested on DO ubuntu machine.

# Requirements
  - Anisble Server - Droplets on Ubuntu server (Ansible should be installed)
  - Laravel Server -  Ubuntu Instance
  - All variables are declared under `group_vars/all.yaml`

# Prerequistie
  - Update inventory file `inventories/dev/hosts`
  - Generate the public key for the user ubuntu `ssh-keygen` on Ansible Server
  - Copy the `id_rsa.pub` from `cd ~./ssh` and paste it on the Laravel Server `vi ~/.ssh/authorized_keys` or you can use the priavte key and run this playbook which will automatically copy the public key on the target hosts

# Using Private Key Directly

- Copy the private key on the ansible server

```
# How to Run with private key
```
cd Ansible-playbook
ansible-playbook main.yml -i inventories/dev/hosts 

```

# 

# Access the application

Make sure security group of DO laravel Server is open for port 80.

```
http://imonisweet.me

```
