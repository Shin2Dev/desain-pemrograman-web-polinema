# Praktikum 7 - Pengaturan Font pada CSS

Beberapa syntax css yang digunakan untuk mengatur font:

- `font-size` digunakan untuk mengatur ukuran font
- `font-weight` di gunakan untuk mengatur ketebalan font
- `font-family` untuk mengubah jenis font
- `font-style` digunakan untuk merubah gaya pada font.
- `color` digunakan untuk merubah warna font

### Langkah Praktikum

1.  Buat satu file baru bernama `fontCSS.html` di dalam folder dasarWeb
2.  Ketikkan ke dalam file `fontCSS.html` tersebut kode di bawah ini.

    ```html
    <!DOCTYPE html>
    <html>
      <head>
        <title>Font CSS</title>
        <link rel="stylesheet" type="text/css" href="styleFont.css" />
      </head>

      <body>
        <h1 class="tulisan_satu">Belajar CSS Dasar asiiik</h1>
        <h1 class="tulisan_dua">Belajar CSS Dasar cihuuuii</h1>
        <h1 class="tulisan_tiga">Belajar CSS Dasar yuhuuuuu</h1>
      </body>
    </html>
    ```

3.  Buat satu file baru bernama `styleFont.css` di dalam folder dasarWeb
4.  Ketikkan ke dalam file `styleFont.css` tersebut kode di bawah ini.

    ```css
    .tulisan_satu {
      color: red;
      font-family: sans-serif;
      font-style: normal;
    }

    .tulisan_dua {
      color: green;
      font-size: 24pt;
      font-style: italic;
    }

    .tulisan_tiga {
      color: blue;
      font-weight: bold;
      font-style: oblique;
    }
    ```

5.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/fontCSS.html](http://localhost/dasarWeb/fontCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![fontCSS.html](/css/img/praktikum7/fontCSS.png)

6.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Dalam mengatur font / tulisan, terdapat banyak properti yang bisa digunakan
    - Untuk mengubah jenis tulisan, menggunakan properti `font-family` dan tulis nilainya dengan font yang tersedia contoh sans-serif, dsb. Jika tidak ada, bisa diimport dengan mendownload font di [Google Font](https://fonts.google.com/).
    - Untuk mengubah gaya tulisan menjadi miring, menggunakan properti `font-style` dan tulis nilainya dengan gaya miring (_italic / oblique_).
    - Untuk mengubah ukuran tulisan, menggunakan properti `font-size` dengan nilai nya dalam bentuk pt (disarankan).
    - Untuk menebalkan tulisan sebagai alternatif pengganti tag `<b>`, menggunakan properti `font-weight` dan tulis nilainya seberapa besar ketebalannya.
    - Untuk mengubah warna tulisan, menggunakan properti `color` dan tulis nilai untuk warna.
    - Penggunaan font ini lebih disarankan menggunakan css dibandingkan tag di html dikarenakan terdapat tag yang sudah jarang dipakai sehingga lebih banyak memakai css dalam mengatur font / tulisan.
