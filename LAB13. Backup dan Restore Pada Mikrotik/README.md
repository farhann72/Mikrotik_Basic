# LAB13. Backup dan Restore Pada Mikrotik

<img width="836" height="383" alt="image" src="https://github.com/user-attachments/assets/801c9274-d69f-44dd-97c9-17e3649a7633" />

Assalamualaikum Wr.Wb

Pada Kali ini saya akan membagikan LAB mengenai backup & restore

<h2> Apa itu backup?? </h2>

Backup  adalah proses menyimpan semua konfigurasi yang sudah di setting pada mikrotik kita. Kenapa hal ini perlu?? karna tanggal sial tidak ada di kalender maka untuk mengantisipasi mikrotik kita yang tiba-tiba error dan tidak bisa menyala sama sekali bahkan harus hard reset maka backup ini bisa membantu mengembalikan semua konfig yang sudah di terapkan sebelumnya pada mikrotik teman-teman.

Yang harus kalian tau : File backup ini nanti akan berupa file dengan format **.backup** dan tidak bisa kalian baca di notepad atau software text editting lainnya karna file yang di simpan berupa angka biner yang hanya bisa di baca oleh mesin. Satu lagi backup ini menyimpan seluruh konfigurasi bahkan username dan password itu sendiri.

# Praktik Backup

1. Remote mikrotik teman-teman menggunakan winbox sesuai topologi di atas

2. klik di bagian menu winbox pada bagian **File** klik pada bagian backup

<img width="602" height="416" alt="Screenshot 2026-08-02 151931" src="https://github.com/user-attachments/assets/e7b72eb8-ab7f-4762-a2ac-e45b2bab4e52" />

3. Beri nama file backup

**Hati-hati** file backup bisa kalian beri password untuk alasan keamanan, password ini juga lah yang nanti di butuhkan kembali untuk proses restore

<img width="297" height="146" alt="Screenshot 2026-08-02 152015" src="https://github.com/user-attachments/assets/fd820970-b479-4110-8c9a-3d2b61672e17" />

4. Cari file backup tersebut lalu simpan pada komputer teman-teman

Caranya bisa dengan cara drag and drop dan download

  a. drag and drop

  -kecilkan tab winbox teman-teman

  -buka file manager dan siapkan pula tempat untuk menyimpan filenya

  -tekan dan tahan lalu geser ke arah folder yang sudah kalian sediakan di file manager

   <img width="1130" height="628" alt="Screenshot 2026-08-02 152718" src="https://github.com/user-attachments/assets/7e3fd3a4-075c-45d7-ac09-afe6c15b6c6b" />

  b. download

   -klik kanan pada bagian file backupnya

   -klik download

  <img width="818" height="448" alt="Screenshot 2026-08-02 153415" src="https://github.com/user-attachments/assets/e963d769-59ed-474e-977f-43e934679bc8" />

   -arahkan pada folder yang ingin kalian simpan lalu klik Ok

   <img width="336" height="338" alt="Screenshot 2026-08-02 153456" src="https://github.com/user-attachments/assets/c8979a52-0576-45be-b750-ebf6b9466345" />

5. Itulah cara backup dan menyimpan filenya pada komputer kita

# Praktik Restore

