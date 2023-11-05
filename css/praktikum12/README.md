# Praktikum 12 - CSS _Layouting_

### Apa itu CSS _Layouting_?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CSS _layouting_ adalah teknik untuk mengatur tata letak sebuah halaman web dengan menggunakan kode CSS. Tujuan dari CSS _Layouting_ adalah agar halaman yang dibuat terlihat rapih, menarik sesuai dengan yang diharapkan oleh si pembuat. CSS _layouting_ terdiri dari beberapa bagian yaitu dimensi, _overflow_, Box model, float dan Position.

### CSS _Display_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Tag pada HTML digunakan untuk memberikan maksud / arti pada sebuah konten (contohnya adalah `p` untuk paragraph, `h1` untuk heading utama dan lain-lain). Tag `<div>` dan tag `<span>` tidak memiliki arti apapun, keduanya digunakan untuk mengelompokkan tag-tag HTML dan memberikan informasi terhadap tag-tag tersebut.

#### Langkah Praktikum

1.  Buat satu file baru bernama `layoutCSS.html` di dalam folder dasarWeb
2.  Ketikkan ke dalam file `layoutCSS.html` tersebut kode di bawah ini.

    ```html
    <!DOCTYPE html>
    <html>
      <head>
        <title>CSS Layouting</title>
      </head>

      <body>
        <h1>Selamat Datang Di Website Kami</h1>

        <h2>Daftar Link</h2>
        <a href="#">Link 1</a>
        <a href="#">Link 2</a>
        <a href="#">Link 3</a>
        <a href="#">Link 4</a>

        <h2>TEKNIK INFORMATIKA</h2>
        <img src="img/polinema.png" />
        <p>
          Pada tahun 2010 berdasar kebutuhan masyarakat dan industri terkait
          Program Diploma IV Bidang Informatika maka Polinema mendirikan program
          studi baru Diploma IV (DIV) Teknik Informatika (TI). Pada awal
          berdirinya jumlah peserta didik Program D-IV TI hanya terdiri dari 46
          Mahasiswa, namun pada tahun 2015 jumlah peserta didik Prodi D-IV TI
          telah mengalami peningkatan menjadi 545 Mahasiswa.
        </p>

        <p>
          Perkembangan jumlah mahasiswa yang sangat pesat baik di Program Studi
          D-III MI maupun D-IV TI mendorong pimpinan di Polinema untuk
          menyatukan kedua program studi tersebut dalam satu organisasi jurusan
          baru terpisah dari Jurusan Teknik Elektro. Dan pada tahun 2015
          berdasarkan SK Direktur Nomor 53 dalam rangka peningkatan mutu
          pengelolaan dan optimasi sumber daya dibentuklah Jurusan Teknologi
          Informasi (JTI) dengan prodi D-III MI dan D-IV TI.
        </p>

        <p class="copyright">
          Copyright 2020. Desain dan Pemrograman Web JTI Polinema
        </p>
      </body>
    </html>
    ```

3.  Kemudian buatlah `<div>` pada halaman html yang sama seperti pada kode program di bawah ini

    ```html
    <!DOCTYPE html>
    <html>
      <head>
        <title>CSS Layouting</title>
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
        </div>

        <div class="main">
          <h2>TEKNIK INFORMATIKA</h2>
          <img src="img/polinema.png" />
          <p>
            Pada tahun 2010 berdasar kebutuhan masyarakat dan industri terkait
            Program Diploma IV Bidang Informatika maka Polinema mendirikan
            program studi baru Diploma IV (DIV) Teknik Informatika (TI). Pada
            awal berdirinya jumlah peserta didik Program D-IV TI hanya terdiri
            dari 46 Mahasiswa, namun pada tahun 2015 jumlah peserta didik Prodi
            D-IV TI telah mengalami peningkatan menjadi 545 Mahasiswa.
          </p>

          <p>
            Perkembangan jumlah mahasiswa yang sangat pesat baik di Program
            Studi D-III MI maupun D-IV TI mendorong pimpinan di Polinema untuk
            menyatukan kedua program studi tersebut dalam satu organisasi
            jurusan baru terpisah dari Jurusan Teknik Elektro. Dan pada tahun
            2015 berdasarkan SK Direktur Nomor 53 dalam rangka peningkatan mutu
            pengelolaan dan optimasi sumber daya dibentuklah Jurusan Teknologi
            Informasi (JTI) dengan prodi D-III MI dan D-IV TI.
          </p>
        </div>

        <div class="copyright">
          <p>Copyright 2020. Desain dan Pemrograman Web JTI Polinema</p>
        </div>
      </body>
    </html>
    ```

4.  Amati hasil dari kedua program tersebut sama atau berbeda, jelaskan alasannya

    Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/layoutCSS.html](http://localhost/dasarWeb/layoutCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![layoutCSS.html](/css/img/praktikum12/layoutCSS.png)

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Tidak ada perbedaan yang signifikan diantara kedua program tersebut.
    - Hanya saja program di tahap ke-5 dikelompokkan sehingga tidak berdiri sendiri.
    - Dibandingkan dengan program tahap ke-3 berdiri sendiri tiap elemen

5.  Tambahkan `style` pada _class_ **navigasi** dan _class_ **main** seperti pada kode program di bawah ini

    ```html
    <head>
      <title>CSS Layouting</title>
      <style>
        .navigasi {
          background-color: pink;
        }

        .main {
          background-color: lightgreen;
        }
      </style>
    </head>
    ```

6.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/layoutCSS.html](http://localhost/dasarWeb/layoutCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![layoutCSS.html](/css/img/praktikum12/layoutCSS2.png)

7.  Jelaskan apa yang terjadi pada website tersebut

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Warna dari **class navigasi** berubah menjadi pink
    - Warna dari **class main** berubah menjadi hijau cerah
    - Penerapan `div` dalam html sangat berguna dalam menerapkan layouting css
    - Selain itu, penerapan css didalam praktikum ini menggunakan internal css yang menyisipkan css langsung dari html dengan tag `<style>` yang ditaruh didalam tag `<head>`
