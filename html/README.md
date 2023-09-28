# Instalasi XAMPP dan HTML Dasar

## Topik

- Pengenalan konsep dasar Internet dan Web
- Instalasi XAMPP
- Pengenalan HTML Fundamental

## Tujuan

Mahasiswa diharapkan dapat:

1. Memahami konsep dasar Internet dan web
2. Melakukan instalasi XAMPP
3. Mahasiswa mampu membuat web statis menggunakan HTML

## Pendahuluan

### Apakah Internet?

- Sebuah jaringan komputer yang besar.
- Network of networks
- Bekerja berdasarkan protokol TCP/IP

### Apa saja layanan Internet?

- World Wide Web (WWW) : bekerja dengan protokol HTTP
- E-mail : bekerja dengan protokol Post Office Protocol (POP), Simple Mail Transfer Protocol (SMTP), Internet Message Access Protocol (IMAP)
- Chat : Internet Relay Chat (IRC)
- File Transfer : File Transfer Protocol (FTP)
- Remote Access : telnet, Shell Secure (SSH)
- VoIP
- dll

### Website dan Aplikasi Web

#### Website (WWW)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Website adalah sebuah kumpulan dari halaman web yang saling berhubungan dan dapat diakses melalui halaman utama (home page) menggunakan sebuah browser

Sebagai contoh, alamat [www.polinema.ac.id](www.polinema.ac.id), jika diakses maka akan tampil homepage.

![Homepage Polinema](/html/img/homepage.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Sedangkan halaman web adalah bagian dari homepage yang berupa menu atau link di mana ketika di-klik maka akan membuka halaman baru dengan informasi yang berbeda dengan homepage.

#### _Web Statis_ vs _Web Dinamis_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Web Statis** adalah website di mana penggunanya tidak bisa mengubah konten dari web tersebut secara langsung menggunakan browser. Interaksi yang terjadi antara pengguna dan server adalah seputar pemrosesan link saja. Halaman-halaman web tersebut tidak memiliki database. Data dan informasi yang ada pada web statis tidak berubah-ubah kecuali diubah sintaksnya. Dokumen web yang dikirim kepada client isinya akan sama dengan apa yang ada di web server.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Web Dinamis** adalah website di mana interaksi yang terjadi antara pengguna dan server sangat kompleks. Seseorang bisa mengubah konten dari halaman tertenti dengan menggunakan browser. Request dari pengguna dapat diproses oleh server yang kemudian ditampilkan dalam isi yang berbeda-beda menurut alur programnya. Halaman-halaman website tersebut terhubung dengan sebuah database, sehingga pada web dinamis akan memiliki informasi dan data yang berbeda-beda tergantung input yang disampaikan oleh client. Dokumen yang sampai di client akan berbeda dengan dokumen yang ada di server.

### Bagaimana Website Bekerja?

1. Pengguna menuliskan URL pada browser [http://www.google.com](http://www.google.com)
2. Browser akan menerjemahkan URL menjadi sebuah alamat IP dan menghubungkannya melalui TCP ke server pada port 80 (HTTP service)

   - Menghubungkan ke sebuah komputer dengan IP address 216.239.39.99 port 80

3. Melalui koneksi yang sudah terhubung, browser mengirimkan sebuah GET request (HTTP request)

   - GET/HTTP/1.1

4. Server merespon dengan HTTP response (dengan header dan file yang diminta dalam body). MIME type juga diikutsertakan sehingga memberitahu browser mengenai tipe file (HTML, text, image, dll)

   ![MIME Text](/html/img/mimetype.png)

5. File di dalam halaman web seperti gambar tidak dikirimkan dengan file utama, sehingga browser harus melakukan request untuk mendapatkan semua file dalam halaman web.

   - GET /logo.gif HTTP/1.0

6. Browser akan melakukan render untuk ditampilkan kepada user dalam browser.
7. Koneksi dalam HTTP tidak berlangsung terus menerus, ketika sebiah file selesai diunduh, koneksi akan putus.

   ![HTTP Request And Response](/html/img/http-request-response.png)

### _Hypertext Markup Language_ (HTML)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_HyperText Markup Language_ (HTML) adalah sebuah Bahasa yang digunakan untuk membuat sebuah halaman web, dimana pemformatan menggunakan hiperteks sederhana yang ditulis menggunakan format ASCII agar menghasilkan tampilan wujud yang terintegerasi.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HTML ini merupakan standart internet yang didefinisikan dan dikendalikan penggunaannya oleh _World Wide Web Consortium_ (W3C). HTML dibuat oleh kolaborasi Caillau TIM dengan Berners-Lee Robert ketika mereka bekerja di CERN pada tahun 1989 (CERN adalah lembaga penelitian fisika energi Tinggi di jenewa).
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HTML dapat dibaca oleh berbagai macam _platform_. HTML juga merupakan Bahasa pemograman yang fleksible dan dapat digabungkan dengan Bahasa pemograman lain seperti PHP, ASP, JSP dan JavaScript.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Beberapa _tag_ dalam dokumen-dokumen HTML menentukan bagaimana teks diformat. Terdapat juga _tag-tag_ yang lain yang memberitahukan bagaimana menanggapi aksi-aksi yang dilakukan oleh pengguna. Sebagai contoh buka halaman [www.google.com](www.google.com) dan klik kanan pada _browser_ (Chrome) pilih inspect sehingga pada browser akan muncul.

![Inspect Element](/html/img/inspect.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Pada baris pertama terdapat tulisan &lt;!DOCTYPE HTML&gt;, ini menunjukkan bahwa dokumen yang sedang anda buka adalah HTML. Pada baris kedua terdapat juga _tag_ HTML, kode tersebut juga menandakan bawah kode-kode yang ditulis didalamnnya adalah kode HTML

### Daftar Praktikum

1. [Instalasi XAMPP](/html/praktikum1/)
2. [Memulai HTML](/html/praktikum2/)
3. [Format Teks](/html/praktikum3/)
4. [Font](/html/praktikum4/)
5. [Karakter Khusus]()
6. [Garis Horizontal]()
7. [Menggunakan List]()
8. [Pewarnaan]()
9. [Bekerja dengan Gambar]()
10. [Link]()
11. [Tabel dan Pengaturannya]()
12. [Bekerja dengan Form pada HTML]()

### Referensi:

1. Jason Beaird, The principles of Beautiful Web Design
2. Rian Ariona, Belajar HTML dan CSS ( Tutorial Fundamental dalam mempelajari HTML dan CSS)
3. Adi Hadisaputra, HTML dan CSS Fundamental dari Akar menuju Daun John Duckett,HTML dan CSS design and build websites
