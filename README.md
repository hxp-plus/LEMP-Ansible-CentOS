# ansible-example

# Deploy Server with php h5ai cockpit and nginx with https Automatically

## Requirements

- CentOS 8.x
- Latest Ansible installed

Edit `hosts` and variables in `group_vars/webservers`

in `hosts`

Change the ip to your server ip

in `group_vars`

Change `domain_name` to your server's domain name

Change `cockpit_username` and `cockpit_pwd`

Then, fire:

```
ansible-playbook site.yml -i hosts
```
