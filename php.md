# PHP installation
* Tambahkan repositories php
``````
sudo add-apt-repository ppa:ondrej/php
``````
* Update Apt nya
``````
sudo apt update
``````
* install php 7.4
``````
sudo apt install php7.4
``````
* INstall extensionnya, ikuti semua sudah tercover
``````
sudo apt install php7.4-{cli,common,gd,xmlrpc,fpm,curl,intl,imagick,mysql,zip,xml,mbstring,bcmath,json}
``````
* cek versi php nya
``````
php -v
``````
