# Playground: For practicing ansible
## Attention:
``
This repository was created to help you experiment with Ansible by skipping the downloading and configuration of a local virtual machine. It provides a pre-configured application running in containers. 
``

If you're part of the **42 network**, this repository follows the same requirements as the **Cloud-1** project.

## Requirement :
```
install vagrant
install virtualbox
install ansible
```
Useful links for installing the required software from official websites. :
[vagrant ](https://developer.hashicorp.com/vagrant/downloads) <=> [virtualbox](https://www.virtualbox.org/wiki/Downloads) <=> [ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

## Clone Repository
```
git clone https://github.com/imaddine1/virtualBox-automated.git && cd virtualBox-automated
```
## Run vagrant 
```
vagrant up
```
![](https://github.com/imaddine1/virtualBox-automated/blob/main/imgs/vagrantfile.png)


This is my Vagrantfile, and you can modify it as needed. However, be cautious: if you change the `private IP address 192.168.56.10`, make sure to update it [here](https://github.com/imaddine1/virtualBox-automated/blob/main/setup/files/wordpress/tools/create.sh)

I used Vagrant for its flexibility in quickly setting up Linux distributions. HashiCorp, the provider of Vagrant boxes (images), offers lightweight images that are easy to install. Additionally, you can create multiple VMs with different Linux distributions
