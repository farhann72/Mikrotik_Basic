# LAB16. Lisensi Router Os

Assalamualaikum Wr.wb

Pada kali ini saya akan memberi tahu lisensi router os pada mikrotik

# Apa itu Lisensi Router Os??

Secara sederhana, Lisensi RouterOS ini adalah hak izin digital yang menentukan kapasitas dan batas maksimal operasional dari router kita. Sistem lisensi ini sifatnya sekali bayar untuk seumur hidup, jadi tidak ada biaya langganan bulanan. Menariknya, lisensi ini tidak membatasi fitur artinya semua fitur MikroTik itu lengkap di setiap level yang dibatasi hanyalah skala jumlah pengguna dan jumlah koneksi yang bisa aktif secara bersamaan.

Yaa intinya sistemnya kaya langganan sebuah aplikasi, jika kita ingin membuka fitur premium kita harus membayarnya, tetapi dengan sekali bayar kita dapat menikmati semua fiturnya

# Tabel Lisensi

<img width="871" height="470" alt="Screenshot 2026-08-03 195339" src="https://github.com/user-attachments/assets/db34cb71-6116-476d-b938-66f29cde8d1e" />

Teman-teman perhatikan saja tabel di atas

1. Level 0 (Trial Mode)

   Ketentuan: Gratis

   Akses & Batasan: Membuka seluruh fitur RouterOS secara penuh tanpa batasan fungsi. Namun, penggunaannya dibatasi waktu selama 24 jam total waktu operasional router. Setelah 24 jam, sistem akan terkunci dan Anda harus memasukkan lisensi resmi untuk menggunakannya kembali.

3. Level 1 (Free Demo)

    Ketentuan: Gratis, didapatkan dengan mendaftar akun di situs resmi MikroTik.

   Akses & Batasan: Masa aktifnya tidak terbatas (unlimited). Namun, fungsi jaringannya sangat dibatasi dan hanya untuk uji coba standar:Sebagian besar fungsi tunnel (EoIP, PPPoE, PPTP, L2TP, OVPN), VLAN, dan antrean (Queues) dibatasi maksimal hanya 1 jalur/pengaturan saja.Pengguna aktif HotSpot dibatasi maksimal 1 user.Tidak mendukung fitur Wireless Access Point (AP).

3. Level 3

    Ketentuan: Berbayar, namun biasanya sudah terpasang langsung pada perangkat MikroTik tipe CPE (Customer Premises Equipment) atau perangkat penerima. Lisensi ini tidak dijual secara terpisah untuk instalasi PC.

    Akses & Batasan:

   Wireless AP: Tidak mendukung mode Access Point standar (tidak bisa memancarkan Wi-Fi ke banyak perangkat sekaligus). Hanya mendukung mode Wireless Client/Bridge (menerima sinyal) atau Point-to-Point terbatas.

   Kapasitas: Mendukung hingga 200 pengguna simultan untuk jalur tunnel PPPoE, PPTP, L2TP, dan OVPN.

   HotSpot: Dibatasi hanya 1 pengguna aktif.

    Fitur Bebas: EoIP, VLAN, Routing (RIP, OSPF, BGP) sudah bersifat unlimited.

4. Level 4

   Ketentuan: Berbayar dan merupakan standar minimum untuk penyedia layanan internet (WISP) skala kecil.

   Akses & Batasan:

   Wireless AP: Sudah mendukung penuh mode Access Point (Yes) untuk memancarkan Wi-Fi ke banyak klien perangkat.

   Kapasitas: Mendukung hingga 200 pengguna aktif secara bersamaan untuk HotSpot, PPPoE, PPTP, L2TP, dan OVPN.

   Fitur Bebas: Queues (manajemen bandwidth) dan fungsi interkoneksi lainnya sudah unlimited

5. Level 5

   Ketentuan: Berbayar, dirancang untuk jaringan dengan kapasitas distribusi yang lebih padat.

   Akses & Batasan:Memiliki semua kemampuan penuh di Level 4 dengan peningkatan jumlah batas tampung jaringan.

   Kapasitas: Jumlah pengguna aktif untuk PPPoE, PPTP, L2TP, dan HotSpot ditingkatkan menjadi 500 pengguna simultan.

   OVPN: Khusus untuk tunnel OpenVPN (OVPN) sudah berstatus unlimited.

6. Level 6

   Ketentuan: Berbayar, Level lisensi tertinggi dan terlengkap di ekosistem MikroTik.

   Akses & Batasan:Sama sekali tidak memiliki batasan (Unlimited) untuk semua fitur operasional.

   Seluruh jenis tunnel VPN, VLAN interfaces, akun HotSpot aktif, hingga sesi Usermanager dapat dikonfigurasi sebanyak mungkin tanpa batasan sistem. Cocok digunakan sebagai pusat pengendali utama (Controller) pada jaringan skala besar atau korporat.

   Harusnya kalian paham lah yaa, intinya setiap mikrotik teman-teman memiliki lisensi yang berbeda-beda dan juga fitur yang dapat digunakannya juga beda-beda pula.

# Cara Melihat Lisensi Router Os

1. Remote mikrotik menggunakan winbox

2. Buka pada bagian **System>>License** (GUI)

   <img width="278" height="152" alt="Screenshot 2026-08-03 202228" src="https://github.com/user-attachments/assets/f78cc5b9-290a-494b-a2ef-25497f131d5f" />

   <img width="371" height="198" alt="Screenshot 2026-08-03 202331" src="https://github.com/user-attachments/assets/65ea14cf-c5cc-4b82-bdd2-c498c0d3a568" />

3. Buka pada bagian new terminal, ketikan **System/License/print** lalu enter (CLI)

<img width="305" height="97" alt="Screenshot 2026-08-03 202627" src="https://github.com/user-attachments/assets/9a75b1ab-42f9-498b-9a6f-9fdde50f16c6" />

# RouterOS License

• Lisensi bersifat lifetime, tidak ada batasan masa aktif dan kewajiban update lisensi berkala

• Tersedia lisensi gratis yang dapat digunakan untuk pengecekan kesesuaian hardware

• Level 0 (trial) – batas masa aktif 24 jam, tidak ada batasan fitur

• Level 1 (demo) – tidak terdapat batasan masa aktif, terdapat batasan pembuatan rule

• Tidak ada batasan interface pada semua lisensi/unlimited interfaces

• Upgrade versi RouterOS bisa dilakukan secara gratis tanpa ada batasan

# Kesimpulan

Materi kali ini hanya seputar lisensi router os mikrotik, dan penjelasan lv lisensinya. Yang harus kalian tahu lv 6 adalah lv terakhir dari lisensi dan juga pasti mendapatkan semua fitur mikrotik tanpa ada batasan penggunaan

Akhir Kata

Wassalamualaikum Wr.Wb
