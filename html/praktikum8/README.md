# Praktikum 8 - Pewarnaan

Untuk memberikan warna background, HTML menyediakan atribut `bgcolor` di tag `<body>`. Atribut ini dapat diisi dengan nama warna (misalnya `red`) atau kode heksadesimal (misalnya `#FFFFFF`).

Khusus untuk elemen-elemen lain tertentu, tersedia atribut `color` yang memungkinkan untuk melakukan pewarnaan. Sama seperti `bgcolor`, nilai atribut ini juga dapat berupa nama warna atau kode heksadesimal.

### Langkah Praktikum

1.  Buat sebuah file bernama `warna.html` dan simpan file tersebut di dalam folder dasarWeb.
2.  Ketikkan kode di bawah ini dalam `warna.html`.

    ```html
    <html>
      <head>
        <title>Pewarnaan</title>
      </head>
      <!-- Memberi warna aqua di body -->
      <body bgcolor="aqua">
        <h3 align="center">Heading 3</h3>
        <font color="red">Font berwarna merah</font> <br />
        <br />
        <font color="#FF0000">
          Font berwarna merah (menggunakan nilai heksa)
        </font>
      </body>
    </html>
    ```

3.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/warna.html](http://localhost/dasarWeb/warna.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![warna.html](/html/img/praktikum8/warna.png)

4.  Amati apa yang muncul pada browser. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Halaman website dapat diberikan warna, baik dari background / latar belakang dan tulisan didalam halaman html.
    - Jika ingin mengubah warna pada latar belakang, menggunakan atribut `bgcolor`.
    - Jika ingin mengubah warna pada tulisan, menggunakan tag `<font>` disertai atribut `color`.
    - Untuk nilai warnanya bisa menggunakan nama warna dalam bahasa inggris, kode hex, atau rgb.
