# wordpress-centos-7
-------------

This playbook has the funcion of installing Wordpress and Mariadb.

Ansible-Galaxy:
------
- Link: https://galaxy.ansible.com/erickveiga02/wordpress_centos7
 Tested ON: 
--------
- Centos 7.9

variable file: 
--------
- "defaults/main.yml"

- Before executing it is necessary to change!!
```yaml
dest_wordpress: /var/www/html
mysql_root_password: d@t@b@s@3sql
mysql_db: wordpressdb
mysql_user_wordpress: wordpress_user
mysql_user_password_wordpress: wordpresspassword
```
Install the role:
-----

- ansible-galaxy install erickveiga02.wordpress_centos7

Playbook.yml example:
----
```yaml
---
- hosts: wordpress
  roles:
    - role: erickveiga02.wordpress_centos7
```
