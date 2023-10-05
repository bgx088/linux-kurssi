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

## b) Tee yksinkertainen esimerkkitietokanta django-kehitysympäristöön

Lisätään /admin url osoitteeseen. http://127.0.0.1:8000/admin/. Päivitetään tietokanta"./manage.py makemigrations" ".manage.py migrate" ja lisätään käyttäjä "./manage.py creatsuperuser" ja ladataan pwgen, jonka avulla voidaan luoda salasanoja. 

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/2be58bf6-7688-4f96-acc8-6356edc9dd98)

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/743aef5b-7cad-4655-9ab7-97fb77e009f5)

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/a3e8431b-41e6-412d-a4d9-e6c6b19070bc)

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/d3bdbb0f-023a-46b4-845c-d86cf0ca6fbb)

Näin superuser on luoto ja kirjauduttu sisään 127.0.0.1:8000/admin/

Seuraavaksi luodaan asiakas tietokanta ".manage.py startapp crm" ka lisätään crm tiedostoon "micro alanti/settings.py" 

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/2a881678-3234-4973-9b37-f61f1d693d89)

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/99d6c461-321d-4b29-ade2-bc9f7e37249f)

Seuraavaksi lisätään models, jossa on customer luokka "micro crm/models.py". Tässä vaiheessa tein kirjoitus virheen "max_lenght" , mutta onneksi huomasin sen heti.

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/dccdf2a5-ce35-49ae-af16-d93d11f97898)

Seuraavaksi lisätään tämä adminiin "micro crm/admin.py". Tämän jälkeen käynnistetään ja kirjaudutaan adminina sisään.

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/5e0a30fa-0a47-4b59-bb33-dc568a282462)

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/7d9e0c52-9998-4e04-ae37-c4d10b4ca528)

Ja näin Customers on luotu

## Lähteet

https://terokarvinen.com/2022/django-instant-crm-tutorial/

https://terokarvinen.com/2023/python-web-idea-to-production/#osaamistavoitteet

https://terokarvinen.com/2022/deploy-django/
