# Laptop configuration in Ansible

## First steps

First install Archlinux base. Then:

  * `pacman -S sudo`
  * `useradd -m <your-username> -G wheel`
  * `pacman -S python`

If you want to perform the installation from another host, you'll need:

  * `pacman -S openssh`
  * `systemctl start sshd`
  * For convenience, copy your ssh public key to .ssh/authorized_keys

Otherwise, if you want to install from localhost, you'll need:

  * `pacman -S ansible`
  * Transfer this repository to your laptop

## Configuration

## Run playbook

Run the `main.yml` playbook to configure your laptop.

## Run scripts

There are some scripts to copy data, usually sensible, that are supposed to run once.

# TODO

Divide tasks in different files for different purposes
