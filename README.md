# Arsitektur-Multiprocessor
## Arsitektur Multiprocessor SIMETRIS
![image](https://github.com/user-attachments/assets/915d2a39-db8e-4448-aa4c-b59d529b528a)

## Arsitektur Multiprocessor ASIMETRIS
![image](https://github.com/user-attachments/assets/403b6f12-a411-4155-bf1c-6a6ccf1c00a7)

## 1. Arsitektur Multiprosesor Simetris (SMP)
Konsep utamanya: Semua prosesor punya peran yang sama, tidak ada yang lebih tinggi atau lebih rendah.

## Penjelasan gambar:
Ada beberapa prosesor (Processor 1, 2, 3, 4) ➔ Semua prosesor ini bisa mengakses memori utama dan jaringan dengan kekuatan yang sama.

Masing-masing prosesor punya cache sendiri ➔ Cache ini tempat data sementara supaya proses lebih cepat, tanpa harus bolak-balik ke RAM.

Semua prosesor terhubung ke satu Memory Controller ➔ Memory Controller ini yang bertugas ngatur keluar masuknya data ke memori utama (Shared Memory).

Setelah lewat Memory Controller, ada dua jalur:

➔ Shared Memory: Tempat semua prosesor bisa baca dan tulis data yang dipakai bareng.

➔ Interkoneksi jaringan: Untuk akses ke jaringan data (kayak server, internet, dll).

Jaringan Data dan Jaringan Perintah:
➔ Jaringan data buat transfer file besar.
➔ Jaringan perintah buat kirim instruksi kecil.

## 2. Arsitektur Multiprosesor Asimetris (AMP)
 Konsep utamanya: Ada satu CPU Master yang mengatur semua CPU lain (CPU Slave).

## Penjelasan gambar:
Ada satu CPU Master ➔ Dialah bos yang memberikan instruksi ke CPU lainnya (Slave).

## CPU Master:

➔ Ngatur komunikasi ke semua CPU Slave.

➔ Langsung berhubungan ke Memory Controller.

## CPU Slave:

➔ menunggu perintah dari CPU Master.

➔ tidak bisa ambil keputusan sendiri.

Semua CPU (baik Master maupun Slave) terhubung ke Memory Controller untuk ambil atau simpan data.

## Memory Controller ngatur akses ke:

➔ RAM (Memory Utama).

➔ Cache (untuk data yang sering diakses biar lebih cepat).

Ada juga jalur dari CPU Master ke Input/Output Controller:

➔ Ini buat akses ke Storage (kayak harddisk, SSD) dan peripheral devices (kayak keyboard, printer).
