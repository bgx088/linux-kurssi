# H5 Nimittäin

## x)Tiivistelmä

Sivulla on kerrottu miten voidaan asentaa Apache web-palvelin ja luoda kotisivut yksikertaiseen Url-osoitteeseen kuten http://example.com

* Apachen lataus: sudo apt-get -y install apache2
* Virtualhostin luominen: sudoedit /etc/apache2/sites-available/tero.conf
* Kytke pois oletus ja kytke päälle oma virtualhost: sudo a2ensite tero.conf ja sudo a2dissite 000-default.conf ja lopuksi käynnistä uudelleen sudo service apache2 restart
* Tee oma kotisivu: mkdir public_html/, cd public_html/
