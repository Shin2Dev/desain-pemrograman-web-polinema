# Praktikum 1 - Menghubungkan HTML dengan CSS

### Langkah Praktikum

1.  Buatlah satu file baru di dalam direktori dasarWeb, beri nama `index.html`.
2.  Ketikkan ke dalam file `index.html` tersebut kode di bawah ini.

    ```html
    <html>
      <head>
        <title>Main Page</title>
        <link rel="stylesheet" href="style.css" />
      </head>

      <body>
        <h2>Welcome To DasarWeb</h2>
      </body>
    </html>
    ```

3.  Buat lagi satu file baru di dalam direktori dasarWeb, beri nama `style.css`. Ketikkan kode di bawah ini di dalam file `style.css`.

    ```css
    h2 {
      color: orange;
      font-family: Trebuchet MS;
      text-align: center;
    }
    ```

4.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb](http://localhost/dasarWeb)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![HTML dan CSS](/css/praktikum1/img/html-css.png)

    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Dalam struktur halaman web, `index.html` akan selalu menjadi halaman utama sebuah web. Sehingga jika dalam sebuah direktori terdapat `index.html` maka dia akan selalu dipanggil dan ditampilkan di browser.

    Itulah sebabnya pada langkah 4 hanya diketik halaman localhost/dasarWeb tanpa nama file.

5.  Pada kode program di dalam `index.html` terdapat tag `<link>` di bagian head di mana atribut href merujuk ke halaman `style.css`.
6.  `style.css` berisi kode program untuk mengatur tampilan di dalam halaman yang merujuk ke file `style.css`, dalam praktikum ini adalah `index.html`. Sehingga tampilan di dalam `index.html` akan sesuai dengan properti yang diatur di dalam `style.css`.
