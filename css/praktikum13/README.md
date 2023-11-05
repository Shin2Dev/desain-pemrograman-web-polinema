# Praktikum 13 - Display _Inline_

Elemen HTML yang secara _default_ tidak menambahkan baris baru Ketika dibuat. Karakteristik dari _display inline_ adalah:

1. Lebar dan tinggi elemennya besarnya sesuai dengan konten yang ada di dalamnya
2. Tidak dapat mengatur tinggi dan lebar dari elemen _inline_
3. _Margin_ dan _padding_ hanya mempengaruhi elemen secara horizontal, tidak vertical

Adapun elemen-elemen inline adalah sebagai berikut; `<b>`, `<strong>`, `<i>`, `<em>`, `<a>`, `<span>`, `<sub>`, `<sup>`, `<button>`, `<input>`, `<label>`, `<select>`, `<textarea>`

### Langkah Praktikum

1.  Buka file `layoutCSS.html` pada [praktikum sebelumnya](/css/praktikum12/dasarWeb/layoutCSS.html)
2.  Silakan hapus `style` kemudian tambahakan link 5 pada class navigasi seperti kode program di bawah ini

    ```html
    <head>
      <title>CSS Layouting</title>
      <style></style>
    </head>

    <body>
      <div class="header">
        <h1>Selamat Datang Di Website Kami</h1>
      </div>

      <div class="navigasi">
        <h2>Daftar Link</h2>
        <a href="#">Link 1</a>
        <a href="#">Link 2</a>
        <a href="#">Link 3</a>
        <a href="#">Link 4</a>
        <a href="#">Link 5</a>
      </div>

      ...
    </body>
    ```

3.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/layoutCSS.html](http://localhost/dasarWeb/layoutCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![layoutCSS.html](/css/img/praktikum13/layoutCSS3.png)

4.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Penambahan link menjadi 5 link
    - Tampilan html dari pengaturan bawaan tanpa css
    - Tidak ada penerapan css seperti `color`, `background`, `float`, dsb
    - Ketika menambahkan link, tanpa tag `<br>`, elemen akan ditaruh disamping link lainnya
