# Praktikum 10 - Perulangan

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Perulangan akan membantu kita mengeksekusi kode yang berulang-ulang, berapapun yang kita mau. Ada lima macam bentuk perulangan di JavaScript. Secara umum, perulangan ini dibagi dua. Yaitu: _counted loop_ dan _uncounted loop_.

Perbedaanya:

- **Counted Loop** merupakan perulangan yang jelas dan sudah tentu banyak perulangannya.
- Sedangkan **Uncounted Loop**, merupakan perulangan yang tidak jelas berapa kali ia harus mengulang.

Perulangan yang termasuk dalam _Counted Loop_:

1. Perulangan For
2. Perulangan Foreach
3. Perulangan Repeat

Perulangan yang termasuk dalam _Uncounted Loop_:

1. Perulangan While
2. Perulangan Do/While

### Perulangan For di JavaScript

Perulangan for merupakan perulangan yang termasuk dalam _counted loop_, karena sudah jelas berapa kali ia akan mengulang.

Bentuknya seperti ini:

```js
for (let i = 0; i < 10; i++) {
  document.write("<p>Perulangan ke-" + i + "</p>");
}
```

#### Langkah Praktikum

1.  Buat File baru bernama `for_javascript.html` dan simpan dalam direktori belajarjavascript
2.  Ketikkan kode program dibawah ini:

    ```html
    <!DOCTYPE html>
    <html>
      <body>
        <h2>JavaScript Loops</h2>
        <p id="demo"></p>
        <script>
          var text = "";
          var i;
          for (i = 0; i < 5; i++) {
            text += "The number is " + i + "<br>";
          }
          document.getElementById("demo").innerHTML = text;
        </script>
      </body>
    </html>
    ```

3.  Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

    Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/for_javascript.html](http://localhost/belajarjavascript/for_javascript.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![for_javascript.html](/js/img/praktikum10/for.png)

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Dalam tampilan tersebut, kalimat **the number** akan diulangi dimulai dari i = 0 hingga i kurang dari 5 yaitu 4
    - Dengan kata lain akan diulangi hingga 5 kali yang dimulai dari 0 sampai 4

### Perulangan While di JavaScript

Perulangan while merupakan perulangan yang termasuk dalam perulangan _uncounted loop_. Perulangan while juga dapat menjadi perulangan yang _counted loop_ dengan memberikan counter di dalamnya

#### Langkah Praktikum

1.  Buat File baru bernama `while_javascript.html` dan simpan dalam direktori belajarjavascript
2.  Ketikkan kode program dibawah ini:

    ```html
    <!DOCTYPE html>
    <html>
      <body>
        <h2>JavaScript While</h2>
        <p id="demo"></p>
        <script>
          var text = "";
          var i = 0;
          while (i < 10) {
            text += "The number is " + i + "<br>";
            i++;
          }
          document.getElementById("demo").innerHTML = text;
        </script>
      </body>
    </html>
    ```

3.  Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

    Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/while_javascript.html](http://localhost/belajarjavascript/while_javascript.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![while_javascript.html](/js/img/praktikum10/while.png)

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - _While_ akan mengecek apakah i kurang dari 10, jika **iya** maka program akan mengulangi kalimat **The number** hingga i melebihi / sama dengan 10
    - Pada saat pengulangan, program melakukan _increment_ supaya i bertambah.
    - Jika tidak melakukan _increment_, maka while akan **true** sehingga output nya menjadi tidak terhingga

      <img src="/js/img/praktikum10/takterbatas.jpg" width="20%" alt="Tak Terbatas">

### Perulangahn Do/While di JavaScript

Perulangan do/while sama seperti perulangan while. Perbedaanya:

Perulangan do/while akan melakukan perulangan sebanyak 1 kali terlebih dahulu, lalu mengecek kondisi yang ada di dalam kurung while

Bentuknya seperti ini:

```js
do {
  // blok kode yang akan diulang
} while (<kondisi>)
```

#### Langkah Praktikum

1.  Buat File baru bernama `dowhile_javascript.html` dan simpan dalam direktori belajarjavascript
2.  Ketikkan kode program dibawah ini:

    ```html
    <!DOCTYPE html>
    <html>
      <body>
        <h2>JavaScript Do... While</h2>
        <p id="demo"></p>
        <script>
          var text = "";
          var i = 0;
          do {
            text += "The number is " + i + "<br>";
            i++;
          } while (i < 10);
          document.getElementById("demo").innerHTML = text;
        </script>
      </body>
    </html>
    ```

3.  Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

    Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/dowhile_javascript.html](http://localhost/belajarjavascript/dowhile_javascript.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![dowhile_javascript.html](/js/img/praktikum10/dowhile.png)

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Bedanya while dengan do while adalah eksekusi perulangannya
    - While akan dieksekusi jika keadaannya menjadi **true** terlebih dahulu lalu mulai perulangan
    - Sedangkan do while akan dieksekusi terlebih dahulu dan mulai perulangan dan _increment_ lalu barulah akan melakukan pengecekan true / false
