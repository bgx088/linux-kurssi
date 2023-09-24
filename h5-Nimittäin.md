# H5 Nimittäin

## x)Tiivistelmä

Sivulla on kerrottu miten voidaan asentaa Apache web-palvelin ja luoda kotisivut yksikertaiseen Url-osoitteeseen kuten http://example.com

* Apachen lataus: sudo apt-get -y install apache2
* Virtualhostin luominen: sudoedit /etc/apache2/sites-available/tero.conf
* Kytke pois oletus ja kytke päälle oma virtualhost: sudo a2ensite tero.conf ja sudo a2dissite 000-default.conf ja lopuksi käynnistä uudelleen sudo service apache2 restart
* Tee oma kotisivu: mkdir public_html/, cd public_html/

https://terokarvinen.com/2016/02/16/new-default-website-with-apache2-show-your-homepage-at-top-of-example-com-no-tilde/

Sivulla on kerrottu miten voidaa hostata monta web-palvelua yhtellä ip-osoitteella.

* Lisätään uusi virtuaalipalvelin ja käynnistetään se uudelleen: $ sudoedit /etc/apache2/sites-available/pyora.example.com.conf
$ cat /etc/apache2/sites-available/pyora.example.com.conf
<VirtualHost *:80>
 ServerName pyora.example.com
 ServerAlias www.pyora.example.com
 DocumentRoot /home/xubuntu/publicsites/pyora.example.com
 <Directory /home/xubuntu/publicsites/pyora.example.com>
   Require all granted
 </Directory>
</VirtualHost>
$ sudo a2ensite pyora.example.com
$ sudo systemctl restart apache2
* 
