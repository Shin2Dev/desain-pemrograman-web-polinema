# Praktikum 10 - Mengenal Position CSS

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Position pada CSS di gunakan untuk mengatur posisi sebuah element HTML. Properti position CSS ini digunakan untuk menentukan posisi sebuah element HTML sesuai dengan yang diinginkan.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Secara umum untuk membuat posisi atau menetapkan posisi sebuah element kita pasti menggunakan properti css lainnya seperti mengatur top, left, bottom, right untuk menetapkan posisi sebuah element, tetapi properti tersebut tidak akan bekerja jika position belum di atur terlebih dahulu, hal ini dikarenakan properti lain tergantung dengan position yang di tetapkan.

Beberapa property CSS yang dapat digunakan untuk menentukan posisi sebuah element HTML adalah:

- _Static_: Position _static_ digunakan untuk mengatur element menjadi statis secara default. Elemen akan mengikuti posisi normal secara default, elemen tidak dipengaruhi oleh properti seperti top, bottom, left dan right.
- _Relative_: Sebuah element HTML yang menggunakan position _relative_ akan terletak pada posisi normal. Mengatur properti atas, kanan, bawah, dan kiri dari elemen yang diposisikan dengan “relatif” akan membuatnya jauh dari posisi normalnya. Konten lain tidak akan disesuaikan agar sesuai dengan celah yang ditinggalkan oleh elemen tersebut.
- _Fixed_: Sebuah element HTML yang di setting dengan position _fixed_ akan memiliki sifat tetap. tanpa ada perubahan bahkan jika halaman website di scroll. Berlaku pengaturan left, bottom, top dan right pada position fixed.
- _Absolute_: Element HTML yang menggunakan position _absolute_ akan diposisikan relatif dengan element lain yang mendahuluinya yang terdekat, bukan relatif terhadap layar secara normal.
- _Sticky_: Diposisikan berdasarkan posisi scroll pengguna. Elemen _sticky_ berganti-ganti antara relatif dan tetap, tergantung pada posisi scroll. Ini diposisikan relatif sampai posisi offset tertentu bertemu di viewport - lalu "menempel" di tempatnya (seperti posisi _fixed_).

### Langkah Praktikum

1.  Buat satu file baru bernama `positionCSS.html` di dalam folder dasarWeb
2.  Ketikkan ke dalam file `positionCSS.html` tersebut kode di bawah ini.

    ```html
    <html>
      <head>
        <title>Position CSS</title>
        <link rel="stylesheet" type="text/css" href="stylePosition.css" />
      </head>

      <body>
        <h2>Position: static;</h2>

        <p>
          Position static digunakan untuk mengatur elemen menjadi statis secara
          default. Elemen akan mengikuti posisi normal secara default. elemen
          tidak dipengaruhi oleh properti seperti top, bottom, left dan right.
        </p>

        <div class="static">Elemen ini diatur menggunakan posisi static</div>
        <br /><br /><br /><br />

        <h2>Position: relative;</h2>

        <p>
          Sebuah elemen HTML yang menggunakan posisi relatif akan terletak pada
          posisi normal. Mengatur posisi atas, kanan, bawah, dan kiri dari
          elemen yang diposisikan dengan "relatif" akan membuatnya jauh dari
          posisi normalnya. Konten lain tidak akan disesuaikan agar sesuai
          dengan celah yang ditinggalkan oleh elemen tersebut.
        </p>

        <div class="relative">
          Elemen ini diatur menggunakan posisi relative
        </div>
        <br /><br /><br />

        <h2>Position: fixed;</h2>

        <p>
          Sebuah elemen HTML yang disetting dengan position fixed akan memiliki
          sifat tetap, tanpa ada perubahan bahkan jika halaman website di
          scroll. Berlaku pengaturan left, bottom, top, dan right pada position
          fixed
        </p>

        <div class="fixed">Elemen ini diatur menggunakan posisi fixed</div>
        <br /><br /><br />
        <br /><br /><br />
        <br /><br /><br />
        <br /><br /><br />
        <br /><br /><br />

        <h2>Position absolute;</h2>

        <p>
          Elemen HTML yang menggunakan posisi absolut akan diposisikan relatif
          dengan elemen lain yang mendahuluinya yang terdekat, bukan relatif
          terhadap layar secara normal.
        </p>

        <div class="relative1">
          Elemen ini diatur menggunakan posisi relative
          <div class="absolute">
            Elemen ini diatur menggunakan posisi absolute
          </div>
        </div>

        <br /><br /><br />
        <br /><br /><br />

        <h2>Position: sticky;</h2>

        <p>
          Cobalah untuk <b>Scroll</b> untuk mengetahui bagaimana posisi sticky
          bekerja.
        </p>
        <p>
          Catatan: IE/Edge 15 dan versi yang lebih lama tidak mendukung sticky.
        </p>

        <div class="sticky">Hola Aku adalah sticky!</div>

        <div style="padding-bottom: 2000px;">
          <p>
            Dalam contoh ini, elemen sticky menempel pada posisi paling atas
            halaman (top:0), ketika mencapai posisi scrollnya.
          </p>
          <p>Cobalah untuk melakukan scroll.</p>
          <p>
            Cobalah untuk melakukan scroll. Lorem ipsum dolor sit, amet
            consectetur adipisicing elit. Provident rem expedita consequuntur
            architecto nesciunt soluta quisquam voluptatum, cum hic voluptas
            vitae maxime, sint atque quibusdam saepe pariatur. Veritatis, error
            maiores.
          </p>
          <p>
            Cobalah untuk melakukan scroll. Lorem ipsum dolor sit, amet
            consectetur adipisicing elit. Provident rem expedita consequuntur
            architecto nesciunt soluta quisquam voluptatum, cum hic voluptas
            vitae maxime, sint atque quibusdam saepe pariatur. Veritatis, error
            maiores.
          </p>
        </div>
      </body>
    </html>
    ```

3.  Buat satu file baru bernama `stylePosition.css` di dalam folder dasarWeb
4.  Ketikkan ke dalam file `stylePosition.css` tersebut kode di bawah ini.

    ```css
    div.static {
      position: static;
      border: 3px solid #73ad21;
    }

    div.relative {
      position: relative;
      left: 30px;
      border: 3px solid #73ad21;
    }

    div.fixed {
      position: fixed;
      bottom: 0;
      right: 0;
      width: 300px;
      border: 3px solid #73ad21;
    }

    div.relative1 {
      position: relative;
      width: 400px;
      height: 200px;
      border: 3px solid #73ad21;
    }

    div.absolute {
      position: absolute;
      top: 80px;
      right: 0;
      width: 200px;
      height: 100px;
      border: 3px solid #73ad21;
    }

    div.sticky {
      position: -webkit-sticky;
      position: sticky;
      top: 0;
      background-color: yellow;
      border: 3px solid #73ad21;
    }
    ```

5.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/positionCSS.html](http://localhost/dasarWeb/positionCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![positionCSS.html](/css/img/praktikum10/positionCSS.gif)

6.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Dari halaman html diatas, terdapat lima jenis posisi, yaitu `static`, `relative`, `absolute`, `fixed`, `sticky`.
    - _Static_ adalah posisi pengaturan bawaan / default yang tidak berubah posisinya dan tidak dipengaruhi oleh properti merubah posisi.
    - _Relative_ adalah posisi yang bisa diubah posisinya dengan menggunakan properti merubah posisi tetapi tidak bertabrakan dengan elemen lain dan tetap di posissinya
    - _Fixed_ adalah posisi tetap apabila posisinya berubah dan tidak akan berpindah walaupun discroll
    - _Absolute_ sama dengan relative. Akan tetapi, dengan merubah posisinya dapat bertabrakan / bertindihan dengan elemen lain
    - _Sticky_ adalah posisi yang sama dengan _relative_. Akan tetapi, sticky juga akan menjadi fixed jika posisi sticky berada diatas halaman saat discroll.
    - Dalam implementasi web, posisi dapat diterapkan sesuai kebutuhan
