## TUGAS SISTEM OPERASI

## Nama  : Yesi Paramita
## NIM   : 09011182328116
## Kelas : SK3B

## CARA MEMASANG DAN MENGOFIGURASI SSH DI UBUNTU

  SSH adalah protokol jaringan yang menyediakan koneksi aman antara klien dan server. Semua komunikasi dienkripsi, mencegah pencurian data yang dikirim melalui jaringan dan serangan jaringan jarak jauh lainnya.
Misalnya, Anda telah memesan server cloud dari Hostman. Anda perlu menginstal dan mengonfigurasi SSH untuk terhubung dan mengelola server.
Panduan di bawah ini akan menjelaskan cara menginstal SSH di Ubuntu 22.04 dan mengonfigurasinya

Langkah 1: Siapkan Ubuntu.\
Hal pertama yang perlu Anda lakukan sebelum mulai menginstal SSH di Ubuntu adalah memperbarui semua paket apt ke versi terbaru. Untuk melakukannya, gunakan perintah berikut:

![Cuplikan layar 2024-10-02 040642](https://github.com/user-attachments/assets/71625aea-843a-4409-8f7e-849ab22e216f)

Langkah 2: Instal SSH di Ubuntu.\
Open SSH belum terinstal di sistem, jadi mari kita instal secara manual. Untuk melakukannya, ketik di terminal:

![Cuplikan layar 2024-10-02 040732](https://github.com/user-attachments/assets/2386eff6-aec9-4cd4-ba78-2d7b52c95a10)

Instalasi semua komponen yang diperlukan akan dimulai. Jawab "Ya" untuk semua perintah sistem.
Setelah instalasi selesai, lanjutkan ke langkah berikutnya untuk memulai layanan.

Langkah 3: Mulai SSH.\
Sekarang Anda perlu mengaktifkan layanan yang baru saja Anda instal menggunakan perintah di bawah ini:

![Cuplikan layar 2024-10-02 040804](https://github.com/user-attachments/assets/de0849a2-04ef-465a-8f31-1fcae819a126)

Untuk memverifikasi bahwa layanan diaktifkan dan berjalan dengan sukses, ketik:

![Cuplikan layar 2024-10-02 040843](https://github.com/user-attachments/assets/995a3c6e-69ea-4965-be6c-c515ee341679)

Output harus berisi baris Aktif: aktif (berjalan), yang menunjukkan bahwa layanan berhasil berjalan.
Jika Anda ingin menonaktifkan layanan, jalankan:

![Cuplikan layar 2024-10-02 041756](https://github.com/user-attachments/assets/2590c42d-2fa9-46b9-9b3e-1ec345df1033)

Ini menonaktifkan layanan dan mencegahnya memulai saat boot.

Langkah 4: Konfigurasikan firewall.\
Sebelum menghubungkan ke server melalui SSH, periksa firewall untuk memastikannya dikonfigurasi dengan benar.
Dalam kasus kami, kami telah menginstal UFW, jadi kami akan menggunakan perintah berikut:

![Cuplikan layar 2024-10-02 050736](https://github.com/user-attachments/assets/521f785c-d58e-419a-bcd1-6fc8db6dc33e)

Pada output, Anda akan melihat bahwa lalu lintas SSH diizinkan. Jika tidak tercantum, Anda perlu mengizinkan koneksi SSH yang masuk. Perintah ini akan membantu Anda:

![Cuplikan layar 2024-10-02 041910](https://github.com/user-attachments/assets/4346440c-cc86-4cc0-a13d-4be0158e74e0)

untuk mengaktifkannya,ketik:

![Cuplikan layar 2024-10-02 051407](https://github.com/user-attachments/assets/37737149-aead-4712-be9a-8ec33153ef99)

Untuk melihat Ip Address:

![Cuplikan layar 2024-10-02 042033](https://github.com/user-attachments/assets/7f2de9fc-ee45-487f-a8ab-1dd3ab6ca024)

Langkah 5: Hubungkan ke server.\
Setelah Anda menyelesaikan semua langkah sebelumnya, Anda dapat masuk ke server menggunakan protokol SSH.
Untuk melakukan ini, Anda memerlukan alamat IP atau nama domain server dan nama pengguna yang dibuat di server.
Pada baris terminal, masukkan perintah:

![Cuplikan layar 2024-09-27 203204](https://github.com/user-attachments/assets/e500a5aa-4127-408f-a576-d196bdd95b2f)

![Cuplikan layar 2024-09-27 203223](https://github.com/user-attachments/assets/ead3ba8f-6809-43a8-bb45-88aa247073a6)

**Untuk menonaktifkan SSH:**

![Cuplikan layar 2024-10-02 052709](https://github.com/user-attachments/assets/5dcaf9b1-aacd-4a62-bc68-d53ab6d08a97)






