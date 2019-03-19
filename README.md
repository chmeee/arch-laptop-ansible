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

## Run

Run the `main.yml` playbook to configure your laptop.
