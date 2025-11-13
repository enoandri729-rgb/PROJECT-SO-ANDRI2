# PROJECT-OS-ANDRI2

# Project Based Learing 2

# LANGKAH 1 BUAT STRUKTUR DIREKTORI DAN FILE

#Berikut contoh perintah membuat direktori project_sistem_operasi_b dan sub-direktori src, doc, data:

*mkdir project_sistem_operasi_b
*cd project_sistem_operasi_b
*mkdir src doc data

https://drive.google.com/file/d/1qTCzcNqx2gVlr2nbMQtGDfVEyoBs0kvK/view?usp=drivesdk

Berikut contoh perintah membuat dan mengisi file README.MD dan file file1.txt:
touch README.MD
echo "Tugas 2 Andri Eno Kelas SI A" > README.MD
touch file1.txt

https://drive.google.com/file/d/1qTCzcNqx2gVlr2nbMQtGDfVEyoBs0kvK/view?usp=drivesdk

Berikut contoh perintah berpindah ke direktori doc dan membuat file file2.docx:
cd doc
touch file2.docx
cd ..

https://drive.google.com/file/d/1qTCzcNqx2gVlr2nbMQtGDfVEyoBs0kvK/view?usp=drivesdk

Penjelasan:
 * mkdir → membuat folder baru.
 * cd → berpindah direktori.
 * touch → membuat file kosong dengan cepat.
 * echo "Teks" → menulis teks ke dalam file.

 #LANGKAH 2 SCRIPT PENGHITUNG UKURAN FILE

Pindah ke direktori src dan buat script yang akan menghitung ukuran direktori:
cd src
nano main.sh

https://drive.google.com/file/d/1qUOiDikoObeE1SS2v4n3p5bLzS_psx4M/view?usp=drivesdk

ISI SCRIPT (main.sh)
Ketikkan isi script persis seperti yang Anda tunjukkan, yang menggunakan perintah du (Disk Usage):

# Menampilkan ukuran direktori project_sistem_operasi_b dalam format mudah di baca

https://drive.google.com/file/d/1qRZTQMl-Ozwg9_ymtgfH-8Gbl1kDhJ1h/view?usp=drivesdk

#!/bin/bash
echo
echo "ukuran total:"
echo "==================================================="
du -sh ~/project_sistem_operasi_b
echo "==================================================="
echo
echo "ukuran per folder:"
echo "==================================================="
du -h ~/project_sistem_operasi_b
echo "==================================================="

Beri Hak Eksekusi dan Jalankan:
Berikan hak eksekusi pada script, lalu jalankan untuk melihat hasilnya:
chmod +x main.sh

./main.sh

Penjelasan:
 * nano → membuka editor teks untuk membuat/mengedit script.
 * du -sh [path] → menampilkan Disk Usage (penggunaan disk) total dalam format summary dan human-readable (mudah dibaca).
 * du -h [path] → menampilkan Disk Usage per sub-folder di path tersebut dalam format human-readable.
 * chmod +x → memberi izin eksekusi (execute) ke script.
