# wordpress-centos-7
<h1> Ansible - WordPress Role </h1>

This playbook has the funcion of installing Wordpress and Mariadb.

<h2> Tested ON: </h2>

<li>Centos 7.9</li>

<h2>variable file: </h2>
"defaults/main.yml"

<li>Before executing it is necessary to change!!</li>

<p>dest_wordpress: /var/www/html</br>

mysql_root_password: d@t@b@s@3sql</br>

mysql_db: wordpressdb</br>

mysql_user_wordpress: wordpress_user</br>

mysql_user_password_wordpress: wordpresspassword</p>


<h2>Example - Install the role:</h2>

ansible-galaxy install erickveiga02.wordpress_centos7

<h2>Playbook.yml example:</h2>

---
- hosts: wordpress
  roles:
    - role: erickveiga02.wordpress_centos7
