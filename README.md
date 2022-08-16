Role Name
=========

Simple installation [lighthouse from github repository](https://github.com/VKCOM/lighthouse)

Requirements
------------
EL7 OS
Nginx

Role Variables
--------------
``` yaml
#lighthouse repository url
lighthouse_git: https://github.com/VKCOM/lighthouse
#directory for installing lighthouse
lh_home_dir: "/opt/lighthouse"
#access log name
lh_alog_name: lighthouse_access
#default nginx user
nginx_user: root
```

Dependencies
------------
(optionally)
nginx-role:

git@github.com:mrbobr/nginx-role.git
version: "1.0.0"

Example Playbook
----------------

    - name: Install Lighthouse
      hosts: lighthouse servers
      roles:
        - lighthouse-role

License
-------
MIT
