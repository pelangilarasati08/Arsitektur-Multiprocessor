# Arsitektur-Multiprocessor
## Arsitektur Multiprocessor SIMETRIS
![image](https://github.com/user-attachments/assets/915d2a39-db8e-4448-aa4c-b59d529b528a)

## Arsitektur Multiprocessor ASIMETRIS
![image](https://github.com/user-attachments/assets/403b6f12-a411-4155-bf1c-6a6ccf1c00a7)

## Penjelasan Arsitektur Simetris (SMP):
Pada arsitektur ini, semua prosesor memiliki kedudukan dan peran yang sama rata. Artinya, tidak ada satu prosesor yang lebih dominan daripada yang lain.
Di dalam diagram, kita bisa lihat ada empat prosesor, yaitu Processor 1, 2, 3, dan 4.
Masing-masing prosesor memiliki cache sendiri untuk menyimpan data sementara, sehingga proses komputasi menjadi lebih cepat.
Semua prosesor ini terhubung ke satu Memory Controller.
Memory Controller bertugas mengatur alur data antara prosesor dan Shared Memory, yang digunakan bersama.

Kemudian, dari Memory Controller, aliran data bisa masuk ke jaringan, melalui:
*Jaringan Data untuk kebutuhan data besar,
*dan Jaringan Perintah untuk komunikasi perintah eksekusi.

Secara sederhana, dalam arsitektur ini, semua prosesor saling berbagi memori dan perangkat dengan hak akses yang setara."

## Penjelasan Arsitektur Asimetris (AMP):
Berbeda dengan Simetris, di sini ada pembagian tugas yang jelas antara CPU.
Satu CPU bertindak sebagai Master, dan CPU lainnya sebagai Slave.
CPU Master bertugas untuk mengendalikan seluruh sistem, mulai dari mengatur tugas, mengelola memori, hingga mengontrol akses ke perangkat input-output.

Sementara itu, CPU Slave hanya bertugas untuk menjalankan instruksi yang diberikan oleh CPU Master, tanpa melakukan koordinasi sendiri.
Semua CPU, baik Master maupun Slave, juga terhubung ke Memory Controller, yang mengakses RAM, cache, serta mengatur penyimpanan data.
Dengan model ini, koordinasi lebih sederhana, namun beban kerja cenderung berat di CPU Master."
