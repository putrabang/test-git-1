# **GENERAL SKILLS CHALLENGES WRITE UP**
## by moo
---

## **Obedient Cat** author by **SYREAL**
### Description :
1. Kamu download flagnya menggunakan command *wget*.
   
    ```
    wget https://xxxxx
    ```
2. Setelah itu file bernama *flag*  akan muncul di direktori kalian, dan gunakan command *cat* pada file tersebut.
   
   ```
   cat flag
   ```
   Output :
   ```
   picoCTF{xxxxxxxxxxxxxxx}
   ```
## **Python Wrangling** author by **SYREAL**
1. Download Python Script, Password dan ciphertext (extensinya .en).
   
   ```
   ende.py flag.txt.en pw.txt
   ```

2. Kemudian, gunakan command *python3* untuk menjalankan python script. Di bawah ini terdapat 3 cara untuk mendapatkan flag yang terencode (flag.txt.en), kita harus mendecryptnya menggunakan switch -d.
   #### 1
   ```
   python3 ende.py -d flag.txt.en < pw.txt
   ```
   -d = decrypt 
   
   < = untuk memasukan sesuatu ke file sebelum <
   #### 2
   ```
   python3 ende.py -d flag.txt.en
   Please enter the password:68f88f9368f88f9368f88f9368f88f93
   ```
   #### 3
   ```
   cat pw.txt | python3 ende.py -d flag.txt.en
   ```
   
   Output :
   ```
   picoCTF{4p0110_1n_7h3_h0us3_68f88f93}
   ```
    > Source useful (https://www.bugninja.de/en/picoctf-python-wrangling-2/)

## **Wave a flag** author by **SYREAL**
