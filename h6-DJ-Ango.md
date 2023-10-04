# H6 DJ Ango

## x) Tiivistelmä

Python Web - Idea to Production - 2023
* Opit palvelemaan asiakkaita eri alustoilla.
* Opit Keräämään tietoa palvelun käytöstä.
* Opit antamaan käyttäjien muokata tietoja yhtä aikaan ilman asennusta.
* Opit pitämään ohjelmat aina ajan tasalla.

Django 4 Instant Customer Database Tutorial
* Djangon asennus.
* Django projektin pystyttäminen.
* Käyttöhien luominen ja muokkaaminen.

Deploy Django 4 - Production Install
* Djangon ja Apachen yhdistäminen.
* Molempien configurointi.
* Pythonin lisäys.
* Projektin teko ja ylläpitäjän hallinta.

## a) Asenna Django

Aloitetaan komennolla "sudo apt-get -y install virtualenv" ja tämän jälkeen luodaan uusi kansio komennolla "virtualenv --system-site-packages -p python3 env/"

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/69720f3b-6f99-4620-b5ba-36c121576d6f)

Seuraavaksi liityin (env) ympäristöön. Ympäristössä lisätään Python paketti tekstitiedostoon. Komenolla "micro requirements.txt saadaan tekstiedotori esiille johon laitetaan pelkkä "django" ja testataan catilla et se onnnistui. Tämän jälkeen "pip install -r requitements.txt" avulla ladataan Django ja "django-admin --version" avulla katsotaan onko oikea versio.

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/e434e037-0c8d-411f-a5ee-16a1f4239a21)

Asennuksen jälkeen luodaan oma projekti "django-admin startproject alanti" ja vielä käynnistetään se "./manage.py runserver" 

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/0615b807-2130-4eb9-a4f1-f7da0d37b13c)

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/4cd41674-d38a-4ea4-a321-aa0a3ca69406)
