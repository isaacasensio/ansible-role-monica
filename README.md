Monica 
=========

Monica helps you organize the social interactions with your loved ones.

This Ansible role installs Monica as a Docker service.

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

```
monica_image: "monica"
```
The version of the docker image to run as a container.
```
monica_db_image: "mysql:5.7"
```
Database docker image version
```
monica_db_user: "monica"
```
Database user
```
monica_db_password: "monica"
```
Database password
```
monica_db_name: "monica"
```
Database name
```
monica_host_config_path: /etc/monica
```
Monica configuration folder in the host machine
```
monica_host_db_path: /var/lib/monica/mysql
```
Monica database folder in the host machine
```
monica_container_user: monica
```
Monica container username
```
monica_host_port: 24560
```
Monica host port

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - iasensio.monica

License
-------

MIT

