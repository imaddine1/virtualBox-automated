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

## Run ansible
You can verify if Ansible is set up correctly by running ansible --version and ansible-playbook --version,  then run 
```
ansible-playbook -i inventory.ini playbook.yml 
```
## The Application is running now.
- access wordpress page by visiting http://192.168.56.110.
- access wordpress login page by visiting http://192.168.56.110/wp-admin => login as admin `user: supervisor ,  password: supervisor123` you can change these credentials in the `setup/files/.env` file 
- access your phpmyadmin interface by visiting http://192.168.56.110/phpmyadmin => login is `user: imad , password: imad123`

## Everything Should Be Up Now
It's your turn to experiment with Ansible by modifying the playbook.yml and setup/tasks/main.yml files. Learn what you need and apply it to this VM.

## What You Can Do Next
- Use other built-in Ansible modules.
- Work with Ansible variables (vars).
- Explore variable precedence by applying it here.
- Create your own collection to manage VMs on VirtualBox.
- Use additional folders generated by the Ansible role inside the setup folder
- Create another VM, modify the Vagrant configuration, and deploy your application in parallel
- Use groups of inventory

## What You Can Fix:
`After gaining some basic knowledge of Ansible, you might notice that idempotency is not working well in this playbook. As a challenge, can you fix it using the appropriate components ??`
  
