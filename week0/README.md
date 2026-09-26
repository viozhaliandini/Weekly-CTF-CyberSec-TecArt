# Week 0 - CyberSec TecArt

**NIM:** 260530911032  
**Nama:** Dewa Ayu Viozha Liandini  
**Divisi:** Cyber Security

## Kategori CTF

**Forensics**

## Tools yang Digunakan

- WSL Ubuntu
- Python 3.14.4
- Git/GitHub
- ExifTool 13.50

---

## 1. Pengujian WSL

WSL Ubuntu digunakan sebagai lingkungan Linux untuk menjalankan tools Cyber Security.

Perintah yang digunakan:

```bash
mkdir Week0-CyberSec-TecArt
cd Week0-CyberSec-TecArt
touch README.md
```
README kemudian dibuat dan diisi dengan identitas peserta.

### Dokumentasi
![NIM Nama dan Divisi](https://raw.githubusercontent.com/viozhaliandini/Week0-CyberSec-Tecart/main/Screenshot%202026-09-08%20175832.png)




## 2. Pengujian Python

Python digunakan untuk menjalankan program sederhana pada WSL Ubuntu.

Perintah untuk mengecek versi Python:

python3 --version

Hasil pengujian menunjukkan Python 3.14.4.

Program sederhana kemudian dijalankan dan menghasilkan output:

Hello TecArt
Viozha

### Dokumentasi
![Pengujian Python](Screenshot%202026-09-08%20175858.png)





## 3. Git/GitHub

Git digunakan untuk mengelola project dan GitHub digunakan sebagai tempat penyimpanan repository tugas.

Repository tugas dibuat dengan nama:

Week0-CyberSec-Tecart

Repository dibuat dalam keadaan Public agar dapat diakses untuk keperluan pengumpulan tugas.




## 4. Instalasi dan Pengujian ExifTool

ExifTool digunakan untuk membaca dan menganalisis metadata pada file.

Instalasi dilakukan menggunakan perintah:

sudo apt install exiftool -y

Versi ExifTool kemudian diperiksa dengan:

exiftool -ver

Hasil pengujian:

13.50

### Dokumentasi
![Instalasi ExifTool](Screenshot%202026-09-08%20190618.png)





## 5. Challenge Forensics - Information

Challenge information dikerjakan menggunakan ExifTool untuk mencari informasi pada file gambar.

File cat.jpg dianalisis menggunakan perintah:

exiftool cat.jpg

Dari hasil metadata ditemukan teks yang dikodekan menggunakan Base64.

Teks tersebut kemudian didekode menggunakan perintah:

echo 'cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9' | base64 -d

Hasil flag:

picoCTF{the_m3tadata_1s_modified}

Flag kemudian dimasukkan ke challenge dan berhasil mendapatkan status Correct flag!

### Dokumentasi
![Challenge Forensics](Screenshot%202026-09-08%20184005.png)

![Memasukkan Jawaban CTF](Screenshot%202026-09-08%20184113.png)

![Correct Flag](Screenshot%202026-09-08%20184125.png)










## 6. Challenge Common - Undo

Challenge Undo dikerjakan menggunakan terminal.

Tahapan penyelesaian yang dilakukan:

1. Melakukan decode Base64 menggunakan base64 -d.


2. Membalik teks menggunakan rev.


3. Mengubah karakter - menjadi _ menggunakan tr.


4. Melakukan transformasi karakter sesuai instruksi challenge.


5. Challenge berhasil diselesaikan.



### Dokumentasi
![Step Challenge Undo](Screenshot%202026-09-08%20211428.png)

![Memasukkan Jawaban Undo](Screenshot%202026-09-08%20204203.png)

![Correct Undo](Screenshot%202026-09-08%20204215.png)







Kesimpulan

Homework 00 telah dikerjakan dengan menggunakan WSL Ubuntu, Python, Git/GitHub, dan ExifTool.

Kategori CTF yang dipilih adalah Forensics.

Tools ExifTool telah berhasil diinstal dan diuji. Challenge information pada kategori Forensics berhasil diselesaikan dan menghasilkan flag yang benar. Challenge Undo juga telah berhasil diselesaikan.

Seluruh dokumentasi proses dan hasil pengujian dilampirkan dalam repository ini.
