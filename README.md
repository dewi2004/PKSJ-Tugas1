# PKSJ-Tugas1


Tugas 1 PKSJ - Ganjil 2016/2017

Pendahuluan


Tugas 1 adalah tugas pertama yang harus di selesaikan sebagai salah satu syarat penilaian pada matakuliah Perancangan Keamanan & Sistem Jaringan (PKSJ) Semester Ganjil 2016/2017, TeknikInformatika ITS, Surabaya


AnggotaKelompok

•	Dewi Kartika 	5113100008

•	M.Sholaudin	5112100075

•	FauzanAdim	5113100101

Penjelasan

Ujipenetrasi1 :


•	Instalsebuah virtual OS dengan Ubuntu server

•	Instal SSH server dengankonfigurasi default

•	Instalsatulagi virtual OS dengan OS bebas, misalnya Kali Linux atau Ubuntu Desktop

•	Pastikan tools untuk SSH brute force attack sudahterinstal

•	Lakukanujipenetrasi 1: dengan THC-Hydra atauNcrackdancatathasilujipenetrasi


Ujipenetrasi 2:

•	Instal fail2ban pada Ubuntu server yang telahdiinstal SSH servernya

•	Konfigurasilah SSH server agar tidak default lagi

•	Lakukan uji penetrasi 2 dengan tools yang sama dancatat hasilnya

DasarTeori

1. OS yang digunakan


•	Ubuntu Server adalah salah satu varian dari distro linux Ubuntu. Dalam pembahasan kali ini dan pembahasan selanjutnya, saya akan membahas tentang perintah CLI di Linux  dan seting server menggunakan ubuntu 12.10. Namun sebelum membahas lebih jauh tentang Ubuntu server akan saya kenalkan dulu apa itu ubuntu server dalam format FAQ sehingga lebih mudah di pahami.


•	Kali Linux adalah distribusi berlandasan distribusi Debian GNU/Linux untuktujuanforensik digital dan di gunakan untuk pengujian penetrasi, yang dipelihara dan didanai oleh Offensive Security. Kali juga dikembangkan oleh Offensive Security sebagai penerus BackTrack Linux. Salah satu distribusi Linux tingkat lanjut untuk Penetration Testingdan audit keamanan. Distroinidulunyaadalahdistro Backtrack, yang kemudian memutuskan mengganti nama distronya tersebut menjadi Kali Linux di versi terbarunya. Kali Linux ini akan dijadikan sebagai standarisasi distro Linux yang digunakan untuk percobaan penetrasi.

2. Tools yang digunakan


•	Hydraadalahsebuah software yang dikembangkan oleh sebuah organisasi bernama "The Hacker's Choice" (THC) yang menggunakan brute force dan dictionary attack untuk menguji  password yang lemahatau password sederhana. Ia di rancang sebagai bukti untuk menunjukkan kemudahan cracking password karena password yang dipilihburuk. Proyek ini mendukung berbagai layanan dan protokol: AFP, TELNET, FTP, HTTP, HTTPS, SMB, MS-SQL, MySQL, REXEC, RSH, rlogin, CVS, SNMP, SOCKS5, VNC, POP3, IMAP, NNTP, NCP, PCNFS, ICQ, Cisco dan lain-lain.


•	Patator adalah tool multiguna untuk melakukan brute force yang ditulis menggunakan bahasa python, dengan desain yang modular danpenggunaan yang fleksibel. Disebutmultiguna, karena sudah terdapat beragam modul objek untuk melakukan brute force. Selain itu, dapat di modifikasi dan ditulis ulang sesuai lingkungan yang digunakan. Patator menggunakan lisensi GPLv2.


•	Fail2Ban adalah salah satu software open source sebagai intrusion prevention sistem yang dikembangkan menggunakan bahasa pemprogramam python. Fail2ban digunakan untuk melakukan monitoring terhadap log sistem seperti /var/logl/pwdfail, /var/log/auth.log, /var/logl/secure, dan lainnya. Fail2ban bisa juga digunakan untuk mencegah IP Address tertentu yang digunakan untuk akses masuk ke sisterm setelah beberapa kali percobaan menggunakan password yang keliru, hal ini karena fail2ban menggunakan iptables untuk melakukan banned terhadap kegagalan akses. Fail2ban tidak hanya sebatas pada aplikasi SSH seperti Denyhosts, melainkan terhadap semua aplikasi yang menggunakan protokol TCP, seperti aplikasi SMTP, HTTP, dan lainnya.


3. UJI PENETRASI 1

A.	Installing Ubuntu 

1.	Klik “New” padaVirtualBox
	 

2.	MemasukkanNama, Type,danVersi

	 

3.	MasukkanNilai RAM yang dibutuhkan

	 

4.	Pilih “Create a virtual harddisk now”

 

5.	Pilih “Virtual Disk Image”

	 

6.	Pilih “Dynamic allocated”

	 

7.	Masukkan size unutk virtual harddiskdalam megabytes

	 

8.	Klik Create

B. Installing Kali Linux

a.	Klik “New”

 

b.	MemasukkanNama, Type,danVersi

 

c.	MasukkanNilai RAM yang dibutuhkan

 

d.	Pilih “Create a virtual harddisk now”

 

e.	Pilih “Virtual Machine Disk ”

 

f.	Pilih “Dynamic allocated”

 

g.	Masukkan size unutk virtual harddiskdalam megabytes
 
h.	Klik Create
i.	

C. Installing SSH Server

a)	
