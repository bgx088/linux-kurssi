# H3 Hello Web Server

## x)Tiivistelmä

Sivulla on esitetty miten voidaan asentaa Apache Web Server:
  * sudo apt-get install apache2: Asennetaan apache2
  * http://localhost : Voidaan löytää oma palvelin selaimesta
  * sudo a2enmod usedir: Annetaan oikeudet käyttäjälle luomaan sivusto
  * sudo systemctl restart apache2: Jotta oikeudet saadaan käyttöön joudutaa tämän komennon avulla käynnistämään apache2 uudelleen
  * Lopuksi voidaan testata, että sivusto toimii, luomalla "mkdir public_html" avulla tiedosto ja lopuksi vielä etsitään selaimen avulla oma sivusti "http://localhost/~omanimi/".

Lähteet: Install apache web server on ubuntu, (Tero Karvinen, 2008) https://terokarvinen.com/2008/05/02/install-apache-web-server-on-ubuntu-4/

## a) Asenna Apache-webbipalvelin

Tämä osio tehtiin jo oppitunnilla ja unohdin ottaa kuvankaappaukset, mutta onneksi sain kaverilta kuvat. Tietenkin heti ensimmäisenä haetaan kaikki mahdolliset päivitykset "sudo apt-get update" komennon avulla, jonka jälkeen asennetaan itse apache "sudo get-apt install apache" komennon avulla. Lopuksi vielä käynnistetään palvelin "sudo systemctl start apache2" komennon avulla ja käydään vielä selaimen kautta katsomassa,että kaikki toimii. ("localhost" haku selaimessa)





![image](https://github.com/bgx088/linux-kurssi/assets/143337810/e8d040ed-cf07-4e6e-8c80-aba402ed32d3)

Toimii! :)

## b) Etsi lokista

Ensimmäiseksi haetaan oma sivusto selaimesta "http://localhost/~alan" ja saada virhekoodi "404 Not Found" ja tämähän on normaalia, sillä emme ole vielä louneet omaa sivustoa.

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/872ee4e4-2920-4611-9b6a-687d594c7f72)

Tämän jälkeen menin etsimään onnistuneita lokeja komennolla "sudo tail -F /var/log/apache2/access.log" ja tämän jälkeen vielä epäonnistuneet lokit komennolla "sudo tail -F /var/lor/apache2/error.log"

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/1c54b8b0-4f39-4b75-8136-21821be13069)

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/18e3fbf3-dc15-41d2-a835-a6e8b333953e)

Lokissa näkyy esimerkiksi milloin tapahtuma on tehty (päivämäärä muodossa), "GET" tarkoittaa, että jotakin haetaan (esimerkiksi /~alan HTTP/1.1", jonka perässy näkyy myös tuo edellinen 404 virhe ilmoitus, Mozilla on selain ja Linux x86_64 on meidän virtuaalikone/systeemi.



