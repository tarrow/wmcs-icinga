This provides a quick way to configure a server to act as an icinga master 

## Prerequisites

This uses [ansible](https://docs.ansible.com/ansible/latest/index.html) to manipulate remote servers via SSH - essentially automating what you'd otherwise do "by hand" in a step-by-step approach.
You need to be in possession of an SSH private key for which there is a associated user that is authorized to perform the operations.

## Config
### Mattermost
Set users, channels, and webhook URLs in infrastructure/files/conf.d/users.conf

## Run (from your local machine)

```sh
# assuming your shell is inside this folder (infrastructure)
ansible-playbook -b -i servers.ini master.yml
```
