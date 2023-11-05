# Praktikum 9 - Mengatur Format Text dengan CSS

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Pengaturan format text di dalam CSS adalah sebagai berikut:

- `color`: untuk mengatur warna text, value yang dapat diisi berupa warna atau kode warna
- `text-align`: untuk mengatur posisi align pada text atau rata text, value yang bisa diisi di antaranya adalah:
  - `center` untuk membuat text rata tengah
  - `left` untuk membuat text rata kiri
  - `right` untuk membuat text menjadi rata kanan
  - `justify` untuk membuat text menjadi rata kanan dan rata kiri.
- `text-decoration`: untuk mengatur dekorasi text, valuenya berupa :
  - `none` untuk membuat text tidak memiliki dekorasi
  - `overline` untuk membuat text memiliki garis pada bagian atas text
  - `line-through` untuk membuat garis yang mencoreng pada text
  - `underline` untuk membuat garis pada bawah text (garis bawah).
- `text-transform`: untuk mengatur huruf kapital pada text, value yang bisa di gunakan diantaranya adalah:
  - `uppercase` untuk membuat text menjadi huruf besar
  - `lowercase` untuk membuat text menjadi huruf kecil
  - `capitalize` untuk membuat huruf awal pada tiap kata menjadi huruf besar.
- `text-indent`: untuk mengatur jarak alinea pada text, value yang bisa digunakan berupa nilai pixel dan lainnya sesuai kebutuhan.
- `letter-spacing`: untuk mengatur jarak antar karakter pada text, value yang di isi berupa nilai pixel dan lain-lain.
- `word-spacing`: untuk mengatur jarak antar kata pada text, value yang di isi juga berupa nilai pixel.
- `line-height`: untuk mengatur jarak antar baris pada text value yang di isi berupa nilai.
- `text-shadow`: untuk mengatur efek bayang pada text, value yang di isikan:

  - pertama mengisi nilai untuk jarak kiri kanan
  - kedua mengisi jarak atas bawah
  - ketiga mengisi warna

  untuk contoh penulisannya `2px 5px blue`.

- `vertical-align`: untuk mengatur align dalam bentuk vertikal pada text value yang digunakan adalah:
  - `left` untuk membuat text rata kiri
  - `right` untuk rata atas
  - `center` untuk rata tengah.

### Langkah Praktikum

1.  Buat satu file baru bernama `textCSS.html` di dalam folder dasarWeb
2.  Ketikkan ke dalam file `textCSS.html` tersebut kode di bawah ini.

    ```html
    <html>
      <head>
        <title>Format Text CSS</title>
        <link rel="stylesheet" type="text/css" href="styleText.css" />
      </head>

      <body>
        <p class="tulisan_warna">Mengatur format text dengan CSS</p>
        <p class="par1">
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptatum,
          temporibus! Libero temporibus voluptate vero porro? Labore nostrum
          commodi repudiandae? Et veniam totam qui nemo commodi dicta fugiat
          voluptatem, quam dignissimos! Lorem ipsum dolor sit amet consectetur
          adipisicing elit. Natus ab impedit aliquam possimus fuga eaque! Harum
          quas nostrum asperiores, hic veritatis corrupti reiciendis ducimus eos
          repellat dolor maiores non delectus!
        </p>
      </body>
    </html>
    ```

3.  Buat satu file baru bernama `styleLink.css` di dalam folder dasarWeb
4.  Ketikkan ke dalam file `styleLink.css` tersebut kode di bawah ini.

    ```css
    .tulisan_warna {
      color: blue;
    }
    ```

5.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/textCSS.html](http://localhost/dasarWeb/textCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![textCSS.html](/css/img/praktikum9/textCSS.png)

6.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Warna pada elemen paragraf dengan class **tulisan_warna** menjadi warna biru yang berasal dari penerapan properti css yaitu `color`.

7.  Tambahkan kode pada `styleText.css` untuk mengubah posisi text menjadi di tengah dengan menambahkan `text-align: center`;. Tulis kode program yang anda tambahkan di sini

    ```css
    .tulisan_warna {
      color: blue;
      text-align: center;
    }
    ```

8.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/textCSS.html](http://localhost/dasarWeb/textCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![textCSS.html](/css/img/praktikum9/textCSS2.png)

9.  Tambahkan kode pada `styleText.css` untuk menambahkan garis bawah pada text. Tulis kode program yang anda tambahkan di sini

    ```css
    .tulisan_warna {
      color: blue;
      text-align: center;
      text-decoration: underline;
    }
    ```

10. Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/textCSS.html](http://localhost/dasarWeb/textCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![textCSS.html](/css/img/praktikum9/textCSS3.png)

11. Tambahkan kode program pada `styleText.css` untuk memberikan jarak antar karakter pada paragraf yang ada menjadi `5px` dengan `letter-spacing`. Tulis kode program yang anda tambahkan di sini

    ```css
    .tulisan_warna {
      color: blue;
      text-align: center;
      text-decoration: underline;
      letter-spacing: 5px;
    }
    ```

12. Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/textCSS.html](http://localhost/dasarWeb/textCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![textCSS.html](/css/img/praktikum9/textCSS4.png)
