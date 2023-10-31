# Praktikum 6 - Margin dan Padding pada CSS

### Mengenal _Margin_ pada CSS

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Margin adalah sisi luar dari sebuah element. misalnya anda ingin mengatur jarak antar element. anda bisa menggunakan _syntax margin_ untuk mengaturnya. Terdapat beberapa sisi luar margin yaitu:

- margin atas di tuliskan pada css dengan `margin-top`,
- margin bawah atau jarak luar bagian bawah di tulis di CSS dengan `margin-bottom`,
- `margin-left` sebagai jarak luar sebelah kiri element, dan
- `margin-right` adalah sisi luar pada bagian sebelah kanan

Tetapi jika anda hanya menggunakan _syntax margin_ saja, maka akan secara otomatis mengatur jarak atas, bawah, kiri dan kanan element.

#### Langkah Praktikum

1.  Buat satu file baru bernama `marginCSS.html` di dalam folder dasarWeb
2.  Ketikkan ke dalam file `marginCSS.html` tersebut kode di bawah ini.

    ```html
    <!DOCTYPE html>
    <html>
      <head>
        <title>Margin CSS</title>
        <link rel="stylesheet" type="text/css" href="styleMargin.css" />
      </head>

      <body>
        <div class="box">
          <h1>Ini adalah box</h1>
        </div>
        <div class="box-dua">
          <h1>Ini adalah box dua</h1>
        </div>
      </body>
    </html>
    ```

3.  Buat satu file baru bernama `styleMargin.css` di dalam folder dasarWeb
4.  Ketikkan ke dalam file `styleMargin.css` tersebut kode di bawah ini.

    ```css
    h1 {
      color: pink;
    }

    .box {
      background: blue;
      height: 200px;
      width: 300px;
      margin: 30px;
    }

    .box-dua {
      background: black;
      height: 100px;
      width: 200px;
      margin-left: 500px;
    }
    ```

5.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/marginCSS.html](http://localhost/dasarWeb/marginCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![marginCSS.html](/css/img/praktikum6/marginCSS.png)

6.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Dari kedua box diatas, terlihat menjauh dari tepi halaman. Hal ini dapat disimpulkan bahwa properti `margin` adalah sebagai jarak antara elemen luar / garis elemen dengan tepi luar.
    - Dari box pertama, dengan diterapkannya salah satu properti css yaitu `margin` bernilai `30px` maka jarak antara box pertama dengan halaman html hanya menjauh `30px` di semua sisi.
    - Sedangkan dari box ke-2, penerapannya sama hanya saja `margin` nya berlaku untuk bagian sisi kiri saja dengan bernilai `500px` sehingga jarak antara kiri elemen dan tepi luar bagian kiri lebih menjauh sepanjang `500px`.

7.  Ubah nilai `margin` pada pengaturan `.box` menjadi `margin : 300px;`.

    ```css
    .box {
      background: blue;
      height: 200px;
      width: 300px;
      margin: 300px;
    }
    ```

8.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/marginCSS.html](http://localhost/dasarWeb/marginCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![marginCSS.html](/css/img/praktikum6/marginCSS.gif)

9.  Catat di sini apa yang anda amati dari kode program di atas.

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Jarak margin / jarak antara garis tepi elemen dengan tepi luarnya makin menjauh yang tadinya berjarak `30px` sekarang menjadi `300px`.

### Mengenal _Padding_ pada CSS

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Padding adalah sisi dalam dari sebuah element. Kita bisa menggunakan syntax `padding` untuk mengatur jarak pada sisi dalam sebuah element yang kita tentukan. Sama seperti `margin` yang memiliki sisi-sisi. seperti top, left, right, bottom. Jenis padding yaitu:

- padding atas di tuliskan pada css dengan `padding-top` yang berarti mengatur sisi dalam sebelah atas sebuah element
- pading bawah atau jarak dalam bagian bawah di tulis di CSS dengan `padding-bottom`
- `padding-left` sebagai jarak dalam sebelah kiri element, - `padding-right` adalah sisi luar pada bagian sebelah kanan.
- Jika anda hanya menggunakan syntax `padding` saja maka akan secara otomatis mengatur jarak atas, bawah, kiri dan kanan element yang bagian dalam.

#### Langkah Praktikum

1.  Buat satu file baru bernama `paddingCSS.html` di dalam folder dasarWeb
2.  Ketikkan ke dalam file `paddingCSS.html` tersebut kode di bawah ini.

    ```html
    <!DOCTYPE html>
    <html>
      <head>
        <title>Padding CSS</title>
        <link rel="stylesheet" type="text/css" href="stylePadding.css" />
      </head>

      <body>
        <h2>Belajar Padding dengan CSS</h2>
        <div class="box">
          <h1>Ini adalah box</h1>
        </div>
        <div class="box-dua">
          <h1>Ini adalah box dua</h1>
        </div>
      </body>
    </html>
    ```

3.  Buat satu file baru bernama `styleMargin.css` di dalam folder dasarWeb
4.  Ketikkan ke dalam file `stylePadding.css` tersebut kode di bawah ini.

    ```css
    h1 {
      text-align: center;
      color: cornsilk;
    }

    h2 {
      text-align: center;
    }

    .box {
      background: blue;
      height: 200px;
      width: 300px;
      padding: 20px;
    }

    .box-dua {
      background: red;
      height: 100px;
      width: 600px;
      padding-left: 70px;
    }
    ```

5.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/paddingCSS.html](http://localhost/dasarWeb/paddingCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![paddingCSS.html](/css/img/praktikum6/paddingCSS.png)

6.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Dari kedua box diatas, terlihat melebar dari elemen dalam dan garis tepi elemen. Hal ini dapat disimpulkan bahwa properti `padding` adalah sebagai jarak antara elemen dalam / isi dengan garis terluar elemen.
    - Dari box pertama, dengan diterapkannya salah satu properti css yaitu `padding` bernilai `20px` maka jarak antara elemen dalam dengan garis tepi hanya menjauh / melebar `20px` di semua sisi.
    - Sedangkan dari box ke-2, penerapannya sama hanya saja `padding` nya berlaku untuk bagian sisi kiri saja dengan bernilai `70px` sehingga jarak antara kiri elemen dalam dan garis luar bagian kiri lebih menjauh / melebar sepanjang `70px`.

7.  Ubah nilai `padding` pada pengaturan `.box` menjadi `padding : 200px;`.

    ```css
    .box {
      background: blue;
      height: 200px;
      width: 300px;
      padding: 200px;
    }
    ```

8.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/paddingCSS.html](http://localhost/dasarWeb/paddingCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![paddingCSS.html](/css/img/praktikum6/paddingCSS.gif)

9.  Catat di sini apa yang anda amati dari kode program di atas.

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Jarak padding / jarak antara garis tepi elemen dengan elemen dalam / isi makin melebar yang tadinya berjarak `20px` sekarang menjadi `200px`.
