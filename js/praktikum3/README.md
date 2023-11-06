# Praktikum 3 - Cara Menulis Kode JavaScript di HTML

Pada [praktikum 2](/js/praktikum2/) kita sudah menulis kode javascript di dalam HTML, cara tersebut merupakan cara penulisan embeded (ditempel). Beberapa cara lain yang perlu kita ketahui diantaranya :

1.  [Embed](#penulisan-kode-javascript-dengan-embed) (Kode Javascript ditempel langsung pada HTML)
2.  [Inline](#penulisan-kode-javascript-inline) (Kode Javascript ditulis pada atribut HTML)
3.  [Eksternal](#penulisan-kode-javascript-eksternal) (Kode Javascript ditulis dengan terpisah dengan file HTML)

### Penulisan Kode JavaScript dengan Embed

#### Langkah Praktikum

1.  Pada cara ini, kita menggunakan tag `<script>` untuk menempelkan (_embed_) kode JavaScript pada HTML. Tag ini dapat ditulis didalam tag `<head>` dan `<body>`
2.  Buat satu file baru bernama `embed.html` di dalam folder belajarjavascript
3.  Ketikkan kode program dibawah ini:

    ```html
    <!DOCTYPE html>
    <html>
      <head>
        <title>Belajar JavaScript dari Nol</title>
        <script>
          // Ini adalah penulisan kode javascript
          // di dalam tag <head>
          console.log("Hello JS dari head");
        </script>
      </head>

      <body>
        <p>Tutorial JavaScript untuk Pemula</p>
        <script>
          // Ini adalah penulisan kode javascript
          // di dalam tag <body>
          console.log("Hello JS dari body");
        </script>
      </body>
    </html>
    ```

4.  Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

    Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/embed.html](http://localhost/belajarjavascript/embed.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![Embed Output](/js/img/praktikum3/embed.png)

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Dari program diatas, implementasi javascript secara embed atau menempelkan kode javascript langsung dari HTML
    - Untuk implementasinya, dengan menggunakan tag `<script>` dan ketik kode javascript.
    - Untuk penempatanya bisa di tag `<body>` maupun `<head>`

5.  Menurut Anda manakah yang lebih baik, dituliskan didalam tag `<head>` atau `<body>`?

    - Menurut saya, untuk tag `<script>` lebih baik ditempatkan di `<body>` dibandingkan `<head>`
    - Hal ini karena posisi peletakkan kode javascript bisa mempengaruhi urutan output halaman website
    - Jika ditaruh di `<head>`, maka javascript akan diproses terlebih dahulu sebelum kode html. Jika itu terjadi, maka kemungkinan error besar
    - Oleh karena itu, disarankan dalam implementasi kode javascript di dalam tag `<body>` supaya konten html terlebih dahulu baru kode javascript dijalankan

### Penulisan Kode JavaScript _Inline_

#### Langkah Praktikum

1.  Pada cara ini, kita akan menulis kode javascript di dalam atribut HTML. Cara ini biasanya digunakan untuk memanggil suatu fungsi pada event tertentu. Salah satu contohnya pada saat di-klik.
2.  Buat satu file baru bernama `inline.html` di dalam folder belajarjavascript
3.  Ketikkan kode program dibawah ini:

    ```html
    <a href="#" onclick="alert('Yey!')">Klik aku!</a>
    ```

    Atau bisa juga seperti ini:

    ```html
    <a href="javascript:alert('Yey!')">Klik aku!</a>
    ```

4.  Amati apa yang terjadi pada browser! Catat hasil pengamatanmu

    Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/inline.html](http://localhost/belajarjavascript/inline.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![Inline Output](/js/img/praktikum3/inline.png)

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Implementasi javascript bisa diterapkan dalam elemen html seperti tag `<a>` disertai dengan atribut onclick
    - Dengan begitu, Ketika klik link “**klik aku!**” maka terdapat notifikasi seperti output diatas

5.  Apa yang membedakan dari kedua kode program tersebut
    - Kode pertama menggunakan notifikasi di dalam atribut `onclick` disertai dengan nilai sintaks js: `alert("Yey!")`
    - Sedangkan kode kedua menggunakan notifikasi di dalam atribut `href` disertai dengan nilai `javascript:alert("Yey!")`

### Penulisan Kode JavaScript _Eksternal_

#### Langkah Praktikum

1.  Pada cara ini, kita akan menulis kode javascript secara terpisah dengan file HTML. Cara ini biasanya digunakan pada proyek-proyek besar, karena diyakini dengan cara ini dapat lebih mudah mengelola kode project.
2.  Mari kita coba, buat dua file yaitu file HTML dan JavaScript.
3.  Buat satu file baru bernama `kode-program.js` di dalam folder belajarjavascript
4.  Ketikkan kode program dibawah ini:

    ```js
    alert("Hello, ini adalah program JS eksternal!");
    ```

5.  Buat satu file baru bernama `eksternal.html` di dalam folder belajarjavascript
6.  Ketikkan kode program dibawah ini:

    ```html
    <!DOCTYPE html>
    <html>
      <head>
        <title>Belajar JavaScript dari Nol</title>
      </head>

      <body>
        <p>Tutorial JavaScript untuk Pemula</p>

        <!-- Menyisipkan kode js eksternal -->
        <script src="kode-program.js"></script>
      </body>
    </html>
    ```

7.  Amati apa yang terjadi pada browser! Catat hasil pengamatanmu

    Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/eksternal.html](http://localhost/belajarjavascript/eksternal.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![External Output](/js/img/praktikum3/external.png)

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Penerapan dari javascript bisa ditempatkan di file terpisah / eksternal
    - Dengan begitu, kode html jadi tidak panjang dan bisa modifikasi javascript dengan mudah
    - Untuk penerapan nya sendiri dengan tag `<script>` hanya saja bukan ditulis secara langsung kode javascript nya melainkan menggunakan atribut `src` disertai lokasi file `.js` supaya dapat saling terhubung

8.  Pada percobaan tersebut, kita menulis kode javascript terpisah dengan kode HTML. Lalu pada kode HTML kita menyisipkan atribut src pada tag `<script>`

    ```html
    <!-- Menyisipkan kode js eksternal -->
    <script src="kode-program.js"></script>
    ```

    Maka apapun yang ada di dalam file `kode-program.js` akan dapat dibaca dari file `index.html`

9.  Apa yang akan terjadi jika file javascript berada di folder yang berbeda? Amati dan catat hasil pengamatanmu

    - Jika file javascript berada di folder yang berbeda, maka javascript dan html tidak dapat terhubung
    - Solusinya adalah dengan membuat relative path pada atribut `src` dan cari lokasi tempat file javascript berada
    - Dengan begitu, javascript dan html dapat terhubung walaupun beda folder

10. Misalkan kita memiliki struktur folder seperti ini :

    ![Direktori HTML dan JS](/js/img/praktikum3/direktori2.png)

    Maka untuk menyisipkan file `kode-program.js` ke dalam HTML, kita bisa menuliskan kode berikut :

    ```html
    <script src="js/kode-program.js"></script>
    ```

    Karena file `kode-program.js` berada didalam direktori `js`.

    Kita juga dapat menyisipkan javascript yang ada di internet dengan memberikan alamat URL lengkap

    Contoh:

    ```html
    <script src="https://www.petanikode.com/js/kode.js"></script>
    ```
