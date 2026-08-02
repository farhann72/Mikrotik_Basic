# LAB 12. Router OS services atau Layanan Router OS

Assalamualaikum Wr.Wb

Teman-teman aneh ga sih ko bisa meremote mikrotik dengan gampang dan mudah? pernah ga sih ke pikiran kalo ada orang asing yang bisa masuk sembarangan?

# Router OS Services / Layanan Router Os / Ip Services

Adalah sebuah layanan yang memberikan akses pada pengguna agar dapat meremote mikrotik dengan mudah, pada dasarnya fitur ini memberi pengguna beberapa opsi untuk dapat meremote mikrotik dari berbagai service, tentu saja setiap service memiiki port default masing-masing. Terus keamanannya bagaimana? di fitur ini admin bisa merubah port dan disable/mematikan service yang kita inginkan untuk alasan security atau keamanan, jika teman-teman mau mikrotik kalian hanya bisa di remote oleh 1 service bisa kok, kalian tinggal matikan semua service yang menyala lalu tinggalkan service yang kalian inginkan agar tetap menyala.

# Port Default Setiap Service

1. Remote mikrotik teman-teman seperti biasa

2. Buka pada bagian **Ip>>Services**

<img width="290" height="436" alt="Screenshot 2026-08-02 140827" src="https://github.com/user-attachments/assets/981caa8f-8497-472b-9669-a4c4328d9cf9" />

3. Kalian dapat melihat semua service yang di beri mikrotik dan port defaultnya

<img width="1015" height="254" alt="Screenshot 2026-08-02 141031" src="https://github.com/user-attachments/assets/91ee160e-8ba1-49ed-b388-7a21b0a4e16e" />

4.  Fungsi dari setiap service

   ## RouterOS Services

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
