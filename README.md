arpp
-------------------------------------------

This project is supposed to be a very simple raspberry pi remote provisioning configuration. If you have to manage more than 1 raspberry pi or provision more than one, this might be for you.


## Why

I have been tasked with provisioning and maintaining 8 raspberry pis that simply host dashboards on a wall. This service will help jump start this process.

## How

These playbooks require Ansible 1.2.

Configure hosts in hosts file

        [webservers]
        localhost

        [dbservers]
        bensible

Run

        ansible-playbook -i hosts site.yml
