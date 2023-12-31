# H2 Komentaja Pingiviini

# x) Tiivistä

$ pdw Prints the working directory

$ ls lists files in the working directory

$ cd (text) you can move to directory and with cd.. you change dictory up.

## File Manipulation

$ nano FOO.TXT creates texteditor file (in nano)

$ mkdir name creates new folder in directory

$ mv name1 name2 moves folders from 1 to 2

$ cp -r copies with all contents

$ rmdir removes empty directory

$ rm FILE removes file called FILE

$ rm -r FILE removes the whole file and all contents (hard to get back)

## Help

$ man ls shows manual for commands

pressin [tab] helps you autocomplete your commands 

$ ls /var/log/ you can check logs to see what has been done

## Administrative Commands

$ sudo apt-get update updates all available packages

$ sudo apt-get -y install (program) this way you can install programs

$ sudo apt-get purge (program) deletes the program

## a) Asenna Micro

Asensin Micron komennolla apt-get -y install micro

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/0559c41a-9c11-4386-9761-673ce418ac18)

Lähteet:Command Line Basic Revisited, Tero Karvinen. https://terokarvinen.com/2020/command-line-basics-revisited/?fromSearch=command%20line%20basics%20revisited
## b) Rauta

Kokeilin sudo lshw -short -sanitize komentoa, joka ei toiminut, jonka jälkeen latasin lhsw käyttämällä sudo apt-get -y install lshw. Latauksen jälkeen kokeilin komentoa: sudo lshw -short -sanitize ja sain ruadan tiedot sitä kautta. 

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/3ec2b818-796c-4bba-b48b-95be5f11e84c)

Listauksessa näköö esimerkiksi oman koneen prosessori "Processor --> AMD Ryzen 7 5700x 8-Core Processor"

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/ca902c53-38c0-4757-91a1-187305ad5a10)


Näkyy myös virtualboxin kautta esimerkiksi tietokoneen hiiren käyttä ja lisäksi virtualboxin kovalevy muisti (64GB). 

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/dc3b0887-3507-4928-b209-0efeb39cd578)

Lähteet: https://micro-editor.github.io

## c)Apt

1. Ternimator: Latasin käyttöen sudo apt-get -y install terminator

   Ohjelma mahdollistaa useamman terminaalin käytön samanaikaisesti.

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/d4bcaa13-7f3a-4495-bd83-81917d69df50)

2. Tilda: Latasin käyttäen sudo apt-get -y install tilda

   Ohjelma mahdollistaa ulkonäön muokkaamista terminaalin sisällä.

   ![image](https://github.com/bgx088/linux-kurssi/assets/143337810/819c7eed-7b70-491d-a9f2-ce395d531cf6)

3. Kitty: Latasin käyttäen sudo apt-get -y install kitty

   Tämäkin mahdollistaa useamman terminaalin avaamisen.

   ![image](https://github.com/bgx088/linux-kurssi/assets/143337810/314d5b76-54f0-47fe-96de-0c0abf5f2815)

Lähteet: linux-terminal-emulators,Ravi Saive. https://www.tecmint.com/linux-terminal-emulators/

## d)FHS

Kansioiden listaus ls /

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/63242865-0993-48f1-a57c-38135d58a835)

Kokeilin erilaisia komentoja

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/31c5a8d3-d6b4-4204-ac63-9d547b6e208c)

## e)The Friendly M

Grep apuri jolla voidaan etsia tarvittavia asioita... esimerkiksi voidaan etsiä tiettyä lausetta haluamasta tiedostosta.

Yritin kokeilla, mutta en oikein saanut komentoa toimimaan tai ainakaan löytämään tarvittavia tietoja.

Lähteet: howto-use-grep-command-in-linux-unix. https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/

## f)Pipe

KUVA PUTKESTA!!!

putkella voidaa yhdistaa komentoja

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/5874962b-da47-40ff-b478-436399c5bf58)

## g)Tukki

Kokeilin aluksi /var/log ls komentoia jostain sain listan komentoja ja yritin kokeilla boot.log komentoa, mutta tuli "Binary file" niin päätin olla avaamatta.

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/4bd2b42c-7853-4b22-8a29-06e1f20d3ecb)

Selasin lisää logeja ja löysin vmboxin asennus login

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/1e5a8941-24a4-414a-a119-ab9b0d81b91c)


## Lähteet:

Karvinen,T.2020. Command Line Basic Revisited. Luoettavissa: https://terokarvinen.com/2020/command-line-basics-revisited/?fromSearch=command%20line%20basics%20revisited

Ravi Saive. Linux-terminal-emulators. Luettavissa: https://www.tecmint.com/linux-terminal-emulators/

Luettavissa: https://micro-editor.github.io












   



