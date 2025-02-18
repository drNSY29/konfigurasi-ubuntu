# konfigurasi-webserver ubuntu
Web service

    Install apache2

apt install apache2 -y

    View status service

systemctl status apache2

    Enable and start apache2

systemctl enable apache2 --now

    Go to configuration service

cd /etc/apache2

    Edit file configuration default apache2

vim sites-available/000-default.conf

    Edit configuration like below

    Edit konten website with echo

echo "<h1><center>Belajar Web Service Bersama Kelompok 17</center></h1>" > /var/www/html/index.html

    Reload configuration apache2

systemctl reload apache2

