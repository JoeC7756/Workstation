# Workstation
An ansible playbook to configure my personal workstation.

This playbook is intended for post configuration of an Arch linux system. To achieve the initial installation the system can be configured manually or a guided install, such as [archinstall](https://github.com/archlinux/archinstall), can be used.

## Getting started

Install the required packages
```
sudo pacman -S git ansible -y
```

Clone this repository and run the playbook
```
git clone https://github.com/JoeC7756/Workstation.git
cd Workstation/
ansible-playbook main.yml -K (First time)
ansible-playbook main.yml -K (Subsequent time)
```