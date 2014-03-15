arpp
-------------------------------------------

Project status: In Progress

This project is supposed to be a very simple raspberry pi remote provisioning configuration. If you have to manage more than 1 raspberry pi or provision more than one, this might be for you.


## Why

I have been tasked with provisioning and maintaining 8 raspberry pis that simply host dashboards on a wall. This service will help jump start this process.

## How

These playbooks require Ansible 1.2.

Configure hosts in hosts file

```yml
    [pis]
    pi01
    pi02
    pi03
```

Add ssh key to `roles/common/templates/authorized_keys.j2`

Run

```bash
    ansible-playbook -i hosts site.yml
```
