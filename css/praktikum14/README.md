# Praktikum 14 - Display _Inline-block_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Jika pada elemen _inline_ kita tidak bisa mengatur tinggi dan lebar dari suatu elemen maka kita bisa mengaturnya dengan menggunaka _inline-block_. tidak ada elemen yang secara _default_ memiliki _property_.

### Langkah Praktikum

1.  Buka file `layoutCSS.html` pada [praktikum 12](/css/praktikum12/dasarWeb/layoutCSS.html)
2.  Tambahkan `width`, `height` dan `display` pada `style` di elemen `<a>` seperti pada kode program dibawah ini

    ```html
    <head>
      <title>CSS Layouting</title>
      <style>
        a {
          background-color: pink;
          width: 200px;
          height: 200px;
          display: inline-block;
        }
      </style>
    </head>
    ```

3.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/layoutCSS.html](http://localhost/dasarWeb/layoutCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![layoutCSS.html](/css/img/praktikum14/layoutCSS4.png)

4.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Display dari link / tag `<a>` berubah dari inline ke inline-block
    - Dengan perubahan display ini, penerapan css ke link dapat diimplementasikan dalam hal mengubah Panjang dan tinggi dari tiap link.
    - Warna link menjadi pink, Panjang dan tinggi `200px`
