# PKSJ-Tugas1
Tugas 1 PKSJ - Ganjil 2016/2017
Pendahuluan
Tugas 1 adalahtugaspertama yang harus di selesaikansebagaisalahsatusyaratpenilaianpadamatakuliahPerancanganKeamanan&SistemJaringan (PKSJ) Semester Ganjil 2016/2017, TeknikInformatika ITS, Surabaya
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
•	Lakukanujipenetrasi 2 dengan tools yang samadancatathasilnya
DasarTeori
1. OS yang digunakan
•	Ubuntu Serveradalahsalahsatuvariandaridistrolinux Ubuntu. Dalampembahasan kali inidanpembahasanselanjutnya, sayaakanmembahastentangperintah CLI di Linux  danseting server menggunakanubuntu 12.10. Namunsebelummembahaslebihjauhtentang Ubuntu server akansayakenalkanduluapaituubuntu server dalam format FAQ sehinggalebihmudah di pahami.
•	Kali LinuxadalahdistribusiberlandasandistribusiDebian GNU/Linuxuntuktujuanforensik digital dan di gunakanuntukpengujianpenetrasi, yang dipeliharadandidanaioleh Offensive Security. Kalijugadikembangkanoleh Offensive Security sebagaipenerusBackTrackLinux. Salah satudistribusi Linux tingkatlanjutuntukPenetration Testingdan audit keamanan. Distroinidulunyaadalahdistro Backtrack, yang kemudianmemutuskanmenggantinamadistronyatersebutmenjadi Kali Linux di versiterbarunya. Kali Linux iniakandijadikansebagaistandarisasidistro Linux yang digunakanuntukpercobaanpenetrasi.

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
