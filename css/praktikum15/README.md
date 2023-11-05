# Praktikum 15 - Display _Block_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_Block_ adalah elemen HTML yang secara _default_ menambahkan baris baru Ketika dibuat Jika tidak diatur lebar-nya, maka lebar _default_ dari elemen _block_ akan memenuhi lebar dari _browser / parent_-nya sehingga kita dapat mengatur tinggi dan lebar dari elemen _block_. Di dalam elemen _block_, kita dapat menyimpan tag dengan elemen _inline_, _inline-block_, atau bahkan elemen _block_ lagi. Adapun contoh-contoh elemen _block_ adalah ; `<h1-6>`, `<p>`, `<ol>`, `<ul>`, `<li>`, `<form>`, `<hr>`, `<div>`

### Langkah Praktikum

1.  Buka file `layoutCSS.html` pada [praktikum 12](/css/praktikum12/dasarWeb/layoutCSS.html)
2.  Beri style pada elemen `<h1>`, `<h2>` dan `<p>` dengan `background-color` warna `lightgreen` seperti pada kode program di bawah ini

    ```html
    <head>
      <title>CSS Layouting</title>
      <style>
        a {
          background-color: pink;
        }

        h1,
        h2,
        p {
          background-color: lightgreen;
        }
      </style>
    </head>
    ```

3.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/layoutCSS.html](http://localhost/dasarWeb/layoutCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![layoutCSS.html](/css/img/praktikum15/layoutCSS5.png)

4.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Display link kembali ke _inline_
    - Perubahan warna pada link yaitu berwarna pink dan warna pada `h1`, `h2`, dan `p` yang merupakan display _block_ (menambah baris baru) yaitu berwarna hijau cerah
    - Perubahan warna pada elemen panjangnya mengikuti ukuran website

5.  Kemudian selanjutnya silakan tambahkan style pada class main seperti pada kode program dibawah ini

    ```html
    <head>
      <title>CSS Layouting</title>
      <style>
        a {
          background-color: pink;
        }

        .main {
          width: 600px;
          background-color: lightgreen;
        }

        .main h2 {
          background-color: pink;
        }
      </style>
    </head>
    ```

6.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/layoutCSS.html](http://localhost/dasarWeb/layoutCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![layoutCSS.html](/css/img/praktikum15/layoutCSS6.png)

7.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Perubahan warna nya hanya elemen `<h2>` didaerah _class main_ dan _class main_ itu sendiri
    - Jika Panjang nya telah ditentukan misalnya `600px`, maka warna akan berada diarea `600px`.

### Display _None_

Untuk value display yang terakhir adalah _none_, _none_ ini dapat digunakan untuk menghilangkan sebuah elemen
