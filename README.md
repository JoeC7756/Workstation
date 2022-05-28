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
ansible-playbook main.yml (Subsequent time)
```

## Development

For development purposes a Virtual Machine (VM) can be used. 

Firstly ensure that Vagrant and VirtualBox are installed. Then to provision one using the provided Vagrantfile run `vagrant up`.

The default username and password are both `vagrant`. You should then take this VM through the default Arch linux installation. Once this is complete, run the playbook using the steps listed in getting started.

Once you have finished, destroy the VM using `vagrant halt`.