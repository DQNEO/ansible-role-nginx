# NAME

Ansible Role of Nginx

# USAGE

in your playbook, define like below:

```
- hosts: all
  become: yes
  become_user: root
  vars:
    nginx_user: "nginx"
    nginx_worker_proccesses: "1"
    nginx_worker_connections: "1024"
    nginx_sendfile: "on"
    nginx_port: "80"
    nginx_server_name: "localhost"
    nginx_root: "/usr/share/nginx/html"
  roles:
    - nginx
```
