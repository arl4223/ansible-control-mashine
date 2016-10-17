# Ansible Control Mashine
This playbook will install the latest stable ansible version onto a debian mashine.

## Requirements
The following requirements need to be fullfilled.

  * Debian Jessie 64bit on target system
  * sudo must be installed
  * user needs to be in the sudo group
  * user must not need a password for using sudo

## How-To
  1. define your target mashine in inventory/hosts
  2. run 
		
		ansible-playbook -i inventory/hosts playbook.yml

  3. the first run will take a lot of time due long tasks like git checkout etc.
