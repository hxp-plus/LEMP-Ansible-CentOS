# ansible-example

# nginx_ssl_php_cockpit

Deploy the latest nginx and use acme.sh to issue cert, and toggling ssl for nginx.

Change `hosts` and variable `domain_name` in `group_vars` to your server ip and domain name.

```
cd nginx_ssl_php_cockpit
ansible-playbook site.yml -i hosts
```
