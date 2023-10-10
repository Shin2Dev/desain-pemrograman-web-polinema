# Praktikum 3 - Format Teks

HTML menyediakan beragam elemen yang dapat dimanfaatkan untuk pemformatan teks.

### Heading

Heading merupakan salah satu elemen penting di dalam dokumen HTML. Heading didefinisikan menggunakan tag `<hn>` dan diakhiri dengan `</hn>`, di mana n menyatakan tipe dengan nilai 1 - 6.

#### Langkah Praktikum

1.  Buat sebuah file bernama `heading.html` dan simpan file tersebut di dalam folder dasarWeb.
2.  Ketikkan kode di bawah ini dalam `heading.html`

    ```html
    <html>
      <body>
        <h1>Heading 1</h1>
        <h2>Heading 2</h2>
        <h3>Heading 3</h3>
        <h4>Heading 4</h4>
        <h5>Heading 5</h5>
        <h6>Heading 6</h6>
      </body>
    </html>
    ```

3.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/heading.html](http://localhost/dasarWeb/heading.html).

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![heading.html](/html/img/praktikum3/heading.png)

4.  Amati apa yang muncul pada browser. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Semua tulisan yang ada didalam halaman tersebut dicetak **tebal** karena tulisan tersebut diapit oleh tag `<hn>` yang dimana tag ini adalah heading atau judul yang mewakili elemen penting di dalam dokumen HTML.
    - Heading juga terdapat hierarki yang dimulai `<h1>` yaitu judul utama halaman, `<h2>` yaitu sub judul dari halaman, hingga `<h6>`.
    - Karena hierarki inilah mengapa jika mengimplentasikan heading mulai `<h1>` hingga `<h6>` akan tampil semakin mengecil

5.  Tambahkan atribut `align` di dalam tag heading seperti di bawah ini dan simpan file dengan nama `headingAlign.html`

    ```html
    <html>
      <body>
        <h1 align="right">Heading 1</h1>
        <h2 align="left">Heading 2</h2>
        <h3 align="center">Heading 3</h3>
        <h4>Heading 4</h4>
        <h5>Heading 5</h5>
        <h6>Heading 6</h6>
      </body>
    </html>
    ```

6.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/headingAlign.html](http://localhost/dasarWeb/headingAlign.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![headingAlign.html](/html/img/praktikum3/headingAlign.png)

7.  Amati apa yang muncul pada browser. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Sama seperti `heading.html`, akan tetapi perbedaan nya adalah align atau pengaturan rata teks/kalimat dalam html.
    - Dari halaman diatas, heading 1 diatur rata kanan, heading 2 diatur rata kiri atau pengaturan bawaan, dan heading 3 diatur rata tengah. Sedangkan heading 4-6 tidak menerapkan align.

### Paragraf

Sebagaimana teks pada umumnya, dokumen HTML dapat terdiri dari kumpulan paragraf. Dalam konteks HTML, paragraf direpresentasikan dengan tag `<p>`. Tag `<p>` sebenarnya merupakan tag pasangan, meski dalam implementasinya kerap kali diabaikan.

#### Langkah Praktikum

1.  Buat sebuah file bernama `paragraf.html` dan simpan file tersebut di dalam folder dasarWeb
2.  Ketikkan kode di bawah ini dalam `paragraf.html`

    ```html
    <html>
      <body>
        <p>ini paragraf pertama</p>
        <p>
          ini paragraf kedua kedua kedua kedua kedua kedua kedua kedua kedua
          kedua kedua kedua kedua kedua kedua kedua kedua
        </p>
        <p>ini paragraf ketiga</p>
      </body>
    </html>
    ```

3.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/paragraf.html](http://localhost/dasarWeb/paragraf.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![paragraf.html](/html/img/praktikum3/paragraf.png)

4.  Amati apa yang muncul pada browser. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - `<p>` berfungsi untuk mempresentasikan paragraf dalam html, didalam halaman tersebut terdapat tiga paragraf.
    - Didalam paragraf dua, walaupun dalam kalimat nya panjang dan diketik dengan dua baris, tetapi tidak dibuat baris baru dan menyambung menjadi satu.

5.  Untuk mengatur posisi paragraf dengan memanfaatkan atribut `align` yang diletakkan dalam tag paragraf.
6.  Tambahkan atribut `align` di dalam tag paragraf seperti di bawah ini dan simpan file dengan nama `paragrafAlign.html`

    ```html
    <html>
      <head>
        <title>Mengatur Paragraf</title>
      </head>

      <body>
        <p align="right">ini paragraf pertama</p>
        <p align="center">
          ini paragraf kedua kedua kedua kedua kedua kedua kedua kedua kedua
          kedua kedua kedua kedua kedua kedua kedua kedua
        </p>
        <p align="left">ini paragraf ketiga</p>
      </body>
    </html>
    ```

7.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/paragrafAlign.html](http://localhost/dasarWeb/paragrafAlign.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![paragrafAlign.html](/html/img/praktikum3/paragrafAlign.png)

8.  Amati apa yang muncul pada browser. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Sama dengan hasil yang terdapat di `paragraf.html`. Yang membedakan adalah setiap paragraf mempunyai perataan paragraf yang berbeda-beda.
