# LAB6. Fitur Quickset di MikroTik

Assalamualikum Wr. Wb

Pada kali ini saya akan membagikan materi Quick Set,  sebelumnya masuk praktek kita akan teoritis dulu yakk :}

# Apa itu Quick Set?

Quick Set adalah fitur pada MikroTik yang digunakan untuk melakukan konfigurasi dasar router dengan cepat melalui tampilan yang sederhana. Fitur ini sangat cocok untuk pengguna yang baru belajar karena tidak perlu melakukan konfigurasi satu per satu melalui terminal atau menu yang lebih kompleks

# Fungsi Quick Set

-Menghemat waktu konfigurasi.

-Mengurangi risiko kesalahan pengaturan.

-Mempermudah proses implementasi.

-Menstandarkan konfigurasi antar perangkat atau pengguna.


# Jenis-Jenis Quick Set

<h3>Home AP</h3>

-Digunakan untuk menjadikan MikroTik sebagai access point sekaligus router.

-Cocok untuk rumah atau kantor kecil.

-Mendukung Wi-Fi, DHCP, NAT, dan internet sharing.

<br>

<h3>Home Mesh</h3>

-Digunakan untuk menghubungkan beberapa perangkat MikroTik dalam jaringan mesh.

-Membantu memperluas jangkauan Wi-Fi tanpa konfigurasi yang rumit.

<h3> CPE (Client Premises Equipment) </h3>

-MikroTik berfungsi sebagai klien yang terhubung ke access point lain.

-Umum digunakan untuk koneksi point-to-point atau menerima internet dari ISP nirkabel.

<h3> WISP AP (Wireless ISP Access Point) </h3>

-Digunakan ketika MikroTik menjadi access point bagi banyak klien.

-Cocok untuk penyedia layanan internet berbasis wireless.

<h3> WISP AP Bridge </h3>

-Mirip WISP AP, tetapi menggunakan mode bridge sehingga perangkat dalam satu segmen jaringan.

<h3> Bridge </h3>

-Menghubungkan beberapa interface menjadi satu jaringan Layer 2.

-Tidak melakukan fungsi routing secara utama.

<h3> Router </h3>

-Digunakan ketika MikroTik berfungsi sebagai router utama.

-Menyediakan NAT, DHCP Server, firewall dasar, dan routing.

# PRAKTEK HOME AP (Dynamic)

<br>

<img width="685" height="405" alt="Screenshot 2026-07-31 152418" src="https://github.com/user-attachments/assets/f446a43b-4bec-4b07-b8fd-58c6f71da0f1" />

NOTE: Ip AP adalah ip accsess point/WIFI yang akan kita gunakan nanti untuk konfigurasi

1. Pastikan teman-teman sudah mengkoneksikan mikrotik sesuai dengan topologi yaa :)

2. Remote Mikrotik teman teman menggunakan winbox

3. Setting DHCP Client di ether 1 mikrotik

   <img width="282" height="294" alt="Screenshot 2026-07-31 145251" src="https://github.com/user-attachments/assets/b43fc70a-b66e-45fa-a290-69bfb0078a02" />


<img width="599" height="188" alt="Screenshot 2026-07-31 145332" src="https://github.com/user-attachments/assets/adf8cac1-c8ee-4c83-9594-f5a5c07e65f0" />

Pastikan statusnya bound yakk, biasa seperti sebelum-sebelumnya

4. Klik Quick set pada bagian menu awal winbox

   <img width="174" height="164" alt="Screenshot 2026-07-31 144233" src="https://github.com/user-attachments/assets/d4cb765a-7224-472f-8a25-a16e40e366a7" />

5. Ganti mode ke mode Home AP di bagian pojok kiri atas 

   <img width="513" height="125" alt="Screenshot 2026-07-31 144303" src="https://github.com/user-attachments/assets/6935fb04-32b3-4cbc-9286-8a109c2097fb" />

6. Teman teman bisa ganti di bagian sini

   <img width="512" height="212" alt="Screenshot 2026-07-31 144541" src="https://github.com/user-attachments/assets/3405ce1d-72a6-40e8-b690-a97517af93cc" />

  Name Network : nama wifi/ssid, teman teman bisa menyesuaikan ssid yang kalian inginkan

  Country : Indonesia, Sesuaikan saja dengan negara teman-teman karna kita cinta tanah air maka saya memilih Indonesia

  Wifi Password : Password wifi teman-teman, ga usah di jelasin lah yaa :) ini adalah password wifi teman-teman jika kalian ingin menambahkan keamanan pada wifi teman-teman. Fitur hide, kalian bisa  hapus centangnya dengan cara di klik pada bagian kotaknya agar kalian bisa melihat password wifi yang kalian ketik

7. Setting pada bagian ini

   <img width="603" height="417" alt="Screenshot 2026-07-31 150129" src="https://github.com/user-attachments/assets/77aa6362-b3ea-4265-a1fc-99245fa5ea78" />

-Klik pada bagian automatic, karna kita ingin mengkonfigurasinya dengan dynamic

-pada bagian local host masukan ip AP yang ada di topologi

-centang pada bagian dhcp server, agar quick set dapat membuat sendiri dhcp servernya sendiri untuk mode Acsess Point

-centang pada bagian Nat, agar quick set dapat membuat firewall NAT-nya sendiri.

-klik Apply lalu Ok

8. Cek Wifi teman-teman, lalu koneksikan. Jangan lupa masukan password wifi yang sudah kalian buat

   <img width="379" height="433" alt="Screenshot 2026-07-31 145927" src="https://github.com/user-attachments/assets/243aae84-dd74-4c19-ae20-9049c0e82317" />

9. Teman-teman bisa cek koneksi internetnya dengan cara ping 8.8.8.8 atau google.com pada CMD.

    <img width="445" height="137" alt="Screenshot 2026-07-31 150934" src="https://github.com/user-attachments/assets/2666fa22-a8af-4d93-b6a6-6a93ceebcbc9" />

    <img width="479" height="138" alt="Screenshot 2026-07-31 151002" src="https://github.com/user-attachments/assets/2d833677-e02e-476d-b398-549f1c3af071" />

    di sini saya cek ping ke gateway-nya (penasaran aja sih :v)

10. Dan itu adalah cara menggunakan menggunakan Quick Set mode Home AP Dynamic

# Praktek




   
