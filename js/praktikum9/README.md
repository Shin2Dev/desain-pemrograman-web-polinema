# Praktikum 9 - Percabangan

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Dapat dikatakan bahwa percabangan dan putaran merupakan salah satu inti metode dalam semua bahasa pemrograman yang ada di dunia, karena dengan percabangan dan putaran akan dihasilkan sebuah program yang dinamis, dan bukan program yang linear serta bersifat statik. Karena JavaScript merupakan salah satu cara dalam melakukan pemrograman web di sisi client, maka JavaScript juga memiliki kemampuan ini.

Beberapa fungsi percabangan:

- Gunakan **_if_** untuk menentukan blok kode yang akan dieksekusi jika kondisi tertentu benar.
- Gunakan **_else_** untuk menentukan blok kode yang akan dieksekusi jika kondisi yang sama adalah salah.
- Gunakan **_else if_** untuk menentukan kondisi baru yang akan diuji jika kondisi pertama salah.
- Gunakan **_switch_** untuk menentukan banyak blok kode alternatif yang akan dieksekusi.

### Percabangan _if_

Percabangan _if_ merupakan percabangan yang hanya memiliki **satu blok pilihan** saat kondisi bernilai benar. Coba perhatikan _flowchart_ berikut ini:

![Flowchart If](/js/img/praktikum9/flowchart-if.png)

“Jika total belanja lebih besar dari Rp. 100.000, Maka tampilkan pesan 'Selamat, Anda dapat hadiah'“

Kalau dibawah Rp 100.000 bagaimana? <br>
Ya pesannya tidak ditampilkan.

<img src="/js/img/praktikum9/cerdas.jpg" width="20%" alt="Cerdas">

#### Langkah Praktikum

1.  Buat File baru bernama `if_javascript.html` dan simpan dalam direktori belajarjavascript
2.  Ketikkan kode program dibawah ini:

    ```html
    <!DOCTYPE html>
    <html lang="en">
      <head>
        <title>Percabangan If</title>
      </head>

      <body>
        <script>
          var totalBelanja = prompt("Total belanja?", 0);

          if (totalBelanja > 30000) {
            document.write("<h2>Selamat anda dapat hadiah</h2>");
          }

          document.write("<p>Terima Kasih sudah berbelanja di toko kami</p>");
        </script>
      </body>
    </html>
    ```

3.  Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

    Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/if_javascript.html](http://localhost/belajarjavascript/if_javascript.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![if](/js/img/praktikum9/if-prompt.png)

    Hasil pengamatan saya sebagai berikut:

    - Dalam program ini, penerapan decision / pilihan yaitu `if`
    - Dalam program, jika total belanja lebih dari 30000, maka akan menampilkan **Selamat anda dapat hadiah**

      ![If True](/js/img/praktikum9/if-true.png)

      Jika tidak, maka tidak dapat hadiah

      ![If False](/js/img/praktikum9/if-false.png)

    - Selanjutnya akan menampilkan **Terimakasih sudah berbelanja di toko kami**, baik yang kondisi nya benar ataupun salah.

### Percabangan _If/Else_

Percabangan _if/else_ merupakan percabangan yang memiliki **dua blok pilihan**. Pilihan pertama untuk kondisi **benar**, dan pilihan kedua untuk kondisi **salah** (_else_). Coba perhatikan flowchart ini:

![Flowchart If Else](/js/img/praktikum9/flowchart-if-else.png)

Ini adalah flowchart untuk mengecek password. Apabila password benar, pesan yang ada pada blok hijau akan ditampilkan: **Selamat datang bos!** Tapi kalau salah, maka pesan yang ada di blok merah yang akan ditampilkan: **Password salah, coba lagi!**

#### Langkah Praktikum

1.  Buat File baru bernama `ifelse_javascript.html` dan simpan dalam direktori belajarjavascript
2.  Ketikkan kode program dibawah ini:

    ```html
    <!DOCTYPE html>
    <html lang="en">
      <head>
        <title>Percabangan If-Else</title>
      </head>

      <body>
        <script>
          var password = prompt("Password:");

          if (password == "teh") {
            document.write("<h2>Selamat Datang</h2>");
          } else {
            document.write("<p>Password Salah, Coba Lagi!</p>");
          }

          document.write("<p>Terima kasih sudah menggunakan aplikasi ini!</p>");
        </script>
      </body>
    </html>
    ```

3.  Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

    Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/ifelse_javascript.html](http://localhost/belajarjavascript/ifelse_javascript.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![if else](/js/img/praktikum9/ifelse-prompt.png)

    Hasil pengamatan saya sebagai berikut:

    - Penerapan if/else di program ini adalah menginputkan password, (_password_ = **Teh**)
    - Jika password benar, maka mengucapkan selamat datang
      ![If](/js/img/praktikum9/ifelse-true.png)
    - Jika password salah, maka akan menampilkan password salah

      ![Else](/js/img/praktikum9/ifelse-false.png)

    - Selanjutnya akan menampilkan **Terimakasih sudah menggunakan aplikasi ini!**, baik yang kondisi nya benar ataupun salah.

### Percabangan _Switch/Case_

Percabangan _switch/case_ adalah bentuk lain dari percabangan _if/else/if_.

Strukturnya seperti ini:

```js
switch (variabel){
  case <value>:
    // blok kode
    break;
  case <value>:
    // blok kode
    break;
  default:
    // blok kode
}
```

#### Langkah Praktikum

1.  Buat File baru bernama `switchcase_javascript.html` dan simpan dalam direktori belajarjavascript
2.  Ketikkan kode program dibawah ini:

    ```html
    <!DOCTYPE html>
    <html lang="en">
      <head>
        <title>Percabangan Switch-Case</title>
      </head>

      <body>
        <script>
          var jawab = prompt(
            "Kamu beruntung! Silahkan pilih hadiahmu dengan memasukkan angka 1 sampai 5"
          );

          var hadiah = "";
          switch (jawab) {
            case "1":
              hadiah = "Tisu";
              break;
            case "2":
              hadiah = "1 Kotak Kopi";
              break;
            case "3":
              hadiah = "Sticker";
              break;
            case "4":
              hadiah = "Minyak Goreng";
              break;
            case "5":
              hadiah = "Uang Rp. 50000";
              break;
            default:
              document.write("<p>Opps! anda salah pilih</p>");
          }

          if (hadiah === "") {
            document.write("<p>Kamu gagal mendapat hadiah</p>");
          } else {
            document.write("<h2>Selamat kamu mendapatkan " + hadiah + "</h2>");
          }
        </script>
      </body>
    </html>
    ```

3.  Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

    Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/switchcase_javascript.html](http://localhost/belajarjavascript/switchcase_javascript.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![switch case](/js/img/praktikum9/switch-prompt.png)

    Hasil pengamatan saya sebagai berikut:

    - Pengguna akan menginputkan nilai 1-5
    - Jika menginputkan nilai antara 1-5 maka akan mendapat hadiah

      ![switch case true](/js/img/praktikum9/switch-true.png)

    - Hadiah nya berbeda tergantung input pengguna seperti

      - angka 1, **Tisu**
      - angka 2, **1 Kotak Kopi**
      - angka 3, **Sticker**
      - angka 4, **Minyak Goreng**
      - angka 5, **Uang Rp. 50000**

      **_Tentunya pilih uang dong, kan yang buat program aing :)_**

      <img src="/js/img/praktikum9/mendset.jpg" width="20%" alt="Genset">

    - Jika salah menginputkan / nilai lebih dari 5 atau nilai 0, maka gagal mendapat hadiah

      ![switch case false](/js/img/praktikum9/switch-false.png)

### Percabangan Bersarang

Kita juga dapat membuat blok percabangan di dalam percabangan. Ini disebut percabangan bersarng atau _nested if_.

#### Langkah Praktikum

1.  Buat File baru bernama `nestedif_javascript.html` dan simpan dalam direktori belajarjavascript
2.  Ketikkan kode program dibawah ini:

    ```html
    <!DOCTYPE html>
    <html lang="en">
      <head>
        <title>Percabangan Ternary</title>
      </head>

      <body>
        <script>
          var username = prompt("Username");
          var password = prompt("Password");

          if (username == "mahasiswa") {
            if (password == "kopi") {
              document.write("<h2>Selamat Datang</h2>");
            } else {
              document.write("<p>Password salah, coba lagi!</p>");
            }
          } else {
            document.write("<p>Anda tidak terdaftar!</p>");
          }
        </script>
      </body>
    </html>
    ```

3.  Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

    Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/nestedif_javascript.html](http://localhost/belajarjavascript/nestedif_javascript.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![Nested If](/js/img/praktikum9/nested-prompt.png)

    Hasil pengamatan saya sebagai berikut:

    - Pengguna akan menginputkan username dan password
    - Jika username dan password benar maka akan mengucapkan selamat datang

      ![User dan Pass Benar](/js/img/praktikum9/akun-ada.png)

    - Jika username benar dan password salah maka akan menampilkan notif password salah

      ![User benar tapi pass salah](/js/img/praktikum9/pass-salah.png)

    - Jika username salah, maka tidak terdaftar

      ![Gak terdaftar](/js/img/praktikum9/gak-diajak.png)

      **_Yang gak terdaftar bilek :)_**

      <img src="/js/img/praktikum9/gak-diajak.jpg" width="20%" alt="Gak diajak">
