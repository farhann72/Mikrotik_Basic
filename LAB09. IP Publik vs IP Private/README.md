# Mengenal Ip Publik Dan Private

Assalamualaikum Wr.Wb

Pada LAB kali ini kita akan materi dan teoritis terlebih dahulu okee?

# Ip Public
IP Public adalah alamat IP yang dapat diakses melalui internet dan bersifat unik di seluruh dunia.
IP Public diberikan oleh Internet Service Provider (ISP) seperti IndiHome, Biznet, MyRepublic, dan lainnya.

-Kasarnya ip public ini yang kita butuhkan agar kita dapat mengakses internet luar, dan juga ip ini tidak mungkin sama antar satu dengan lainnya.

<h2> Kriterianya </h2>

-Dapat di akses dari internet

-Bersifat unik (tidak boleh ada yang sama di seluruh dunia)

-Biasa digunakan untuk mengkases internet luar

<h2> Contoh IP </h2>

-8.8.8.8

-1.1.1.1

-103.28.16.1

-122.123.54.1

# Ip Private

Ip private adalah alamat ip yang digunakan pada jaringa lokal, dan tidak dapat di akses lewat internet. Ipnya dapat digunakan berulang
di jaringan yang berbeda, dan juga ip private ini biasanya digunakan untuk komunikasi antar perangkat di rumah, sekolah, ataupun kantor.
Ip ini juga lah yang sering kita temui di perangkat-perangkat handphone maupun laptop yang terhubung ke router rumahan/wifi, dan juga
sebelum teman-teman terhubung ke dunia internet luar teman-teman pasti akan melalui hope jaringan lokal terlebih dahulu, yang 
sudah di rancang atau di konfig oleh admin server/router server.

<h2> Kriteria </h2>

-Hanya berlaku di jaringan lokal

-Bisa digunakan berulang di jaringan yang berbeda

-Biasanya teman-teman dapat ipnya otomatis dari dhcp router

# Rentang Ip Private & Publik

Kang ko gada contoh dari ip private sihh?

Di sini saya akan sedikit bahas tentang kelas/class ip terlebih dahulu agar, saya akan memberikan pemahaman maksimal yang saya pahami okee?

Ada 5 kelas ip yang ada jaringan, tetapi yang sering sekali digunakan itu adalah kelas A, B, dan C.

kang ko di beda-bedain sih kelasnya? setiap kelas dapat menampung client yang berbeda-beda, secara default

-kelas a : /8 = 16.777.214 host (cocok untuk jaringan ISP,Perusahaan besar. Jaringan yang dapat melayani banyak di berbagai daerah)

-kelas b : /16 = 65.534 host (cocok untuk jaringan seluas kapus, sekolah, perushaan std)

-kelas c : /24 = 254 host (cocok untuk jaringan yang berskala kecil, beberapa perangkat dan router dalam satu kantor/lab sekolah.

tetapi class A,B, dan C digunakan untuk mengenalkan sejarah pemabgian ip address, di jaringan modern seperti sekarang ini para admin server lebih sering menggunakan CIDR (Classless Inter domain Routing) atau yang sering saya sebut denga prefix atau tanda slash (/).

# Range Ip Private

-kelas a : 10.0.0.0 - 10.255.255.255

-kelas b : 172.16.0.0 - 172.31.255.255

-kelas c : 192.168.0.0 - 192.168.255.255

Penting : jika kalian mendapatkan ip yang lebih dari range di atas ntah itu kelas a,b, dan c. Berarti ip tersebut ip publik, tips ini juga yang bisa teman-teman terapkan untuk membedakan ip private dan publik

Note : Sedikit melebihkan batasan pembahasan, saya hanya ingin menjelaskan sedikit kelas setiap ip, mungkin di next lab saya bisa membahas full tentang ip, dan perhitungan subnetting pada alamat ip.
Dann jika teman-teman kurang paham dan puas dengan pembahasan kelas ip, bisa cari sedikit-sedikit pembahasannya di internet, dan juga teman-teman bisa mengkoreksi kesalahan tentang saya menjelaskan.

intinya materi ini saya hanya ingin mengenalkan Ip public + private dan range dari ip privatenya


# Kesimpulan

Ip public adalah ip yang digunkan untuk mengakses internet dan bersifat unik, juga dapat di akses lewat internet

Ip private adalah ip yang digunakan lokal untuk membuat jaringan lokal kita sendiri, juga tidak dapat di akses lewat internet luar

kedua ip ini saling berhubungan, karna dalam pengaplikasiannya ip private ini yang nantinya juga bakal keluar ke internet menggunakan ip publik dengan cara menyamar/masquerade. Jika jaringan lokal kita tidak memiliki akses ke ip public tentu saja jaringan lokal kita tidak dapat menembus ke jarigan luar/internet 
