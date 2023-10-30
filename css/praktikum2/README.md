# Praktikum 2 - Penggunaan div

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Tag `<div>` mendefinisikan sebuah bagian dalam dokumen `HTML`. Elemen `<div>` sering digunakan sebagai sebuah kontainer untuk elemen `HTML` lain untuk menambahkan `style` dengan `CSS` atau untuk menampilkan tugas tertentu menggunakan JavaScript.

### Langkah Praktikum

1.  Buat satu file baru bernama `div.html` di dalam folder dasarWeb
2.  Ketikkan ke dalam file `div.html` tersebut kode di bawah ini.

    ```html
    <html>
      <body>
        <p>Ini adalah beberapa teks.</p>

        <div style="background-color: lightblue;">
          <h3>Ini adalah sebuah heading di dalam elemen div</h3>
          <p>Ini adalah teks di dalam div.</p>
        </div>

        <p>This is some text.</p>
      </body>
    </html>
    ```

3.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/div.html](http://localhost/dasarWeb/div.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![div.html](/css/img/praktikum2/div.png)

4.  Apa yang anda pahami dari penggunaan div pada file tersebut. Catat di bawah ini pemahaman anda

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Untuk menggunakan css, tidak harus membuat file css dan menyambungkannnya. Anda bisa langsung menyisipkan css di dalam html secara _inline_ / sebaris.
    - Untuk mengimplementasikan css _inline_, menggunakan atribut `style` dan tulis properti css seperti contoh didalam `div`, setelah membuat atribut selanjutnya menulis properti `background-color` dan nilainya adalah `lightblue` sehingga warna dari `div` menjadi biru muda.
    - Fungsi dari `div` adalah sebagai wadah kosong sehingga cocok untuk mengimplementasikan sebagian elemen untuk diterapkan css.
