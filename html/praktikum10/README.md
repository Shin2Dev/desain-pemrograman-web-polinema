# Praktikum 10 - Link

- Link pada HTML adalah Hyperlink.
- Hyperlink adalah sebuah elemen, teks atau sebuah image yang dapat diklik dan kemudian menuju ke dokumen lain.
- Browser akan menyorot (highlight) teks atau gambar yang diidentifikasi sebagai link dengan warna dan/atau garis bawah untuk menunjukkan bahwa itu adalah hypertext link (hyperlink atau link)
- Sintaks link pada HTML : <br>
  Tag Anchor `<a>` digunakan untuk membuat suatu link kepada dokumen lain dengan menambah atribut href sebagai definisi lokasi link.

  ```html
  <a href="url">teks yang mengandung link</a>
  ```

- Atribut `href` memberikan alamat tujuan link
- Teks yang mengandung link adalah tulisan yang akan tampak pada halaman web yang berisi link, dan jika diklik maka halaman akan menuju ke alamat yang ada di dalam atribut `href`.
- Contoh :
  ```html
  <a href="http://www.microsoft.com">click here to show it</a>
  ```
- Macam-macam Link :

  - Link Relative

    Link lokal yang memberikan link ke dalam website yang sama yang dispesifikasikan dengan sebuah URL (tanpa `http://www.`)

  - Link Absolute

    Digunakan untuk membuat link ke halaman web lain yang berada pada website lain di internet.

  - Link dalam Dokumen yang Sama

    Link ini dibuat untuk dokumen yang panjang sekali, sehingga apabila ditampilkan dalam browser web akan mengharuskan kita melakukan scroll layar berulang-ulang.

    Navigasi untuk penelusuran dokumen dapat dimudahkan dengan membuat link antar bagian dengan menandai setiap bagian tersebut dengan memberinya nama, sehingga pada tempat di dalam dokumen akan ada bagian yang bernama dan di bagian lainnya dapat diletakkan link untuk menuju ke bagian-bagian tersebut.

    Langkah-langkah memberi nama suatu bagian dalam dokumen :

    - Letakkan kursor pada baris atau teks yang menjadi awal dari bagian tersebut
    - Sisipkan nama bagian tersebut dengan : `<a name="nama bagian">`
    - Membuat link yang menuju pada bagian dokumen yang sama dapat dilakukan dengan cara yang sama seperti link absolut atau relatif, namun nama dokumen dalam link diganti dengan nama_bagian dokumen dengan ditambah tanda # yang ditulis sebelum nama bagian tersebut. <br>
      Contoh : `<a href = "#nama bagian">Bagian tentang link </a>`

### Langkah Praktikum

1.  Buat sebuah file bernama `macamLink.html` dan simpan file tersebut di dalam folder dasarWeb.
2.  Ketikkan kode di bawah ini dalam `macamLink.html`

    ```html
    <html>
      <head>
        <title>Membuat Link</title>
      </head>

      <body>
        <a name="TOP">
          <h4>Macam-Macam Link</h4>
          <a href="#Link Relatif">Link Relatif</a> <br />
          <a href="#Link Absolut">Link Absolut</a> <br />
          <a href="#Link with New Window">Link with New Window</a> <br />
          <a href="#Link ke Email">Link ke Email</a>
        </a>
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <br />
        <a name="Link Relatif">
          <h1>Ini adalah contoh Link Relatif</h1>
          <p>
            Klik <a href="gambar.html">di sini</a> Jika anda ingin menuju ke
            halaman berikutnya. <br />
            <br />
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Veritatis
            iure doloremque dolores quisquam quo dolorem! Accusamus, nisi,
            excepturi beatae saepe soluta odio dolor omnis, aliquid suscipit
            quod molestias ducimus numquam! Lorem ipsum dolor sit amet
            consectetur adipisicing elit. Enim molestias impedit numquam rerum
            cum perferendis temporibus fugiat debitis nisi velit dicta itaque
            vero eos reiciendis, officia, commodi incidunt ex pariatur! <br />
            <br />
            <br />
            <br />
            <br />
            <br />
            <br />
            <br />
            <br />
            <br />
            <a href="#TOP">Kembali ke Menu</a>
          </p>
        </a>
        <br />
        <br />
        <a name="Link Absolut">
          <h1>Ini adalah contoh Link Absolut</h1>
          <p>
            Klik <a href="http://www.google.com">di sini</a> untuk pencarian
            yang Anda inginkan.<br />
            <br />
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Veritatis
            iure doloremque dolores quisquam quo dolorem! Accusamus, nisi,
            excepturi beatae saepe soluta odio dolor omnis, aliquid suscipit
            quod molestias ducimus numquam! Lorem ipsum dolor sit amet
            consectetur adipisicing elit. Enim molestias impedit numquam rerum
            cum perferendis temporibus fugiat debitis nisi velit dicta itaque
            vero eos reiciendis, officia, commodi incidunt ex pariatur! <br />
            <br />
            <br />
            <br />
            <br />
            <br />
            <br />
            <br />
            <br />
            <br />
            <a href="#TOP">Kembali ke Menu</a>
          </p>
        </a>
        <br />
        <br />
        <a name="Link with New Window">
          <h1>Ini adalah contoh Link with New Window</h1>
          <p>
            Buka
            <a href="http://www.google.com" target="_blank"
              >http://www.google.com</a
            >
            di halaman baru.<br />
            <br />
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Veritatis
            iure doloremque dolores quisquam quo dolorem! Accusamus, nisi,
            excepturi beatae saepe soluta odio dolor omnis, aliquid suscipit
            quod molestias ducimus numquam! Lorem ipsum dolor sit amet
            consectetur adipisicing elit. Enim molestias impedit numquam rerum
            cum perferendis temporibus fugiat debitis nisi velit dicta itaque
            vero eos reiciendis, officia, commodi incidunt ex pariatur! <br />
            <br />
            <br />
            <br />
            <br />
            <br />
            <a href="#TOP">Kembali ke Menu</a> <br />
            <br />
            <br />
            <br />
            <br />
            <br />
            <br />
          </p>
        </a>
        <a name="Link ke Email">
          <h1>Ini adalah contoh Link ke Email</h1>
          <p>
            Anda bisa menghubungi saya di
            <a href="mailto:hapeoppojoy3@gmail.com">email ini</a> untuk
            pertanyaan lebih lanjut.<br />
            <br />
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Veritatis
            iure doloremque dolores quisquam quo dolorem! Accusamus, nisi,
            excepturi beatae saepe soluta odio dolor omnis, aliquid suscipit
            quod molestias ducimus numquam! Lorem ipsum dolor sit amet
            consectetur adipisicing elit. Enim molestias impedit numquam rerum
            cum perferendis temporibus fugiat debitis nisi velit dicta itaque
            vero eos reiciendis, officia, commodi incidunt ex pariatur!
          </p>
        </a>
        <br />
        <br />
        <a href="#TOP">Kembali ke Menu</a>
      </body>
    </html>
    ```

3.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/macamLink.html](http://localhost/dasarWeb/macamLink.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![macamLink.html](/html/img/praktikum10/macamLink.gif)

4.  Amati apa yang tampil pada browser dan bagaimana tiap link bekerja. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Terdapat empat link, Relative, Absolute, With New Window, dan Email.
    - **_Link Relative_** adalah link yang akan merujuk ke lokal direktori yang dimana letak dari halaman html yang lain sehingga halaman berganti. Seperti contoh diatas jika diklik maka akan beralih ke halaman `gambar.html`.
    - **_Link Absolute_** adalah link yang merujuk ke web lain seperti contoh diatas jika diklik maka beralih ke laman [google.com](https://www.google.com).
    - **_Link with new window_** adalah link yang akan dibuka ke halaman baru. Cara ini bisa diterapkan oleh link Absolute maupun Link Relative. Untuk penerapannya memakai atribut `target=_blank`. Contohnya seperti diatas.
    - **_Link ke Email_** adalah link yang akan merujuk ke email yang dituju seperti contoh diatas.
    - **_Link yang berada dalam kalimat “Kembali ke Menu”_** adalah link yang menuju ke dokumen yang sama. Jika diklik maka akan merujuk ke nama yang sesuai. Contoh di halaman paling atas terdapat elemen atribut name yang dimana menjadi bookmark / penanda link. Setelah itu, buatlah link dengan merujuk ke elemen yang terdapat atribut name dan jika diklik, halaman akan berada di elemen tersebut.
    - Untuk nilai dari atribut name harus sesuai penamaan, jika tidak maka hubungan dari kedua link tidak terhubung
    - Untuk pembuatan link menggunakan tag `<a>` disertai atribut `href`.
    - Jika tidak pernah diklik / buat link baru maka link berwarna biru, dan jika sudah pernah diklik maka warna link lebih gelap.

# Tugas Praktikum 10

Buat sebuah halaman, beri nama `tugasLink.html` <br>
Tampilkan sebuah gambar yang mengandung link ke http://www.google.com.

1.  Buat sebuah file bernama tugasLink.html dan simpan file tersebut di dalam folder dasarWeb dan ketikkan kode untuk menampilkan gambar yang mengandung link ke http://www.google.com.

    ```html
    <html>
      <head>
        <title>Tugas Link Gambar</title>
      </head>

      <body>
        <p>Link menuju <b>Google</b> dengan klik gambar dibawah</p>
        <a href="http://www.google.com" target="_blank">
          <img src="img/google.png" width="100" />
        </a>
      </body>
    </html>
    ```

2.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/tugasLink.html](http://localhost/dasarWeb/tugasLink.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![tugasLink.html](/html/img/praktikum10/tugasLink.png)
