# Praktikum 7 - Menggunakan List

HTML mendukung list dalam bentuk terurut (ordered), tak terurut (unordered) dan definisi (definition). Untuk setiap bentuk list ini, terdapat list item yang dinyatakan dengan tag `<li>` dan `</li>` yang merepresentasikan item-item list.

### Langkah Praktikum

1.  Buat sebuah file bernama `list.html` dan simpan file tersebut di dalam folder dasarWeb.
2.  Ketikkan kode di bawah ini dalam `list.html`

    ```html
    <html>
      <head>
        <title>Bekerja dengan List</title>
      </head>

      <body>
        Ordered List
        <ol>
          <li>satu</li>
          <li>dua</li>
          <li>tiga</li>
        </ol>
        <br />
        <hr />
        Unordered List
        <ul>
          <li>satu</li>
          <li>dua</li>
          <li>tiga</li>
        </ul>
        <br />
        <hr />
        Definition List
        <dl>
          <dt>satu</dt>
          <dd>satu satu</dd>
          <dd>satu dua</dd>
          <dt>dua</dt>
          <dd>dua dua</dd>
        </dl>
      </body>
    </html>
    ```

3.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/list.html](http://localhost/dasarWeb/list.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![list.html](/html/img/praktikum7/list.png)

4.  Amati apa yang muncul pada browser. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Dalam mengimplementasikan list, terdapat tiga jenis list yaitu Ordered, Unordered, dan Definition List.
    - Ordered list `<ol>`, yaitu daftar yang terurut dan pengaturan bawaan nya adalah list dimulai dari satu (1) hingga sebanyak daftar tersebut.
    - Unordered list `<ul>`, yaitu daftar yang tidak terurut dan pengaturan bawaan nya adalah untuk list ditandai dengan bulat hitam kecil.
    - Ordered list dan Unordered list mempunyai definisi daftar nya yaitu tag `<li>`.
    - Definition list `<dl>`, yaitu daftar yang didefinisikan dengan deskripsi atau daftar penjelasan. Jika diimplementasikan seperti halaman diatas, satu dan dua yang didefinisikan dengan tag `<dt>` adalah judul dari daftar dan satu satu, satu dua, dua dua yang didefinisikan dengan tag `<dd>` adalah daftar penjelasan tersebut.
