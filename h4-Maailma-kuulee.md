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




  
