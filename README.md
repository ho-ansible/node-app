# Ansible role: node-app
Node.js web app

## DEPRECATED
This functionality has been moved to kubernetes,
so this ansible role is no longer maintained.

## Requirements
Only tested on Debian buster.

## Role Variables
+ `node_name` (default: myapp): base filename for nginx config
+ `node_description` (default: "My Node.js app"): title 
+ `node_repo`: URL to git repo of node package
+ `node_hostname` (default: myapp.example.com): domain name for nginx listen
+ `node_listen` (default: ["443 ssl http2"]): list of nginx `listen` directives
+ `node_localport` (default: 8080): tcp port for nginx to listen on
+ `node_user` (default: node): user to run nodejs as
  
## Playbooks
+ `main.yml`: apply role

## Dependencies
+ [ho-ansible.nodejs](https://github.com/ho-ansible/nodejs)
+ [ho-ansible.nginx](https://github.com/ho-ansible/nginx)

## License
+ This ansible role is licensed [MIT](LICENSE).

## Author Information
+ This ansible role is by [Sean Ho](https://github.com/ho-ansible/)
