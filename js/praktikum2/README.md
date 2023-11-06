# Praktikum 2 - Membuat Program JavaScript Pertama

### Langkah Praktikum

1.  Silahkan buka text editor, kemudian buat folder baru bernama `belajarjavascript` di dalam folder `htdocs` dan buat file baru bernama `hello_world.html`
2.  Ketikkan kode program dibawah ini:

    ```html
    <!DOCTYPE html>
    <html>
      <head>
        <title>Hello World JavaScript</title>
      </head>

      <body>
        <script>
          console.log("Saya belajar JavaScript");
          document.write("Hello World!");
        </script>
      </body>
    </html>
    ```

3.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/hello_world.html](http://localhost/belajarjavascript/hello_world.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![Hello World](/js/img/praktikum2/hello-world.png)

4.  Amati apa yang terjadi pada browser, kemudian catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Didalam halaman website, hanya terdapat tampilan output “**Hello World!**”
    - Sedangkan dari yang ditulis di program, seharusnya terdapat output “**Saya Belajar Javascript**”
    - Hal ini terjadi dikarenakan dalam point dua, output nya tidak tampil di halaman langsung tetapi didalam console
    - Jika dibandingkan dengan point satu, output yang keluar karena `document.write` menulis dan menampilkan langsung di halamannya

5.  Sekarang coba buka console javascript, kemudian lihat pada Inspect Elements

    ![Inspect Element](/js/img/praktikum2/console.png)

6.  Amati apa yang terjadi pada tab Console, kemudian catat hasil pengamatanmu!

    - Jika dilihat dari console, output “**Saya Belajar Javascript**” muncul

7.  Tadi kita menuliskan perintah :

    ```js
    console.log("Saya belajar JavaScript");
    ```

    Menurut Anda, mengapa perintah tersebut tidak ditampilkan?

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Hal ini dikarenakan menggunakan program console.log yang digunakan untuk debugging
    - Karena inilah program tersebut bukan ditampilkan di halaman website melainkan di console dan hanya dijadikan untuk mengecek outputnya
