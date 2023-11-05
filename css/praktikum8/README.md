# Praktikum 8 - Mengatur Hyperlink dengan CSS

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_Hyperlink_ merupakan link yang dibuat untuk mengalihkan halaman saat di klik. _Hyperlink_ atau link dibuat dengan menggunakan tag dan di akhiri dengan tag di HTML. Ada 4 status yang di miliki oleh _hyperlink_ html dan bisa di manipulasi dengan menggunakan css. yaitu:

- _link._ merupakan link aktif biasa.
- _visited._ merupakan status sebuah link yang telah di kunjungi.
- _hover._ merupakan status sebuah link pada saat diletakkan cursor mouse di atasnya.
- _active_. merupakan status sebuah link atau _hyperlink_ pada saat sudah di klik.

_Syntax_ nya adalah sebagai berikut:

- `a:link` = untuk link biasa
- `a:visited` = merupakan status sebuah link yang telah di kunjungi.
- `a:hover` = merupakan status sebuah link pada saat diletakkan cursor mouse di atasnya.
- `a:active` = merupakan status sebuah link atau hyperlink pada saat sudah di klik.

### Langkah Praktikum

1.  Buat satu file baru bernama `linkCSS.html` di dalam folder dasarWeb
2.  Ketikkan ke dalam file `linkCSS.html` tersebut kode di bawah ini.

    ```html
    <!DOCTYPE html>
    <html>
      <head>
        <title>Hyperlink CSS</title>
        <link rel="stylesheet" type="text/css" href="styleLink.css" />
      </head>

      <body>
        <a class="link" href="http://www.polinema.ac.id" target="_blank"
          >Klik di sini</a
        >
      </body>
    </html>
    ```

3.  Buat satu file baru bernama `styleLink.css` di dalam folder dasarWeb
4.  Ketikkan ke dalam file `styleLink.css` tersebut kode di bawah ini.

    ```css
    .link {
      font-size: 20pt;
    }

    .link:link {
      color: blue;
    }

    .link:hover {
      color: red;
    }
    ```

5.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/linkCSS.html](http://localhost/dasarWeb/linkCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![linkCSS.html](/css/img/praktikum8/linkCSS.gif)

6.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Warna link sebelum diklik atau link yang baru dibuat, warna nya menjadi biru dari properti `a:link`.
    - Warna link saat mouse menggeser ke link / diatas link, warnanya menjadi merah dari properti `a:hover`.

7.  Tambahkan kode pada `styleLink.css` untuk mengubah warna link menjadi hijau muda (greenyellow) setelah link dikunjungi. Tulis kode program yang anda tambahkan di sini

    ```css
    .link:visited {
      color: greenyellow;
    }
    ```

8.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/linkCSS.html](http://localhost/dasarWeb/linkCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![linkCSS.html](/css/img/praktikum8/linkCSS2.png)
