# LAB13. Backup dan Restore Pada Mikrotik

<img width="836" height="383" alt="image" src="https://github.com/user-attachments/assets/801c9274-d69f-44dd-97c9-17e3649a7633" />

Assalamualaikum Wr.Wb

Pada Kali ini saya akan membagikan LAB mengenai backup & restore

<h2> Apa itu backup?? </h2>

Backup  adalah proses menyimpan semua konfigurasi yang sudah di setting pada mikrotik kita. Kenapa hal ini perlu?? karna tanggal sial tidak ada di kalender maka untuk mengantisipasi mikrotik kita yang tiba-tiba error dan tidak bisa menyala sama sekali bahkan harus hard reset maka backup ini bisa membantu mengembalikan semua konfig yang sudah di terapkan sebelumnya pada mikrotik teman-teman.

**Yang harus kalian tau :** File backup ini nanti akan berupa file dengan format **.backup** dan tidak bisa kalian baca di notepad atau software text editting lainnya karna file yang di simpan berupa angka biner yang hanya bisa di baca oleh mesin. Satu lagi backup ini menyimpan seluruh konfigurasi bahkan username dan password itu sendiri.

<h2> Apa itu Restore </h2>

Sebaliknya Restore adalah proses menyimpan kembali konfigurasi dari file backup, simpel lah yaa?? :)

**Yang harus kalian tau :** Saat proses restore mikrotik akan me-reboot sendiri karna memang begitu proses restore, dan juga jangan lupa dengan password yang sudah di buat pada backup kenapa? karna ketika ingin melakukan restore akan di mintai password untuk melanjutkan proses restore

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

1. Remote seperti biasa bisa kan yaa?

2. Buka bagian **File>>Uploud**

   kang kenapa uploud dulu? karna kita ingin menyimpan file backupnya ke penyimpanan mikrotik, lahh ko gitu? jadi saat teman-teman dapat tanggal sial maka mikrotik jelas akan mengalami error dan apesnya bisa sampe hard reset maka dari itu mikrotik pasti dalam keadaan default/blank configuartion, NAHH dari sini kita harus menyimpan filenya terlebih dahulu sebelum melakukan restore

   <img width="652" height="324" alt="Screenshot 2026-08-02 155415" src="https://github.com/user-attachments/assets/5a01fe9e-3f89-4882-9099-ee65d7e6b37a" />

3. Cari file backup dari pc kita lewat file manager

   Note: Saya sudah merubah nama filenya agar kalian bisa tau kalau cara uploud ini berhasil okee?

   <img width="676" height="484" alt="Screenshot 2026-08-02 155855" src="https://github.com/user-attachments/assets/1aef321f-0188-44f6-a021-bc5b4b283b0b" />

4. Pilih File backup yang sudah kalian uploud tadi lalu klik restore

   <img width="763" height="386" alt="Screenshot 2026-08-02 155951" src="https://github.com/user-attachments/assets/8a887671-b292-42ea-a755-783f24130835" />

5. Klik restore lalu masukan password (bila ada), password apa? password yang kalian buat di backup tadi. Karna saya tidak memasukan password maka saya kosongkan saja

   <img width="372" height="145" alt="Screenshot 2026-08-02 160044" src="https://github.com/user-attachments/assets/523230ef-d3aa-4d8d-a1e2-e2308ccab001" />

6. Lalu klik yes

   Tunggu mikrotik me-reboot sendiri kurang lebih 30-60 detik, dan kembali ke tampilan awal winbox

   <img width="272" height="111" alt="Screenshot 2026-08-02 160103" src="https://github.com/user-attachments/assets/eadca153-5bbd-48f6-8650-7286053c30f4" />

7. Mikrotik Sukses melakukan restore


   # Tips Backup & Export

   Export apa sih?? nanti ada ko di next lab :)

- Lakukan backup dan export secara berkala, baik secara manual atau otomatis (scheduler)
- Backup hanya direkomendasikan untuk router yang sama
- Untuk router dengan type yang sama atau type yang berbeda, silakan gunakan export
- Simpan file backup atau export di luar router (misal laptop)
- Bisa juga file backup dikirim via email

  # Kesimpulan

  Backup adalah cara kita agar dapat menyimpan konfigurasi kalau kalau kita mendapatkan musibah masih ada backup yang dapat membantu. Restore proses mengembalikan konfigurasi dari file backup. Yang harus di perhatikan password, Type router, dan penyimpanan file backup, jangan sampai teman-teman lupa menyimpan file backup-nya di laptop masing-masing.

  Akhir kata

  Wassalamualaikum Wr.Wb




