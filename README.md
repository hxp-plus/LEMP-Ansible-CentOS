# ansible-example

# nginx

Deploy the latest nginx and use acme.sh to issue cert, and toggling ssl for nginx.

Change `hosts` and variable `domain_name` in `nginx.yml` to your server ip and domain name.

```
cd nginx
ansible-playbook site.yml -i hosts
```
