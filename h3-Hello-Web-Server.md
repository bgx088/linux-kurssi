# H2 Hello Web Server

## X)Tiivistelmä

Sivulla on esitetty miten voidaan asentaa Apache Web Server:
  * sudo apt-get install apache2: Asennetaan apache2
  * http://localhost : Voidaan löytää oma palvelin selaimesta
  * sudo a2enmod usedir: Annetaan oikeudet käyttäjälle luomaan sivusto
  * sudo systemctl restart apache2: Jotta oikeudet saadaan käyttöön joudutaa tämän komennon avulla käynnistämään apache2 uudelleen
  * Lopuksi voidaan testata, että sivusto toimii, luomalla "mkdir public_html" avulla tiedosto ja lopuksi vielä etsitään selaimen avulla oma sivusti "http://localhost/~omanimi/".
