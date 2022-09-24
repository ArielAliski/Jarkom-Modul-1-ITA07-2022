# Komunikasi Data dan Jaringan Komputer
# Laporan Praktikum Modul 1 ITA07

# Anggota

| Nama                           | NRP          | 
| -------------------------------| -------------| 
| Naftali Salsabila Kanaya Putri    | `5027201012` | 
| Ariel Daffansyah Aliski           | `5027201058` | 
| Anak Agung Bintang Krisnadewi     | `5027201060` |

## Soal 1

### Menyebutkan web server yang digunakan pada "monta.if.its.ac.id"
<br>
    display filter menggunakan domain http.host contains monta.if.its.ac.id lalu follow, pilih TCP Stream seperti yang ada di bawah ini.
    ![Soal 1](1a.png)
    setelah itu akan ditemukan web server yang digunakan pada monta.if.its.ac.id adalah nginx/1.10.3
    ![Soal 1](1b.png)

## Soal 2

### Menemukan detail topik pada website “monta.if.its.ac.id” yang berisi judul TA
<br>
    mirip dengan cara nomor 1, display filter menggunakan domain http.host contains monta.if.its.ac.id, lalu klik File, pilih Export Objects, pilih HTTP seperti yang ada di bawah ini.
    ![Soal 2](2a.png)
    setelah itu export file dengan nama 194 yang merupakan detail topik TA, lalu klik Save. 
    ![Soal 2](2b.png)
    setelah itu, buka file yang telah di export, dan akan ditemukan judul TA yaitu Evaluasi unjuk kerja User Space Filesystem
    ![Soal 2](2c.png)
    
## Soal 3
Untuk memfilter sesuai permintaan soal digunakan perintah display filter tcp.dstport == 80 || udp.dstport == 80
![Soal3](Soal3.jpg)

## Soal 4
Untuk memfilter sesuai permintaan soal didgunakan perintah display filter tcp.srcport == 21 || udp.srcport == 21
![Soal4](Soal4.jpg)

## Soal 5
Untuk memfilter sesuai permintaan soal digunakan display filter  tcp.srcport == 443 || udp.srcport == 443 
![Soal5](Soal5.jpg)

## Soal  6
Periksa terlebih dahulu apa IP Address website lipi.go.id menggunakan domain name checker. Setelah ditemukan gunakan display filter sesuai ip addressnya sebagai berikut: ip.dst == 203.160.128.158
![Soal6](Soal6.jpg)

## Soal 7
Periksa IP Adress sendiri terlebih dahulu, lalu gunakan display filter sesuai ip address kita sebagai berikut: ip.src == 192.168.1.7
![Soal7](Soal7.jpg)
