# Praktikum 2 - Memulai HTML

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HTML merupakan format standar yang digunakan untuk membuat dokumen halaman web. Dokumen HTML memiliki sintaks tanda berpasangan yang disebut TAG untuk memberikan efek yang diinginkan. Secara umum format TAG adalah sebagai berikut:

### Struktur Dasar Halaman HTML

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Setiap dokumen HTML harus diawali dengan tag `<html>` dan diakhiri dengan komplemennya, yakni tag `</html>` tag. Dokumen HTML juga menyertakan tiga pasang tag.

- Tag `<head>` dan `</head>`: digunakan untuk menyatakan informasi mengenai dokumen HTML.
- Tag `<title>` dan `</title>`: digunakan untuk menambahkan title di title bar browser.
- Tag `<body>` dan `</body>`: digunakan untuk melingkupi semua teks yang terdapat di halaman HTML.

Pada HTML5, struktur penulisan lebih ringkas dengan bentuk sebagai berikut:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <!-- Ini baris komentar, tidak diproses -->
    <title>Ini judul dokumen HTML5</title>
  </head>

  <body>
    Ini adalah teks di body
  </body>
</html>
```

### Langkah Praktikum

1.  Buka folder XAMPP di direktori tempat Anda menginstall XAMPP. Buka direktori **htdocs** kemudian buat satu folder baru bernama dasarWeb.

    ![htdocs](/html/img/praktikum2/htdocs.png)

    ![dasarWeb](/html/img/praktikum2/dasarweb.png)

2.  Kemudian buka text editor Anda, buat file baru bernama `hello.html` dan simpan di dalam direktori dasarWeb yang baru saja Anda buat.

    ```html
    <html>
      <head>
        <title>My First HTML Document</title>
      </head>

      <body>
        <p>
          Hello World! <br />
          Welcome to my <b>first</b> HTML Page.
        </p>
      </body>
    </html>
    ```

3.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/hello.html](http://localhost/dasarWeb/hello.html).

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![Tampilan Web](/html/img/praktikum2/br.png)

4.  Amati apa yang muncul pada browser. Catat hasil pengamatanmu.

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Tulisan “**My First HTML Document**” pada elemen `<title>`, akan terlihat di atas tab browser.
    - Didalam halaman web akan muncul paragraf yang diawali dengan tag `<p>` disertai dengan isi atau tulisan didalamnya.
    - Tulisan “**Hello World!**” dengan “**Welcome to my first HTML Page**” akan terlihat pisah walaupun didalam hello.html ditulis gabung. Hal ini dikarenakan fungsi dari `<br>` yaitu sebagai pemisah antara satu kalimat dengan kalimat yang lain dan membuat baris baru.
    - Kata “**first**” dicetak tebal karena diantara kata tersebut diapit dengan tag `<b>` yang berfungsi untuk menebalkan huruf.

5.  Hilangkan tag `<br>` pada kode, amati perbedaan dan sampaikan dibawah ini apakah fungsi tag `<br>`.

    - Seperti apa yang saya jelaskan pada point no. 4 yaitu fungsi dari `<br>` yaitu sebagai pemisah antara satu kalimat dengan kalimat yang lain dan membuat baris baru. Jika tag `<br>` dihilangkan, maka hasilnya seperti berikut:

      | Tanpa `<br>`                                  | Pakai `<br>`                               |
      | --------------------------------------------- | ------------------------------------------ |
      | ![Tanpa <br>](/html/img/praktikum2/no-br.png) | ![Pakai <br>](/html/img/praktikum2/br.png) |
