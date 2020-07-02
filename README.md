# ansible-example

# Deploy Server with php h5ai cockpit and nginx with https Automatically

## Requirements

- CentOS 8.x
- Latest Ansible installed

# with_ssl version

include
- nginx
- acme.sh
- cockpit
- php
- h5ai

will install the stuffs above and issue cert according to your domain with acme.sh, install cert to nginx automatically, and configure cockpit reverse proxy.

Visit <https://yourdomain.com/panel/> to enter cockpit panel, a user admin with password admin will be created without root access. You may change it in `group_vars/webservers`

Edit `hosts` and variables in `group_vars/webservers`

in `hosts`

Change the ip to your server ip

in `group_vars/webservers`

Change `domain_name` to your server's domain name.

Change `cockpit_username` and `cockpit_pwd`

Then, fire:

```
cd with_ssl
ansible-playbook site.yml -i hosts
```

# without_ssl

include
- nginx
- cockpit
- php

will install the stuffs above and configure cockpit reverse proxy.

Visit <https://yourip/panel/> to enter cockpit panel, a user admin with password admin will be created without root access. You may change it in `group_vars/webservers`

Edit `hosts` and variables in `group_vars/webservers`

in `hosts`

Change the ip to your server ip

in `group_vars/webservers`

Change `domain_name` to your server's ip.

Change `cockpit_username` and `cockpit_pwd`

Then, fire:

```
cd without_ssl
ansible-playbook site.yml -i hosts
```

