# LAB14. Export dan Import Pada Mikrotik 

<img width="836" height="383" alt="image" src="https://github.com/user-attachments/assets/86c4b1f3-9e19-4fcc-9021-67943adf06ce" />

Assalamualaikum Wr.Wb

<h3> Export </h3>

Langsung aja lah yaa? Materi kali ini mengenai export dan import, sama seperti backup, export adalah proses menyimpan konfigurasi dari mikrotik dengan file berformat **.rsc** dengan file yang berisi cli, jadi dapat di edit dan di ubah oleh software text editor. Bedanya dari backup, export lebih flexible karna bisa menyimpan konfigurasi yang yang kita inginkan

contoh: kita hanya ingin menyimpan konfigurasi ip address, tanpa menyimpan seluruh konfigurasi yang lain, export bisa melakukan hal tersebut

Ngerti lah yaa? intinya menyimpan konfigurasi dengan format .rsc yang basicnya cli, dan dapat menyimpan konfigurasi yang kita inginkan, dan juga tidak dapat mmenyimpan password username dan password router


<h3> Import </h3>

Kalo restore adaah proses menyimpan kembali konfigurasi dari backup, maka import adalah proses menyimpan kembali konfigurasi dari file export, dengan basic yang sama menggunakan CLI, yang membedakanya pada import kita tidak perlu report-report memasukan password ketika ingin melakukan import karna emag dasarnya export tidak dapat menyimpan password.

Langsung praktik lahh yaa

# Praktek Export & Import (konfigurasi khusus)

1. Remote mikrotik sesuai topologi

2. Buat Sebuah konfigurasi, contoh di sini saya akan membuat konfigurasi ip address saja yang sederhana :), untuk apaa? untuk tes apakah export ini akan work atau tidak

   <img width="350" height="357" alt="Screenshot 2026-08-03 164942" src="https://github.com/user-attachments/assets/64eb9fd2-4390-41f4-813d-636d3e717f0f" />

   Simpan ip pada ether 2 yaa

3. Masuk ke menu New Terminal

   <img width="144" height="156" alt="Screenshot 2026-08-03 170547" src="https://github.com/user-attachments/assets/020c425f-71ba-45e7-8496-c0aeda8b2dc2" />

4. Ketikan **ip address/export file=namafile** lalu klik enter

   <img width="394" height="122" alt="image" src="https://github.com/user-attachments/assets/6a260f3a-0c0b-4f93-ad5f-462fea5fac56" />

5. Simpan File backupnya di folder laptop kalian, ada 2 cara yaitu drag and drop & download (ada pada lab sebelumnya)

   <img width="1119" height="363" alt="Screenshot 2026-08-03 171608" src="https://github.com/user-attachments/assets/ac80b43e-e7ef-4f9c-9922-15f837312669" />

6. Jika kalian penasaran bisa buka file exportnya lewat notepad

   <img width="556" height="122" alt="image" src="https://github.com/user-attachments/assets/1889a4f3-510a-4b47-8007-4ae629f9180e" />

   berbeda dari backup,file export lebih manusiawi dan dapat di baca oleh mata kita :)

7. Reset mikrotik kalian ke blank konfigurasi + do not backup, lalu tunggu mikrotik kembali ke tampilan winbox lagi

   <img width="395" height="163" alt="image" src="https://github.com/user-attachments/assets/0430cfbe-3fad-4737-aa26-6ebcf9866e07" />

8. Sekarang kita coba uploud kembali file export yang berformat .rsc, cara nya masih sama dengan lab sebelumnya

   <img width="672" height="408" alt="Screenshot 2026-08-03 172446" src="https://github.com/user-attachments/assets/4ee5a255-4f86-458c-9a0c-c09456ee1dcd" />


9. Buka kembali new terminal dan ketikan **import file-name=namafile** lalu klik enter

    <img width="411" height="124" alt="image" src="https://github.com/user-attachments/assets/95409b04-8feb-4203-af45-fb564b614f67" />

10. Cek konfigurasi ip yang tadi kalian export

    <img width="408" height="82" alt="Screenshot 2026-08-03 172745" src="https://github.com/user-attachments/assets/228b1c3e-a8c6-4ad5-b136-1eca0abda013" />

    <img width="348" height="169" alt="Screenshot 2026-08-03 172851" src="https://github.com/user-attachments/assets/a4f1bf4d-85ad-468b-9a49-a726f952fbd2" />

11. Sukses kan?? simpel sekali yekann


# Praktik Export & Import (semua konfigurasi)

1. Jika tadi kita hanya backup file khusus/konfigurasi yang kita mau, sekarang kita akan export semua konfigurasi

2. Untuk membuktikan praktik kali ini sukses, coba kalian buat konfigurasi ip addres dan nat terlebih dahulu, karna ip address sudah di buat saya tinggal membuat nat

   <img width="348" height="169" alt="Screenshot 2026-08-03 172851" src="https://github.com/user-attachments/assets/1a18c8a5-d2ac-4ece-8925-cb75d220d90e" />

   <img width="266" height="148" alt="Screenshot 2026-08-03 173509" src="https://github.com/user-attachments/assets/9d3eca71-6482-4b7e-bb8c-751eadf34fd2" />

3. Buka new terminal, ketikan **export file=namaexport**

   <img width="356" height="93" alt="Screenshot 2026-08-03 173624" src="https://github.com/user-attachments/assets/7c60f2f5-8e00-4fb5-977e-98544aace541" />

4. Seperti biasa kalian simpan kembali file yang sudah di export dengan cara drag and drop atau download

  <img width="1007" height="333" alt="Screenshot 2026-08-03 174538" src="https://github.com/user-attachments/assets/80c26ce2-117d-415c-a61e-2a19abf4ee06" />

5. Reset Mikrotik dengan mencentang No default configuration + do not backup

   <img width="395" height="163" alt="Screenshot 2026-08-03 171951" src="https://github.com/user-attachments/assets/66e17be4-2551-4a5d-a434-1c0fa40d3ad7" />

6. Setelah menyala seperti biasa kalian uploud kembali file dari menyimpanan pc kalian

   <img width="671" height="401" alt="Screenshot 2026-08-03 175137" src="https://github.com/user-attachments/assets/01e08f3c-df5b-4fe0-ac08-fa9623339ab1" />

7. Buka new terminal kembali, ketikan **import file-name=namafile** lalu klik enter

    <img width="386" height="117" alt="Screenshot 2026-08-03 175358" src="https://github.com/user-attachments/assets/d5edc0fc-08c7-48f1-927b-69ccbfec597c" />

8. Cek kembali konfigurasi yang tadi di export, ketikan ip address print (enter) dan ip firewall nat print, kalian juga bisa cek lewat gui

   <img width="425" height="125" alt="Screenshot 2026-08-03 175633" src="https://github.com/user-attachments/assets/36455ccf-630c-4e2a-803c-ff92f087c07c" />

   tanda kalau konfig benar-benar terimport

9. Gampang bukan??




# Tips Backup & Export

• Lakukan backup dan export secara berkala, baik secara manual atau otomatis (scheduler)

• Backup hanya direkomendasikan untuk router yang sama

• Untuk router dengan type yang sama atau type yang berbeda, silakan gunakan export

• Simpan file backup atau export di luar router (misal laptop)

• Bisa juga file backup dikirim via email


# Kesimpulan

Mungkin itu sedikit lab yang saya sampaikan, yang membedakan export mungkin flexible dari pada backup. dan juga  dapat di export dan di import di berbeda router maupun versi, dan juga export tidak membawa user dan password dari ketika kita ingin mengembalikan konfigurasinya

Mungkin sudah jelas lahh yaa


Akhir kata

Wassalamualaikum Wr.Wb
 







   







