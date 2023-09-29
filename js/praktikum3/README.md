# Praktikum 3 - Cara Menulis Kode JavaScript di HTML

Pada [praktikum 2](/js/praktikum2/) kita sudah menulis kode javascript di dalam HTML, cara tersebut merupakan cara penulisan embeded (ditempel). Beberapa cara lain yang perlu kita ketahui diantaranya :

1.  [Embed](/js/praktikum3#penulisan-kode-javascript-dengan-embed) (Kode Javascript ditempel langsung pada HTML)
2.  [Inline](/js/praktikum3#penulisan-kode-javascript-inline) (Kode Javascript ditulis pada atribut HTML)
3.  [Eksternal](/js/praktikum3#penulisan-kode-javascript-eksternal) (Kode Javascript ditulis dengan terpisah dengan file HTML)

### Penulisan Kode JavaScript dengan Embed

1.  Pada cara ini, kita menggunakan tag `<script>` untuk menempelkan (_embed_) kode JavaScript pada HTML. Tag ini dapat ditulis didalam tag `<head>` dan `<body>`
2.  Ketikkan kode program dibawah ini:

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

3.  Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

    ![Embed Output](/js/praktikum3/img/embed.png)

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Dari program diatas, implementasi javascript secara embed atau menempelkan kode javascript langsung dari HTML
    - Untuk implementasinya, dengan menggunakan tag `<script>` dan ketik kode javascript.
    - Untuk penempatanya bisa di tag `<body>` maupun `<head>`

4.  Menurut Anda manakah yang lebih baik, dituliskan didalam tag `<head>` atau `<body>`?

    - Menurut saya, untuk tag `<script>` lebih baik ditempatkan di `<body>` dibandingkan `<head>`
    - Hal ini karena posisi peletakkan kode javascript bisa mempengaruhi urutan output halaman website
    - Jika ditaruh di `<head>`, maka javascript akan diproses terlebih dahulu sebelum kode html. Jika itu terjadi, maka kemungkinan error besar
    - Oleh karena itu, disarankan dalam implementasi kode javascript di dalam tag `<body>` supaya konten html terlebih dahulu baru kode javascript dijalankan

### Penulisan Kode JavaScript _Inline_

1.  Pada cara ini, kita akan menulis kode javascript di dalam atribut HTML. Cara ini biasanya digunakan untuk memanggil suatu fungsi pada event tertentu. Salah satu contohnya pada saat di-klik.
2.  Ketikkan kode program dibawah ini:

    ```html
    <a href="#" onclick="alert('Yey!')">Klik aku!</a>
    ```

    Atau bisa juga seperti ini:

    ```html
    <a href="javascript:alert('Yey!')">Klik aku!</a>
    ```

3.  Amati apa yang terjadi pada browser! Catat hasil pengamatanmu

    ![Inline Output](/js/praktikum3/img/inline.png)

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Implementasi javascript bisa diterapkan dalam elemen html seperti tag `<a>` disertai dengan atribut onclick
    - Dengan begitu, Ketika klik link “**klik aku!**” maka terdapat notifikasi seperti output diatas

4.  Apa yang membedakan dari kedua kode program tersebut
    - Kode pertama menggunakan notifikasi di dalam atribut `onclick` disertai dengan nilai sintaks js: `alert("Yey!")`
    - Sedangkan kode kedua menggunakan notifikasi di dalam atribut `href` disertai dengan nilai `javascript:alert("Yey!")`

### Penulisan Kode JavaScript _Eksternal_

1.  Pada cara ini, kita akan menulis kode javascript secara terpisah dengan file HTML. Cara ini biasanya digunakan pada proyek-proyek besar, karena diyakini dengan cara ini dapat lebih mudah mengelola kode project.
2.  Mari kita coba, buat dua file yaitu file HTML dan JavaScript.
3.  Isi dari file `kode-program.js`

    ```js
    alert("Hello, ini adalah program JS eksternal!");
    ```

4.  Isi dari file `index.html`

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

5.  Amati apa yang terjadi pada browser! Catat hasil pengamatanmu

    ![External Output](/js/praktikum3/img/external.png)

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Penerapan dari javascript bisa ditempatkan di file terpisah / eksternal
    - Dengan begitu, kode html jadi tidak panjang dan bisa modifikasi javascript dengan mudah
    - Untuk penerapan nya sendiri dengan tag `<script>` hanya saja bukan ditulis secara langsung kode javascript nya melainkan menggunakan atribut `src` disertai lokasi file `.js` supaya dapat saling terhubung

6.  Pada percobaan tersebut, kita menulis kode javascript terpisah dengan kode HTML. Lalu pada kode HTML kita menyisipkan atribut src pada tag `<script>`

    ```html
    <!-- Menyisipkan kode js eksternal -->
    <script src="kode-program.js"></script>
    ```

    Maka apapun yang ada di dalam file `kode-program.js` akan dapat dibaca dari file `index.html`

7.  Apa yang akan terjadi jika file javascript berada di folder yang berbeda? Amati dan catat hasil pengamatanmu
    - Jika file javascript berada di folder yang berbeda, maka javascript dan html tidak dapat terhubung
    - Solusinya adalah dengan membuat relative path pada atribut `src` dan cari lokasi tempat file javascript berada
    - Dengan begitu, javascript dan html dapat terhubung walaupun beda folder
