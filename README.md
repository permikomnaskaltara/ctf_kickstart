# ctf_kickstart

Dalam bahasa Indonesia.

Dalam rangka meningkatkan kualitas dalam [agrihack.party](http://agrihack.party)

### [See To Believe (login pakai lx/akun univ) ](https://lx.apps.cs.ipb.ac.id/profile/13200)

## Pengenalan CTF basic

> Capture The Flag adalah salah satu kompetisi bidang keamanan. Jadi, peserta intinya ingin mendapat "flag". Dengan submit "flag", peserta dapat point.

![Image of CTF](http://digibond.wpengine.netdna-cdn.com/wp-content/uploads/2015/01/ffc-capture-the-flag-400x400.png)


Untuk referensi dasar, bisa baca di [blog ini](http://blog.rentjong.net/2014/11/mau-ikut-ctf-perlu-belajar-apa.html).


## Persiapan

### Yang Dibutuhkan
- Alat Komputasi ( desktop komputer / laptop / dll) yang direkomendasi terinstall Linux (Windows sebenarnya bisa)
- Koneksi Internet

### Setting Dasar

#### Install Linux

APA itu Linux?
> Linux adalah nama yang diberikan kepada sistem operasi komputer bertipe Unix. Linux merupakan salah satu contoh hasil pengembangan perangkat lunak bebas dan sumber terbuka utama.

Instalasi linux bisa secara dual boot dengan windows ataupun dengan **Virtualbox**

Distro Linux Yang Direkomendasi:
- Ubuntu
- Linux Mint
- Kali(tidak terlalu perlu sebenarnya)
- Yang penting Linux

Link terkait
- [Instalasi Linux](http://www.wikihow.com/Install-Ubuntu-Linux)
- [Dengan Virtualbox](http://www.instructables.com/id/How-to-install-Linux-on-your-Windows)


### Linux Dasar

Sekarang sudah di desktop linux, mari buka command line:

Mari Buka Terminal
```bash
Ctrl + T

```
atau
```bash
Ctrl + Alt + T
```
Selain command diatas, terminal bisa dibuka lewat menu, dan pilih **terminal** atau **xterm**, atau **console**

Keluar terminal, bisa ketik:
```bash
$ exit
```



## Nah, disinilah kita mulai perjalanan kita :camel:

### Syntax Dasar

Pertama - tama, lihat direktori anda dimana
```bash
pwd
```

Untuk masuk ke direktori gunakan:
```bash
# masuk ke dalam direktori
cd <DIREKTORI>

# kembali dari suatu direktori
cd ..
```
anda bisa menganggap cd adalah "change directory"

Untuk membuat sebuah direktori:
```bash
mkdir <DIREKTORI>
```

Untuk menampilkan semua file yang ada dalam direktori anda:
```bash
ls
```

Untuk membuka text editor di terminal :star: :
```bash
nano <NAMA FILE>
```
ketik yang anda mau, lalu tekan **Ctrl+O** untuk save dan **Ctrl+X** untuk keluar 


Untuk menampilkan isi file:
```bash
cat <NAMA FILE>
```
#### Contoh

*Anggaplah **#** sebuah komentar, tidak termasuk dalam kode*
**$** merupakan input
**>** merupakan output

```bash
# cek direktori sekarang
$ pwd
> /home/saya
$ mkdir coba_dir

$ cd coba_dir

$ pwd
> /home/saya/coba_dir

$ nano ayam

# ketik yang anda mau, lalu save

$ cat ayam
> rendang memang enak sekali

$ cd ..
$ pwd
> /home/saya

```

Jika stuck dalam program dan tidak bisa input command, Terpaksa gunakan **Ctrl+Z**


### Administrasi

```bash
# mengetahui username akun
$ whoami
> agrihacker

$ id
> uid=1000(agrihacker) gid=1000(agri) groups=1000(agri)

# menjadi root
$ sudo su
> [sudo] password for agrihacker: XXXXX

$ whoami
> root

```



*Note tentang **root** dalam linux*

> root is the user name or account that by default has access to all commands and files on a Linux or other Unix-like operating system

(sumber)[http://www.linfo.org/root.html]


Jalankan program:
```bash
./<NAMA_PROGRAM>

misal 

$ ./simple_cipher
> hai, ini output dari program
```

Terkadang, kita harus mengatur permission untuk menjalankan program
```bash
$ ./simple_cipher
> bash: ./simple_cipher: Permission denied

$ chmod +x simple_cipher

$
> hai, ini output dari program
```
Contoh diatas menggunakan **chmod**, yaitu untuk mengganti file permission
dan **chmod +x** berguna untuk mengganti file permission agar dapat di-execute/di-jalankan


### Manual

Tidak tahu kegunaan command linux? gunakanlah *manual* atau command **man**
```bash
man <COMMAND>
```
atau 
```bash
whatis <COMMAND>
```

#### contoh

```bash
$ whatis whoami
> whoami (1)           - print effective userid

$ man whoami
> `Akan keluar output yang dapat di-navigasi dengan arrow key, dan ketik q untuk keluar `


```




## Kategori Web

### Dasar
Untuk kategori web, dapat memanfaatkan *developer tool* bawaan browser.

Untuk browser chrome dan firefox dapat mengetikkan **F12** untuk menampilkan jendela *developer tool*
Untuk melihat source code, dapat menggunakan **Ctrl+U**


##### Komponen Web
Kita dapat mengkategorikan sebuah web menjadi dua bagian, yaitu **sisi server** dan **sisi client**

###### Client Side (Sisi Client)
Pada sisi client, komponen yang paling umum adalah **HTML** dan **CSS** untuk tampilan.

Dan **Javascipt** merupakan salah satu bahasa pemograman yang sering digunakan di sisi client sebuah website.

Javascript sangat powerful karena bisa melakukan hal-hal layaknya bahasa pemograman, dan sayangya banyak kelemahan pada website karena komponen javascript itu sendiri. Jadi, cukup berbahaya jika menaruh "data sensitif" pada client side .

###### Server Side (Sisi Server)
Pada sisi server,  banyak variasi skema, bahasa pemograman, dll. Untuk kompetisi CTF, sisi server paling banyak menggunakan bahasa **PHP**, **Javascript**, dan **Python**.

.


*in progress*




To Be Updated.....


### Sumber Lain
[Fan Page Cyber Security IPB](https://www.facebook.com/cysecipb)

[Situs Kompetisi agrihack.party](http://agrihack.party)

[Youtube Cyber Security IPB](https://www.youtube.com/channel/UCH6CPf10u9uQu3w1DRhOliw)
