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


## b) Rauta

Kokeilin sudo lshw -short -sanitize komentoa, joka ei toiminut, jonka jälkeen latasin lhsw käyttämällä sudo apt-get -y install lshw. Latauksen jälkeen kokeilin komentoa: sudo lshw -short -sanitize ja sain ruadan tiedot sitä kautta. 

![image](https://github.com/bgx088/linux-kurssi/assets/143337810/3ec2b818-796c-4bba-b48b-95be5f11e84c)



