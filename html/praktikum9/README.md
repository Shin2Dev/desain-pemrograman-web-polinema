# Praktikum 9 - Bekerja dengan Gambar

Tak hanya teks, kita juga bisa menyisipkan gambar di dalam dokumen HTML. Untuk keperluan ini, HTML menyediakan tag `<img>` yang didukung dengan sejumlah atribut.

### Langkah Praktikum

1.  Tempatkan satu gambar dalam folder dasarWeb dengan ukuran bebas dan beri nama gambar tersebut dengan nama : bunga2, jika file berbentuk jpg maka namanya akan menjadi `bunga2.jpg` (file boleh berformat selain jpg)

    - Contoh gambar bisa download dari [Google](https://www.google.com) atau ambil foto sendiri.

      ![Cari Gambar di Google](/html/img/praktikum9/cari-gambar.png)

2.  Buat folder baru di dalam folder dasarWeb dan beri nama img.

    ![Folder Img di Dasar Web](/html/img/praktikum9/buat-file-img.png)

3.  Tempatkan satu gambar yang berbeda dengan gambar di langkah 1 dengan ukuran bebas di dalam folder img dan beri nama dengan bunga1, jika file berbentuk jpg maka namanya akan menjadi `bunga1.jpg` (file boleh berformat selain jpg)

    ![Bunga 1 dan Bunga 2](/html/img/praktikum9/file-dua-gambar.png)

4.  Buat sebuah file bernama `gambar.html` dan simpan file tersebut di dalam folder dasarWeb.

5.  Ketikkan kode di bawah ini dalam `gambar.html`

    ```html
    <html>
        <head>
            <title>Bekerja dengan gambar</title>
        </head>
        <body>
            <p>
                <!-- Menggunakan Path Relative -->
                <img src="img/bunga2.jpeg">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Odio id suscipit nobis repellat libero, repellendus
                iste consectetur enim, ex obcaecati voluptate sapiente eaque quia quos reprehenderit debitis minus quasi! Minus?
                <br>
                <hr>
            </p>
            <p>
                <!-- Menggunakan Path Absolute -->
                <img src="../dasarWeb/img/bunga1.jpeg" align="right">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Eum assumenda officia blanditiis nobis magnam
                doloribus itaque reprehenderit quas in quidem voluptates asperiores ad nisi doloremque, molestias voluptate
                earum beatae ullam?
            </p>
        </body>
    </html>
    ```

6.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/gambar.html](http://localhost/dasarWeb/gambar.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![gambar.html](/html/img/praktikum9/gambar.png)

7.  Amati apa yang muncul pada browser. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Untuk menyisipkan gambar pada halaman html, bisa dengan dua cara yaitu Path Relative atau Path Absolute.
    - **_Path Relative_** adalah cara menyisipkan gambar dengan menunjukkan direktori gambar yang spesifik dimana gambar itu berada dan berada dalam folder yang sama.
    - **_Path Absolute_** adalah cara menyisipkan gambar dengan menunjukkan direktori gambar secara global dan berada di luar folder. Dimulai dengan (../) hingga gambar yang diinginkan ditemukan. Fungsi dari (../) adalah untuk menunjukkan direktori terluar dan bisa ditumpuk.
    - Untuk menyisipkan gambar tidak harus didownload, bisa melalui link gambar di internet.
    - Format gambar dan penamaan harus sesuai, jika tidak maka gambar tidak bisa muncul.
    - Gambar juga dapat diberi perataan sesuai dengan keinginan.
