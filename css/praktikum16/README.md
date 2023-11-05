# Praktikum 16 - _Box Model_

### Dimensi dan _Overflow_ pada CSS

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Dimensi memiliki dua property di CSS yaitu _width_ untuk lebar dan _height_ untuk tinggi. Satuan dari dimensi ada macam macam diantaranya adalah **px**, **%**, **in**, **cm**, **mm**, **pc**.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_Overflow_ adalah _property_ CSS yang digunakan untuk mengatur perilaku elemen yang tidak cukup pada suatu _parent_. Ada empat _value_ dari _property overflow_ diantaranya yaitu;

1. _Visible_ : _Value default_
2. _Auto_ : CSS akan secara otomatis akan menambahkan _scroll_ jika konten tidak cukup
3. _Hidden_ : konten akan disembunyikan atau tidak kelihatan
4. _Scroll_ : seperti auto, akan memunculkan _scroll_, tetapi jika _content_ cukup _scroll_ akan tetap ada

### _Box Model_ pada CSS

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Setiap elemen di halaman _website_ berada di dalam sebuah _box_ (kotak). Kita bisa mengatur ukuran dan posisi kotak tersebut. Kita bisa memberi warna / gambar sebagai _background_ kotak tersebut. Box model pada CSS mendefinisikan ‘kotak’ yang dihasilkan oleh sebuah elemen, lalu menampilkannya sesuai dengan format visualnya. CSS box model terdiri dari 4 komponen yaitu; _margin_, _border_, _padding_ dan _content_ seperti pada gambar di bawah ini.

![Komponen Box Model](/css/img/praktikum16/box-model.png)

1. _Margin_: area transparan di sekitar kotak (diluar _border_)
2. _Border_: batas disekeliling _content_ dan _padding_
3. _Padding_: area transparan di dalam kotak (antara _content_ dan _border_)
4. _Content_: konten sebenarnya di dalam _box_, bisa berupa teks atau gambar

Cara mengatur propertinya seperti pada tabel dibawah ini

| _Margin_        | _Padding_        | _Border_        |
| --------------- | ---------------- | --------------- |
| _Margin-top_    | _Padding-top_    | _Border-top_    |
| _Margin-right_  | _Padding-right_  | _Border-right_  |
| _Margin-bottom_ | _Padding-bottom_ | _Border-bottom_ |
| _Margin-left_   | _Padding-left_   | _Border-left_   |
| _Margin_        | _Padding_        | _Border_        |

### _Box Model: Margin_

- _Ovelapping_ margin <br>
  Terjadi Ketika kita menggabungkan dua buah margin. Kiri dan kanan atau atas dengan bawah. Secara teori jika terjadi maka akan di ambil nilai yang paling besar.

- _Negative_ margin akan membuat kotak berlawanan arah. Bisa digunakan jika kita ingin menyembunyikan elemen.

- _Auto_ margin adalah nilai yang dapat kita kasih kedalam margin khusus untuk margin kiri dan margin kanan. Auto ini akan membuat elemenya berada di tengah-tengah halaman web browser

- _Shorthand_ margin adalah cara menyingkat penulisan margin

#### Langkah Praktikum

1.  Buat satu file baru bernama `boxCSS.html` di dalam folder dasarWeb
2.  Ketikkan ke dalam file `boxCSS.html` tersebut kode di bawah ini.

    ```html
    <!DOCTYPE html>
    <html>
      <head>
        <title>Latihan Margin</title>
        <link rel="stylesheet" href="styleBox.css" />
      </head>

      <body>
        <div class="satu">1</div>
        <div class="dua">2</div>
        <div class="tiga">3</div>
      </body>
    </html>
    ```

3.  Buat satu file baru bernama `styleBox.css` di dalam folder dasarWeb
4.  Ketikkan ke dalam file `styleBox.css` tersebut kode di bawah ini.

    ```css
    .satu {
      width: 200px;
      height: 200px;
      background-color: lightgreen;
    }

    .dua {
      width: 100px;
      height: 100px;
      background-color: lightblue;
    }
    .tiga {
      width: 50px;
      height: 50px;
      background-color: violet;
    }
    ```

5.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/boxCSS.html](http://localhost/dasarWeb/boxCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![boxCSS.html](/css/img/praktikum16/boxCSS.png)

6.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Pembuatan tiga kotak persegi dari elemen `div` dengan ukuran dan warna yang berbeda beda

7.  Selanjutnya adalah memberi _margin_, dimana _margin_ adalah area _transparan_ yang ada di sekitar kotak. Tambahkan _style_ pada style.css `margin-top` sebesar `100px` pada **class.satu**

    ```css
    .satu {
      width: 200px;
      height: 200px;
      background-color: lightgreen;
      margin-top: 100px;
    }
    ```

8.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/boxCSS.html](http://localhost/dasarWeb/boxCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![boxCSS.html](/css/img/praktikum16/boxCSS2.png)

9.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Jarak kotak satu menjauh dari halaman atas website karena penerapan `margin-top` yang membuat area transparan diluar elemen lebih lebar
    - Tidak hanya satu kotak, tetapi ketiga kotak sekaligus terkena dampak perubahan posisi
    - Walaupun penerapan `margin-top` hanya satu kotak, tetapi perubahan posisi tetap semua elemen

10. Kemudian tambahkan ukuran _margin_ yang lain seperti pada kode program berikut ini

    ```css
    .satu {
      width: 200px;
      height: 200px;
      background-color: lightgreen;
      margin-left: 100px;
      margin-top: 30px;
      margin-bottom: 150px;
      margin-right: 50px;
    }
    ```

11. Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/boxCSS.html](http://localhost/dasarWeb/boxCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![boxCSS.html](/css/img/praktikum16/boxCSS3.png)

12. Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Jarak kotak satu telah diatur menjauh dari segala arah sehingga kotak satu terpisah dengan kotak dua dan tiga
    - Pengaturan margin berbeda-beda dari kotak satu

### _Box Model: Padding, Border & Box Sizing_

#### _Padding_

Cara pakai _padding_ sama seperti margin yaitu, tidak bisa di pakai _negative_, tidak bisa di beri nilai _auto_ dan mempengaruhi ukuran dari _box_ dari suatu elemen.

#### _Border_

Cara menulisnya; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`Border: width style color;`

_Style_ pada border; solid, dotted (titik titik), dashed(garis-garis), double

#### _Box sizing_

_Box sizing_ adalah properti yang menerima nilai _padding_ dan _border_ pada suatu elemen termasuk sebagai nilai total dari _width_ dan _height_ suatu elemen.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`box-sizing: content-box (default)| border-box | unser | initial | inherit;`
