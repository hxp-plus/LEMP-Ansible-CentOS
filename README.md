# ansible-example

# nginx_ssl_php_cockpit_h5ai

Deploy the latest nginx and use acme.sh to issue cert, and toggling ssl for nginx.

Change `hosts` and variable `domain_name` in `group_vars` to your server ip and domain name.

```
cd nginx_ssl_php_cockpit_h5ai
ansible-playbook site.yml -i hosts
```
