# LAB 12. Router OS services atau Layanan Router OS

Assalamualaikum Wr.Wb

Teman-teman aneh ga sih ko bisa meremote mikrotik dengan gampang dan mudah? pernah ga sih ke pikiran kalo ada orang asing yang bisa masuk sembarangan?

<h3> Router OS Services / Layanan Router Os / Ip Services </h3>

Adalah sebuah layanan yang memberikan akses pada pengguna agar dapat meremote mikrotik dengan mudah, pada dasarnya fitur ini memberi pengguna beberapa opsi untuk dapat meremote mikrotik dari berbagai service, tentu saja setiap service memiiki port default masing-masing. Terus keamanannya bagaimana? di fitur ini admin bisa merubah port dan disable/mematikan service yang kita inginkan untuk alasan security atau keamanan, jika teman-teman mau mikrotik kalian hanya bisa di remote oleh 1 service bisa kok, kalian tinggal matikan semua service yang menyala lalu tinggalkan service yang kalian inginkan agar tetap menyala.

<h3> Port Default Setiap Service </h3>

1. Remote mikrotik teman-teman seperti biasa

2. Buka pada bagian **Ip>>Services**

<img width="290" height="436" alt="Screenshot 2026-08-02 140827" src="https://github.com/user-attachments/assets/981caa8f-8497-472b-9669-a4c4328d9cf9" />

3. Kalian dapat melihat semua service yang di beri mikrotik dan port defaultnya

<img width="1015" height="254" alt="Screenshot 2026-08-02 141031" src="https://github.com/user-attachments/assets/91ee160e-8ba1-49ed-b388-7a21b0a4e16e" />

4.  Fungsi dari setiap service

   RouterOS Services

| Service | Protokol | Port Default | Fungsi |
|---------|----------|--------------|--------|
| Winbox | TCP | 8291 | Mengelola router menggunakan aplikasi Winbox. |
| SSH | TCP | 22 | Mengakses router melalui Command Line Interface (CLI) dengan koneksi terenkripsi. |
| Telnet | TCP | 23 | Mengakses router melalui Command Line Interface (CLI) tanpa enkripsi. |
| HTTP | TCP | 80 | Mengakses WebFig (antarmuka web RouterOS) melalui browser tanpa enkripsi. |
| HTTPS | TCP | 443 | Mengakses WebFig melalui browser dengan koneksi terenkripsi (SSL/TLS). |
| FTP | TCP | 21 | Mengirim dan mengambil file dari router. |
| API | TCP | 8728 | Memungkinkan aplikasi pihak ketiga berkomunikasi dan mengelola RouterOS melalui API. |
| API-SSL | TCP | 8729 | API dengan koneksi terenkripsi menggunakan SSL/TLS. |

<h3> Cara Merubah Port & Mematikan Service </h3>

1. Pastikan kalian masih di menu **Ip>>Service**

   a. Cara Merubah Port

   <img width="658" height="321" alt="Screenshot 2026-08-02 142413" src="https://github.com/user-attachments/assets/5c8a6ec8-64e0-4c39-844d-4597c52d034e" />

   Klik pada service yang ingin di ganti portnya, sebagai contoh saya pilih service ftp, ubah pada bagian port, **range port 1 - 65535** dengan ketentuan tidak boleh sama dengan service yang lain. Lalu klik Apply + Ok

   b. Cara Mematikan/Disable Service

   <img width="493" height="287" alt="Screenshot 2026-08-02 142806" src="https://github.com/user-attachments/assets/15a8d2e6-df8b-4ea4-bd43-d156d4874d2d" />

   Klik pada service yang ingin di matikan, lalu klik gambar X atau disable yang sudah di beri tanda

   <img width="350" height="239" alt="Screenshot 2026-08-02 142830" src="https://github.com/user-attachments/assets/172d90aa-878f-4d8b-ad8f-c8032902253b" />

   Perhatikan Service yang di matikan akan berubah menjadi abu-abu dan tanda hijau pun ikut menghilang, itu berarti service tersebut tidak dapat di akses di mikrotik kita

2. Percobaan

   Teman-teman bisa mencoba untuk meremote service yang sudah di matikan

   a. Jika mikrotik teman-teman dalam kondisi blank konfigurasi bisa langsung kalian tambah ip **Ip>>Address**, masukan ipnya **192.168.10.1**. ip ini untuk percobaan remote via ssh

   b. Buka putty teman-teman

   <img width="459" height="448" alt="Screenshot 2026-08-02 143708" src="https://github.com/user-attachments/assets/150f135f-0a5e-4e92-83d5-95d44efd2b62" />

   masukan ip yang sudah kita setting tadi, pilih ssh dan perhatikan portnya juga. lalu klik Open

   <img width="668" height="423" alt="Screenshot 2026-08-02 143729" src="https://github.com/user-attachments/assets/4e2d5f95-ac3a-45cd-bbcd-ea696a2cb93c" />

   Pasti akan eror seperti ini, maka kalian sukses mematikan servicenya

3. Untuk memastikan apakah ini work atau tidak, teman-teman bisa menyalakan kembali service lalu pastikan hijau pada servicenya, setelah itu coba kalian remote kembali

   <img width="669" height="337" alt="Screenshot 2026-08-02 144247" src="https://github.com/user-attachments/assets/0d2c35ba-46f2-47a8-ac67-28d7c811c576" />

# Kesimpulan

Router Os Service ini memberikan kita banyak opsi untuk meremote dengan memberikan beberapa service, terlihat memudahkan para admin untuk meremote bukan?? maka dari itu agar mencegah orang yang ingin jail, kalian bisa merubah port bahkan mematikan service yang kalian inginkan. Merubah port juga tidak sembarangan ada rangenya mulai dari 1 - 65535 dengan aturan tidak boleh sama dengan port yang lain. Mungkin sudah jelas lah yaww >< 

Akhir Kata 

Wassalamualaikum Wr.Wb


