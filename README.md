wordpress-xavki
=========

This role install wordpress on Debian stretch with all LAMP packages needed.

Requirements
------------

Need Debian Stretch

Role Variables
--------------

# default package LAMP for wordpress

lamp_packages:
    - apache2
    - mysql-server
    - php7.0-common
    - php7.0-mysql
    - libapache2-mod-php7.0
    - python-mysqldb
    - wget


# default variables for mysql

mysql_db: "blog"
mysql_user: "user1"
mysql_password: "toto"


# default wordpress source

wordpress_source: "https://wordpress.org/latest.tar.gz


Example Playbook
----------------

- name: "[TEMPLATE]"
  hosts: all

  roles:
    - wordpress-xavki


License
-------

BSD

Author Information
------------------

Xavki is owner of https://xavki.blog and you can see his channel on youtube.

