## Check_MK Raw Edition (Debian, Ubuntu, CentOS, RHEL)

version: 1.5.0p4

* installs or updates Check_MK Raw, creates and starts a site if doesn't exist
* usage example:
  1. wget https://raw.githubusercontent.com/jeremylarose/server_install_scripts/master/Check_MK_Raw.sh && chmod +x Check_MK_Raw.sh && ./Check_MK_Raw.sh -v '1.5.0p4' -s monitoring && rm -f Check_MK_Raw.sh


## MariaDB (*Debian, Ubuntu, CentOS, RHEL, Fedora)

version: 10.3

* Installs MariaDB and/or just creates a database if mariadb/mysql already installed
* usage example:
  1. wget https://raw.githubusercontent.com/jeremylarose/server_install_scripts/master/MariaDB.sh && chmod +x MariaDB.sh && ./MariaDB.sh -r password -d databasename -u dbusername -p dbpassword && rm -f MariaDB.sh

* * currently MariaDB's authentication key is having issues with Debian

## Gitea (Debian, Ubuntu, CentOS, RHEL, Fedora)

version: 1.5.1

* builds with PAM authentication capability (not available with developer binaries) and Installs with service (mysql) enabled
* usage example (install Gitea and MariaDB with two commands filling in your command line arguments):
  1. wget https://raw.githubusercontent.com/jeremylarose/server_install_scripts/master/MariaDB.sh && chmod +x MariaDB.sh && ./MariaDB.sh -r password -d databasename -u dbusername -p dbpassword && rm -f MariaDB.sh
  2. wget https://raw.githubusercontent.com/jeremylarose/server_install_scripts/master/Gitea.sh && chmod +x Gitea.sh && ./Gitea.sh && rm -f Gitea.sh

## Guacamole Apache (Debian, Ubuntu, CentOS, RHEL, Fedora)

version: 0.9.14

* Installs or upgrades Apache Guacamole, installs any extensions specified in command line, and also adds JDBC Drivers for mysql and postgresql if needed... afterward, would just need to modify guacamole.properties and install database schema
usage example (install Guacamole and MariaDB with two commands filling in your command line arguments):
wget https://raw.githubusercontent.com/jeremylarose/server_install_scripts/master/MariaDB.sh && chmod +x MariaDB.sh && ./MariaDB.sh -r password -d databasename -u dbusername -p dbpassword && rm -f MariaDB.sh
wget https://raw.githubusercontent.com/jeremylarose/server_install_scripts/master/Guacamole.sh && chmod +x Guacamole.sh && ./Guacamole.sh && rm -f Guacamole.sh


## OCS Inventory NG (Debian, Ubuntu, CentOS, RHEL)

version: 2.5

* install example (install OCS Inventory NG and MariaDB with two commands filling in your command line arguments):

  1. wget https://raw.githubusercontent.com/jeremylarose/server_install_scripts/master/MariaDB.sh && chmod +x MariaDB.sh && ./MariaDB.sh -r 'rootpassword' -d ocsweb -u ocs_dbuser -p 'dbpassword' && rm -f MariaDB.sh
  2. wget https://raw.githubusercontent.com/jeremylarose/server_install_scripts/master/OCSInventoryNG.sh && chmod +x OCSInventoryNG.sh && ./OCSInventoryNG.sh -u ocs_dbuser -p 'dpbassword' -v 2.5 -h localhost -p 3306 && rm -f OCSInventoryNG.sh
