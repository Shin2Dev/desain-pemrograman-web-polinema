# Praktikum 17 - _Flex Box_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Merupakan Model layout 1 dimensi yang dapat mengatur jarak dan penjajaran antar item dalam sebuah _container_. Yang dimaksud dengan satu dimensi adalah hanya dapat mengatur satu dimensi pada saat tertentu, antara baris atau kolom, tidak bisa keduanya sekaligus.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_Flex Box_ atau bisa di sebut juga _Flexbox Layout Module_ adalah sebuah modul yang menawarkan cara yang efektif untuk Menyusun, mensejajarkan dan mendistribusikan jarak antar item di dalam sebuah _container_, meskipun ukuranya dinamis atau bahkan kita tidak tahu.

![Flex](/css/img/praktikum17/flex.png)

- **_Main axis_**; Sumbu utama dari sebuah _container_ yang menentukan urutan dari penempatan item secara horizontal
- **_Main start/main end_**; Mulai dan berakhirnya items yang disimpan di dalam _container_
- **_Main size_**; ukuran (_width/height_) dari _container_ yang akan membuat dimensi dari items nya relative terhadap size

### _Property_ pada _container_

_Container_ adalah pembungkus dari elemen-elemen

![Container](/css/img/praktikum17/container.png)

**_Display_**

```css
.container {
  display: flex; /* on inline flex */
}
```

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_Display_ Membuat sebuah elemen _parent_ menjadi flex box, dan membuat elemen elemen di dalamnya bisa berprilaku flex juga.

**_Flex-direction_**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_Flex-direction_ Mengatur arah / urutan dari items di dalam _container_

![Flex-direction](/css/img/praktikum17/flex-direction.png)

```css
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```

**_Flex-Wrap_**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Secara _default_, semua _items_ di dalam _container_ akan berada pada satu baris meskipun ukuranya sudah sudah tidak cukup, _wrap_ memungkinkan untuk memindahkan items ke baris di bawahnya

![Flex-Wrap](/css/img/praktikum17/flex-wrap.png)

```css
.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```

#### Langkah Praktikum

1.  Buat satu file baru bernama `flexboxCSS.html` di dalam folder dasarWeb
2.  Ketikkan ke dalam file `flexboxCSS.html` tersebut kode di bawah ini.

    ```html
    <!DOCTYPE html>
    <html>
      <head>
        <title>Latihan Flexbox</title>
        <link rel="stylesheet" href="styleFlexbox.css" />
      </head>

      <body>
        <div class="container-satu">
          <div class="kolom-utama">
            <h2>Judul Artikel</h2>
            <p>
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Suscipit
              eos, nostrum vero, iusto deserunt adipisci labore error facere vel
              velit quibusdam sed dolor rerum? Dolorem explicabo beatae quia
              impedit repudiandae.
            </p>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Id
              pariatur officia quasi aliquid neque vero, quibusdam quo?
              Asperiores pariatur aliquam eveniet praesentium mollitia
              perspiciatis culpa ea ducimus accusamus nulla. Minima.
            </p>
          </div>

          <div class="sidebar-satu">
            <h3>Sidebar Satu</h3>
            <ul>
              <li><a href="">Link 1</a></li>
              <li><a href="">Link 2</a></li>
              <li><a href="">Link 3</a></li>
              <li><a href="">Link 4</a></li>
              <li><a href="">Link 5</a></li>
            </ul>
          </div>

          <div class="sidebar-dua">
            <h3>Sidebar Dua</h3>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas
              nobis tenetur eaque mollitia earum debitis ratione. Consequatur
              enim ullam vel quibusdam. Voluptatem illum sequi minima velit
              ipsum eveniet dicta maiores.
            </p>
          </div>
        </div>
      </body>
    </html>
    ```

3.  Buat satu file baru bernama `styleFlexbox.css` di dalam folder dasarWeb
4.  Ketikkan ke dalam file `styleFlexbox.css` tersebut kode di bawah ini.

    ```css
    html,
    body {
      margin: 0;
      padding: 0;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      background-color: #ddd;
      line-height: 1.65;
      padding-bottom: 1000px;
    }
    ```

5.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/flexbox.html](http://localhost/dasarWeb/flexbox.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![flexbox.html](/css/img/praktikum17/flexbox.png)

6.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - `Padding` dan `margin` dalam halaman html yang menjadi pengaturan bawaan diatur `0`
    - Jarak tulisan diatur dalam `1.65` dan jenis tulisan dengan menggunakan font `Arial` (diutamakan)
    - Warna latar belakang berubah menjadi abu-abu

7.  Tambahkan _style_ pada class **container-satu** pada file `styleFlexbox.css` seperti pada kode program di bawah ini

    ```css
    .container-satu {
      width: 800px;
      margin: 50px auto;
      background-color: #fff;
      padding: 20px;
      box-sizing: border-box;
    }
    ```

8.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/flexbox.html](http://localhost/dasarWeb/flexbox.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![flexbox.html](/css/img/praktikum17/flexbox2.png)

9.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Tampilan website menjadi lebih rapi dari sebelumnya
    - Pengaturan css pada class **container-satu** membuat tampilan website menjadi lebih baik dari sebelumnya
    - Yang membuat ukuran class **container-satu** lebih pas karena dengan adanya `box-sizing` dengan value `border-box`

10. Tambahkan property **display** pada selector **container-satu** dengan value **flex**. Capture dan jelaskan hasil nya

    ```css
    .container-satu {
      width: 800px;
      margin: 50px auto;
      background-color: #fff;
      padding: 20px;
      box-sizing: border-box;
      display: flex;
    }
    ```

11. Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/flexbox.html](http://localhost/dasarWeb/flexbox.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![flexbox.html](/css/img/praktikum17/flexbox3.png)

12. Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Elemen dalam website menjadi menyamping karena `display: flex;`
    - Tampilan website menjadi agak berantakan, tetapi bisa diperbaiki dari jarak antar elemen / item
