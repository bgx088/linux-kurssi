# H4 Maailma kuulee

## x)Tiivistelmä

Sivulla on kerrottu miten voidaan luoda uusi virtuaali palvelin (esimerkkinä DigitalOcean).

* Opiskelijat voivat lunastaa GitHub Education student pack, joka sisältää virtuaali palvelimen ja domain nimen.

* Ensimmäinen ja viimeinen kerta kun kirjaudutaan roottiin "ssh root@10.0.0.1". Kirjautumisen jälkeen annetaan VAHVA salasana.

* Tehdään reikä SSH:ta varten (serveri avain) "sudo ufw allow 22/tcp" ja tämän jälkeen aktivoidaan palomuuri "sudo ufw enable".

* Tehdään käyttäjä ja lukitaan root käyttäjä.

* Lopuksi vielä haetaan päivitykset "sudo apt-get update" ja "sudo apt-get upgrade"

## a) Vuokraa oma virtuaalipalvelin

Lähetin Github Education-paketti hakemuksen ja sain hyväksytyn vastauksen noin viiden päivän päästä. Lunastin GitHub Educational-paketin, kirjautumalla DigitalOceaniin Githubin kautta (jouduin syöttää luottokortin tiedot, vaikka ei veloitusta ollutkaan). Saatuani edut, valitsin "Create Droplet". Valitsin sijainniksi Frankfurt/Saksan (kannattaa valita sijainti, joka on lähimpänä asiakasta). Valitsin Debianin ja versioksi 12 x64. Valitsin myös Basic CPU-vaihtoehdoista, Disk type: SSD ja toisiksi halvin vaihtoehto, joka taisi olla 6$ kuussa. Lopuksi vielä vahva salasana Rootille.

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/c990af14-1a7d-4bed-aa7e-7d5d258581ef)

## b) Tee alkutoimet

Tietenkin aluksi päivitetään "sudo apt-get update". Tämän jälkeen tarkastin, että onko minulla ssh komennolla "ssh" ja selvisi, että sitä ei ole,joten asensin SSH "sudo apt-get install openssh-client" ja testasin löytyykö se. 

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/cb5d0118-6306-4cbf-bb85-5de5a19d4536)

Asennuksen jälkeen loin ssh-yhteyden palvelimeen "ssh root@161.35.204.205", jonka jälkeen kirjoiten yes ja rootin salasanan. 

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/68ddc3ae-33b2-4441-9962-d7dee53fe0cf)

Asensin palomuurin "sudo apt-get install ufw" ja tein vielä reiän palomuuriin "sudo ufw allow 22/tcp". Lopuksi aktivoin palomuurin "sudo ufw enable". (Tein tämän aluksi vahingossa normaaliin terminaaliin enkä roottiin) :D

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/2e5fa856-07a9-466e-85b2-741bb75c9749)

Lisin vielä käyttäjän "sudo adduser alan" ja lisäsin vielä sudo oikeudet "sudo adduser alan sudo"

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/66cfad9a-dfa6-4243-b862-33c020583e87)

Lukitsin vielä root-käyttäjän (oletan, että ei tule erikseen ilmoitusta kun se on lukittu) testasin vielä toisessa terminaalissa.

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/162da206-6238-45b3-894e-b76f3effb0b5)

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/df78d88f-4fd9-4003-be02-7e3cdc5ba376)

## c) Asenna weppipalvelin omalle virtuaalipalvelimellesi

Muodostin ssh-yhteyden "ssh alan@161.35.204.205" ja asensin apachen tuttuun tapaan "sudo apt-get install -y apache2" ja käynnistin "sudo systemctl start apache2"

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/71809a7a-c7da-42f0-9fa1-fec62db0f1a7)

Tein viel reiän palomuuriin, jotta saadaan yhteys sivulle. Täällä kertaan "sudo ufw allow 80/tcp" 

Testasin vielä, että sivusto löytyy selaimesta (haku ip-osoitteella) "161.35.204.205". Löytyihän se (kokeilin myös puhelimella).

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/8cb5218f-59b9-49cd-9c40-5d1e13464c7a)

## d) Murtautumisyritykset

Kävin vielä nopeasti vilkaisemassa murtautumisyritkset "journalctl SYSLOG_FACILITY=10 # auth events", mutta jostain syystä en nähnyt mitään lokeja? Kokeilin muita komentoja, mutta mikään ei näyttänyt toimivan.

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/673e8514-f122-4ea8-9daf-a94fda7c903a)

## Lähteet:

First Steps on a New Virtual Private Server - an Example on DigitalOcean and Ubuntu 16.04 LTS,(Tero Karvinen,2017. Luettavissa: https://terokarvinen.com/2017/first-steps-on-a-new-virtual-private-server-an-example-on-digitalocean/

Linux palvelimet 2023 alkusyksy,(Tero Karvinen, 2023). Luettavissa: https://terokarvinen.com/2023/linux-palvelimet-2023-alkusyksy/














  
