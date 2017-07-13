Role Name
=========

Role to deploy a mariadb cluster in docker in Centos/RHEL 7

Requirements
------------

Needs docker,docker-py installed in the hosts

Role Variables
--------------

image_name: "mariadb:10.3"
mysql_root_pass: "mysqlr00tp4ss"
mariadb_data_dir: /var/lib/mysql
docker_api_version: 1.22
users:
  - name: username
    pass: pass
databases:
  - test_db

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        -  role: ansible-mariadb-docker
           users:
             - user: test_user
               pass: test_pass
           databases:
             - test_database

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
