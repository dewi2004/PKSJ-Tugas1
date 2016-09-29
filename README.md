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
•	Hydraadalahsebuah software yang dikembangkanolehsebuahorganisasibernama"The Hacker's Choice" (THC) yang menggunakan brute force dan dictionary attack untukmenguji  password yang lemahatau password sederhana. Iadirancangsebagaibuktiuntukmenunjukkankemudahan cracking password karena password yang dipilihburuk. Proyekinimendukungberbagailayanandanprotokol: AFP, TELNET, FTP, HTTP, HTTPS, SMB, MS-SQL, MySQL, REXEC, RSH, rlogin, CVS, SNMP, SOCKS5, VNC, POP3, IMAP, NNTP, NCP, PCNFS, ICQ, Cisco dan lain-lain.
•	Patatoradalahtool mutigunauntukmelakukan brute force yang ditulismenggunakanbahasa python, dengandesain yang modular danpenggunaan yang fleksibel. Disebutmultiguna, karenasudahterdapatberagammodulobjekuntukmelakukan brute force. Selainitu, dapat di modifikasidanditulisulangsesuailingkungan yang digunakan. Patatormenggunakanlisensi GPLv2.
•	Fail2Banadalahsalahsatu software open source sebagai intrusion prevention sistem yang dikembangkanmenggunakanbahasapemprogramam python. Fail2ban digunakanuntukmelakukan monitoring terhadapa log sistemseperti /var/logl/pwdfail, /var/log/auth.log, /var/logl/secure, danlainnya. Fail2ban bisajugadigunakanuntukmencegah IP Address tertentu yang digunakanuntukaksesmasukkesistermsetelahbeberapa kali percobaanmenggunakan password yang keliru, halinikarena fail2ban menggunakaniptablesuntukmelakukan banned terhadapkegagalanakses. Fail2ban tidakhanyasebataspadaaplikasi SSH sepertiDenyhosts, melainkanterhadapsemuaaplikasi yang menggukananprotokol TCP, sepertiaplikasi SMTP, HTTP, danlainnya.
3. UJI PENETRASI 1
A.	Installing Ubuntu 
1.	Klik “New” padaVirtualBox
i.	 

2.	MemasukkanNama, Type,danVersi

i.	 

3.	MasukkanNilai RAM yang dibutuhkan

i.	 

4.	Pilih “Create a virtual harddisk now”

i.	 

5.	Pilih “Virtual Disk Image”

i.	 

6.	Pilih “Dynamic allocated”

i.	 

7.	Masukkan size unutk virtual harddiskdalam megabytes

i.	 

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
