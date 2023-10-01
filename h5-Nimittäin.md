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

Domainin vuokrausta varten käytin namecheap.com sivustua ja käytin myös guthubin educational-pakettia ja sain tämän kautta ilmaisen .me päätteisen domanin nimen. Pienen kikkailun jälkeen sain kirjauduttua ja lunastettuun etuuden. 

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/fb34e2aa-05b6-4f62-b365-748aa54819fd)

Tilauksen jälkeen menin Domain list kohdasta "Adavanced DNS" välilehdelle ja sieltä laitoin "host records" kohtaan oman virtuaalipalvelimeni IP-osoitteen. Nyt sivusto löytyy osoitteesta www.alaninsivu.me

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/8ea49fc3-0998-419d-a73f-e7a10b38f833)

## b) Tutki oman nimesi tietoja

Ensimmäseksi yritin "host alaninsivu.me" komentoa, mutta minulla ei ollu sitä asennettu, joten asensinsin sen ja samalla myös dig komentoa varten dns utilities. "sudo apt-get install host" ja "sudo apt-get install dnsutils".

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/06e5b23f-3c08-4e75-8914-ba0f0522ded5)

Host komennon avulla saadaan tulostettua palvelimen IP-osoite. Lisäksi saadaan MX-records, jotka ovat jonkin tyyppisen sähköpostipalvelinten paketit. Alkuosassa nähdään kenen paketteje käsitellään ja lopussa näkyy ketkä niitä käsittelee.

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/79ef0da5-824c-4ff5-97ba-116cbcc21a55)

Komennolla "dig alaninsivu.me" saadaa hyvin sekavan näköinen lista tietoa. 
* Ihan ylhäällä on debianin versio ja syötetty osoite.
* Global option +cmd ei oikein selvinnyt, mutta voiko liittyä terminaaliin?
* Got answear = saatu vastaus
* Status ja sen id eli NOERROR meni läpi
* flags voisiko olla jonkin näköin hakemisto ja 0 ja 1 vastauksia?
* OPT on jonkin näköinen DNS lisätieto
* Saadut vastaukset
* Osoite
* Aika
* Vastauksen koko

## c) Etusivu uusiksi

muokkaa

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/0e8b6865-417d-4136-b002-7ec34327e759)

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/146c7669-e171-4b23-abc7-83d02d9868fe)

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/f343367d-e736-446c-b3b7-cebbef7f51f7)

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/e35345a5-1aac-439f-87ff-e5f563501102)

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/b5ff0470-36ac-4015-9024-c1c9c280b5fd)

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/ace4d54b-0f82-4064-9c11-3efe9c3b6c6b)

