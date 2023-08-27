 # X

 Raportin kirjoittaminen: 
  -sdfgjsgdhfgsjhfd
   
 
 # H1 Oma linux

 ## 15.08.2023 virtualikoneen asentaminen
 Raudan tiedot:

 Prosessori: AMD Ryzen 7 5700x

 Ram: 32gb 3600hz 

 Näytönohjain: NVIDIA RTX 3080 - 12gb

 Järjestelmä: Windows 11 


Käytin opettajan sivulta löytyvää asennus ohjetta: https://terokarvinen.com/2021/install-debian-on-virtualbox/

Alkuun latasin VirtualBox ohjelman ja sen kautta loin uuden virtuaalikoneen ja laitoin ohjeen mukaan tarvittavat asetukset (64-bit, "Skip Unattended Install", lisäsin muistin määrä). Tämän jälkeen tein virtual hard diskin ja laitoin siihen muistin määräksi 60GB. Tämän jälkeen menin "new" kohtaan ja lisäsin ISO image kohtaan "debian-live-12.1.0-amd64-xfce.iso".

Tämän jälkeen kun luulin että kaikki on valmista tupla klikkasin debian virtualkonetta ja minulle tuli "Aborted" status ja debian ei mennyt päälle. Pienen selvituksen jälkeen ongelmaksi selvisi että omalla tietokoneella ei ole virtualmachine asetus päällä, jonka jälkeen jouduin sammuttamaan koneen ja laittaa BIOS asetuksista virtuaalikone asetuksen päällä ja tämän jälkeen pystying normaalisti käyttäämään virtuaalikonetta.

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/adbdc331-5685-45c3-8294-95e9d5b7f947)

  ## Debian asennus
  
Tämän jälkeen painoin ohjeiden mukaan aloitus näytöllä olevaa "install debian". Avautui ikkunam, jossa laitoin ohjeiden mukaan kaikki tarvittavat asetukset ja "summary" kohdassa oli bugi jossa ei näkynyt "install" painiketta ja tunnilla opettaja näytti ohjeet miten sen saa näkyviin painamalla pientä neliön muotoista painiketta oikealla yläkulmassa, jonka jälkeen install nappi ilmestey ja sitä pystyi painamaan.

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/436eb02f-aaa8-4eb1-9343-9b5899411bb0)

installin jälkeen --> 

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/2a07ecb4-888d-4e95-94a3-dad165979288)

## Lataus tehty
![image](https://github.com/bgx088/linux-kurssi/assets/143337810/c995ac4d-04ed-44f2-85d9-c9fdc96af319)

Testasin, että selain toimii ja kaikki kirjaimet toimii (öäå). Tämän jälkeen avasin Terminal Emulator ja latasin päivitykset ohjeen mukaan.

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/a955096b-dfc9-4fff-923e-8a1c84e7d5f8)

Lisää päivityksiä

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/703c89f9-3b7e-4b8f-9027-adc435f448b4)

tämän jälkeen palomuurin asennus ja käyttöönotto 

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/7ab59f66-1d02-4a22-9601-fd24edc2050e)

Käynnistin uudelleen ja nyt minulla on kaikki valmista!

Tein viel vapaaehtoisen tehtävän, jossa pystyn nyt säätämään ikkunan kokoa, joka helpottaa työskentelyä huomattavasti.

Ennen

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/a507bed2-bc17-4436-a08c-a263b45a1203)

Jälkeen 

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/c6e18fb9-7c23-4166-876c-2a40b84ec485)


All DONE




