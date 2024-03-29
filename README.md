### Ansible Role to Install LAMP Stack on Amazon Linux 2

This role can be used to install a fully featured LAMP stack on Amazon Linux. Tihs can be used to deply a full WordPress installation or any CMS/Application that works over a LAMP stack.

---
#### Features
  - Fully confgurable and compatible with AWS
  - Flexible and feature rich with easy customization of roles
  - Can be modified to support additional modules
  - Can be used to create a standalone LAMP stack or deploy applications over the current LAMP stack

#### For Customization
> Edit roles/default/main.yml 
- mysql_rooti_password: This variable defines the root password ofthe MySQL database
- wordpress_user: This variable defines the additional database user 
- wordpress_password: This variable defines the additional MySQL database password
- wordpress_database: This variable defines the additional MySQL database name
> Additional user will have full privilege on the mysql_database 

#### How to change DB settings

```sh
$ cat var/main.yml
---
mysql_root_password: mysqlroot123
wordpress_user: mysqluser123
wordpress_password: mysqlpassword
wordpress_database: mysqldb
domain: www.example.com
```
