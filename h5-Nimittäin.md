# H5 Nimittäin

## x)Tiivistelmä

Sivulla on kerrottu miten voidaan asentaa Apache web-palvelin ja luoda kotisivut yksikertaiseen Url-osoitteeseen kuten http://example.com

* Apachen lataus: sudo apt-get -y install apache2
* Virtualhostin luominen: sudoedit /etc/apache2/sites-available/tero.conf
* Kytke pois oletus ja kytke päälle oma virtualhost: sudo a2ensite tero.conf ja sudo a2dissite 000-default.conf ja lopuksi käynnistä uudelleen sudo service apache2 restart
* Tee oma kotisivu: mkdir public_html/, cd public_html/

https://terokarvinen.com/2016/02/16/new-default-website-with-apache2-show-your-homepage-at-top-of-example-com-no-tilde/

Sivulla on kerrottu miten voidaa hostata monta web-palvelua yhtellä ip-osoitteella.

* Lisätään uusi virtuaalipalvelin ja käynnistetään se uudelleen: ![image](https://github.com/bgx088/linux-kurssi/assets/143337810/fdc557d6-ef60-45ea-ab56-ea3fb3c88d3d)
* luodaan sivusto ja testataan:
*  mkdir -p /home/xubuntu/publicsites/pyora.example.com/
*  echo pyora > /home/xubuntu/publicsites/pyora.example.com/index.html
*  curl -H 'Host: pyora.example.com' localhost
*  curl localhost

 https://terokarvinen.com/2018/04/10/name-based-virtual-hosts-on-apache-multiple-websites-to-single-ip-address/

## a) Vuokraa domain-nimi

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/fb34e2aa-05b6-4f62-b365-748aa54819fd)

