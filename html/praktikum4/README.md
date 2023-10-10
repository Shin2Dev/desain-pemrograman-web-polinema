# Praktikum 4 - Font

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HTML menyediakan sejumlah elemen yang dapat dimanfaatkan untuk mengatur font seperti huruf tebal, huruf miring, garis bawah dan masih banyak lagi. <br>
Sebagai tambahan, di sini juga akan dijelaskan mengenai cara mencetak tag. Seperti diketahui, tag `<p>` di dokumen secara otomatis akan diterjemahkan sebagai paragraf. Adapun untuk mencetak karakter `<p>` di layar, kita perlu menggunakan nama entitas. <br>
Sebagai contoh, karakter < dinyatakan dengan nama entitas `&lt` dan karakter > dinyatakan dengan `&gt`.

### Langkah Praktikum

1.  Buat sebuah file bernama `font.html` dan simpan file tersebut di dalam folder dasarWeb.
2.  Ketikkan kode di bawah ini dalam `font.html`

    ```html
    <html>
      <head>
        <title>Pengaturan Font</title>
      </head>

      <body>
        <b>Menggunakan tag &lt;b&gt;</b><br />
        <strong>Menggunakan tag &lt;strong&gt;</strong><br />
        <i>Menggunakan tag &lt;i&gt;</i><br />
        <em>Menggunakan tag &lt;em&gt;</em><br />
        <u>Menggunakan tag &lt;u&gt;</u><br />
        <strike>Menggunakan tag &lt;strike&gt;</strike>
      </body>
    </html>
    ```

3.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/font.html](http://localhost/dasarWeb/font.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![font.html](/html/img/praktikum4/font.png)

4.  Amati apa yang muncul pada browser. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Tag `<b>` dan `<strong>` berfungsi untuk menebalkan kata. Yang membedakan adalah `<b>` hanya menebalkan sedangkan `<strong>` menebalkan dan menegaskan / menekankan kata.
    - Tag `<i>` dan `<em>` berfungsi untuk memiringkan kata. Yang membedakan adalah `<i>` hanya memiringkan sedangkan `<em>` memiringkan dan menekankan kata.
    - Tag `<u>` berfungsi untuk menggaris bawahi kata.
    - Tag `<strike>` berfungsi untuk mencoret kata.
