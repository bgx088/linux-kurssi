 # H1 Oma linux

 ## 15.08.2023 virtualikoneen asentaminen

Käytin opettajan sivulta löytyvää asennus ohjetta: https://terokarvinen.com/2021/install-debian-on-virtualbox/

Alkuun latasin VirtualBox ohjelman ja sen kautta loin uuden virtuaalikoneen ja laitoin ohjeen mukaan tarvittavat asetukset (64-bit, "Skip Unattended Install", lisäsin muistin määrä). Tämän jälkeen tein virtual hard diskin ja laitoin siihen muistin määräksi 60GB. Tämän jälkeen menin "new" kohtaan ja lisäsin ISO image kohtaan "debian-live-12.1.0-amd64-xfce.iso".

Tämän jälkeen kun luulin että kaikki on valmista tupla klikkasin debian virtualkonetta ja minulle tuli "Aborted" status ja debian ei mennyt päälle. Pienen selvituksen jälkeen ongelmaksi selvisi että omalla tietokoneella ei ole virtualmachine asetus päällä, jonka jälkeen jouduin sammuttamaan koneen ja laittaa BIOS asetuksista virtuaalikone asetuksen päällä ja tämän jälkeen pystying normaalisti käyttäämään virtuaalikonetta.

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/adbdc331-5685-45c3-8294-95e9d5b7f947)


