<img width="890" height="492" alt="image" src="https://github.com/user-attachments/assets/3ef630de-1aa0-43bc-adad-1116acab5cfd" />

<br>

Assalamualaikum Wr. Wb

Kali ini saya akan membagikan materi "Cara Mengkoneksikan Mikrotik Ke Internet", tentu saja sampai laptop teman-teman dapat mengakses internet. Langsung saja kita Lab, sebelum itu koneksikan mikrotik teman-teman menggunakan kabel lan/RJ45 sesuai topologi di atas.

<h1> Koneksikan Mikrotik Ke Internet DHCP (otomatis) </h1>

1. Remote mikrotik teman-teman menggunakan WinBox

2. Buka IP >> DHCP Client

<img width="308" height="336" alt="Screenshot 2026-06-27 090705" src="https://github.com/user-attachments/assets/dafcdf0e-ecad-44ed-8d29-3d6209e04ad5" />


3. Klik (+)

   -Arahkan interfacenya ke ether1

   -Centang Use Peer DNS
   
   Ini berfungsi agar kita mendapatkan DNS secara otomatis dari ISP (sumber internet)

   -Centang Use Peer NTP

    Ini berfungsi agar perangkat router atau komputer secara otomatis menerima dan menyinkronkan pengaturan waktu dari server NTP (Network Time Protocol) yang diberikan oleh ISP

   -Klik Aplly, lalu Ok

   <img width="673" height="340" alt="Screenshot 2026-06-27 090855" src="https://github.com/user-attachments/assets/8b0ef82d-279a-455b-9136-36d077269418" />

   -Pastikan statusnya sudah bound

   <img width="494" height="404" alt="Screenshot 2026-06-27 091824" src="https://github.com/user-attachments/assets/1f20cc09-a176-4e1e-ae89-d6ff455a6d81" />

4. Teman-teman boleh mecatat terlebih dahulu Ip yang keluar

   <img width="531" height="353" alt="image" src="https://github.com/user-attachments/assets/aa218753-d37e-4b66-91b1-5c720de67131" />

5. Selanjutnya kita buat ip gateway (UNTUK LAPTOP KITA)

   -Klik Ip >> Address

<img width="267" height="280" alt="Screenshot 2026-06-27 092415" src="https://github.com/user-attachments/assets/43a2991d-21ef-4409-a75a-ab55017e8421" />


   -Klik tanda (+)

   -Tambahkan Ipnya 192.168.10.1/24

   -Arahkan Interfacenya ke ether2

   -Klik Aplly lalu Ok

   <img width="466" height="166" alt="Screenshot 2026-06-27 092539" src="https://github.com/user-attachments/assets/0402bdf5-e577-4cfb-bd0d-29f7f6d15b15" />

   Kita sudah punya ip gateway (UNTUK LAPOP KITA) yakni 192.168.10.1

6. Kita setting firewall NAT

     -Klik Ip >> Firewall >> NAT

     <img width="533" height="216" alt="Screenshot 2026-06-27 093028" src="https://github.com/user-attachments/assets/e0fc3195-af87-476f-939b-413fdf3e1c98" />

     -Klik (+) lalu chain=srcnat out-interfaceny=ether1

     <img width="426" height="349" alt="Screenshot 2026-06-27 093145" src="https://github.com/user-attachments/assets/f31f53c9-52cd-44e9-bb37-d66ce9534037" />

     -Klik bagian action lalu pilih masquerade, klik Aplly dan Ok

     <img width="407" height="168" alt="Screenshot 2026-06-27 093229" src="https://github.com/user-attachments/assets/7ebd7948-5fbd-4e99-8272-ba9dc3d53f69" />

7. Setting Ip teman-teman menggunakan Control Panel

   -Klik Ctrl + R mengeluarkan tab run lalu ketikan control panel & klik Ok

   -Klik bagian Network And Internet

   <img width="1150" height="679" alt="Screenshot 2026-06-27 093936" src="https://github.com/user-attachments/assets/e4156314-6066-49f7-8917-054a426b3ab1" />

   -Klik Network And Sharing Center

   <img width="509" height="131" alt="Screenshot 2026-06-27 094251" src="https://github.com/user-attachments/assets/74f6a6b9-b0ee-4432-9aaf-78ce995687a8" />

   -Klik Change Adapter Setting

   <img width="247" height="149" alt="Screenshot 2026-06-27 094739" src="https://github.com/user-attachments/assets/9303ca0e-ebff-4a33-b8c3-8203e7e83ada" />

   -Doble klik Adapter Kabel LAN teman-teman, pilih properties, pilih internet protocol version 4

   <img width="741" height="491" alt="Screenshot 2026-06-27 094504" src="https://github.com/user-attachments/assets/61cf3eb4-2236-425f-ad5b-8fd8fdddf23c" />

   -Isikan sesuai dengan foto lalu klik Ok

   <img width="406" height="459" alt="Screenshot 2026-06-27 095150" src="https://github.com/user-attachments/assets/be3e0135-9fda-4311-b9d6-ebdc7cef08d6" />

8. Cek koneksi internet dengan ping google.com lewat cmd teman-teman, bila sudah replay berarti laptop dan mikrotik teman-teman sudah mendaptakan internet, teman-teman juga bisa coba ping lewat mikrotik teman-teman, dengan cara buka Winbox >> New Terminal >> ping google.com

   <img width="569" height="297" alt="Screenshot 2026-06-27 095544" src="https://github.com/user-attachments/assets/a26074c9-b26d-4a69-b241-0e8e160cacad" />

   PIng lewat CMD

   <img width="598" height="195" alt="Screenshot 2026-06-27 095902" src="https://github.com/user-attachments/assets/59533ca6-8985-410d-b5eb-913aef681295" />

   Ping lewat Mikrotik



   


