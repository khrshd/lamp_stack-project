# lamp_stack-project
This my ansible playbook to configure LAMP (linux-Apache_MySQL-PHP) stack on Ubuntu 20.04 (VM) written on Centos 7(VM).
Version of Ansible is 2.9, Apache 2.4 and PHP 7,3.

index.html is functional and has solutation content only.
MySQL database will be installed automatically but has to be finalized manually regarding the passwords due to ANsible idimpotency which may not work properly as that is only single time setup.

Installation of PHP was done to max possiblity but might have some extra work both, finishing up in terms of installation as well as further manual setup of MediaWiki part.
Issues with installation was mainly concerned regarding the ubuntu repo unavailability as the time of this writing with following error code:
"  Temporary failure resolving 'us.archive.ubuntu.com'", "Ign:7 http://security.ubuntu.com/ubuntu focal-updates/main amd64 apache2-data all 2.4.41-4ubuntu3.1"
This playbook was functional when tested with centos 7 with slight modifications.

The playbook was created based on DNS rather than purely using IP address.
