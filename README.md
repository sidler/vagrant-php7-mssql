# vagrant-php7-mssql
Vagrant Box with php7 and MS SQL php drivers

The box is based on
* Centos 7
* PHP 7
* MSSQL Drivers / sqlsrv drivers

The box fires up the apache httpd server with following port mapping:
* 80 -> 8080
* 443 -> 8443

Make sure to adopt the mapped filesystem dir according to your needs:

    config.vm.synced_folder "./../", "/var/www/html"
  
  
The box requires the vbguest plugin to be available:

    vagrant plugin install vagrant-vbguest
