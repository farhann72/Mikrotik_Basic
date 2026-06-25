LAB 1
Logging in  ke mikrotik

 
Lakukan logging in ke mikrotik dengan beberapa  cara : 
Tuliskan langkah-langkah nya :
1.	Winbox
Cara Pertama yang paling mudah menurut saya adalah menggunakan aplikasi winbox yang dapat didownload di mikrotik.com, berikut langkah nya
a.	Buka Winbox, 
 
b.	Klik Tab Neighbors >> Refresh
c.	Setelah muncul , pilih MAC Address >> MAC Address: 64:D1:54:0F:07:3F
d.	Login: admin
Password:
e.	Klik Connect
 

f.	Setelah berhasil login, maka akan muncul tampilan mikrotik pada winbox
 



2.	WebFig
Cara kedua menggunakan webfig  (menggunakan web browser), berikut ini langkah nya
a.	Buka chrome (aplikasi web browser)
 
b.	Pada URL ketik IP Address: 192.168.88.1 (ip default mikrotik)
c.	Login: admin
Password:
d.	Klik Login atau Tekan Enter
 

e.	Setelah berhasil login, maka akan muncul tampilan mikrotik dalam mode GUI pada web browser
 


3.	Telnet
Cara ketiga menggunakan telnet pada  aplikasi putty, berikut ini langkah nya
a.	Buka putty
 
b.	Klik Tab Telnet 
c.	Ketik IP Address: 192.168.88.1 (ip default mikrotik)
d.	Ketik Port: 23 (port default telnet)
e.	Klik Open atau Tekan Enter
 

f.	Login: admin
Password:
Tekan Enter
 

g.	Setelah berhasil login, maka akan muncul tampilan mikrotik dalam mode CLI
 


4.	SSH
Cara keempat menggunakan SSH pada  aplikasi putty, berikut ini langkah nya
a.	Buka putty
 
b.	Klik Tab SSH 
c.	Ketik IP Address: 192.168.88.1 (ip default mikrotik)
d.	Ketik Port: 23 (port default telnet)
e.	Klik Open atau Tekan Enter
 

f.	Login: admin
Tekan Enter  

g.	Setelah berhasil login, maka akan muncul tampilan mikrotik dalam mode CLI
 


5.	FTP (filezilla)
Akses mikrotik via FTP (filezilla) bermanfaat untuk upload dan download file ke router mikrotik.
a.	Buka filezilla
 
b.	Isi Host: 192.168.88.1 (ip default mikrotik)
c.	Login: admin
d.	Password:
e.	Ketik Port: 21 (port default ftp)
f.	Klik Quickconnect
 

g.	Setelah berhasil login, maka akan muncul tampilan mikrotik dalam mode CLI
 

6.	Console
Akses mikrotik via console belum penulis lab kan, sambil menanti perangkat mikrotik yang ada port console nya.

7.	Tik App
Akses mikrotik via console belum penulis lab kan, sambil menanti perangkat smartphone android, karena Tik App yang rilis 2015 baru support OS Android.


Buat  kesimpulan : 

Ada 7 cara koneksi / akses/ remote / logging in ke dalam mikrotik, dengan berbagai manfaat dan karakteristik yang berbeda,
Hal ini sangat memudahkan admin untuk mengakses mikrotik, dengan pilihan yang bervariasi.
Kita dapat memilih akses mikrotik sesuaikan dengan kebutuhan.
