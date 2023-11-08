# Praktikum 7 - Tipe Data

Tipe data adalah jenis-jenis data yang bisa kita simpan di dalam variabel. <br>
Ada beberapa tipe data dalam pemrograman JavaScript:

- String (teks)
- Integer atau Number (bilangan bulat)
- Float (bilangan Pecahan)
- Boolean
- Object

JavaScript adalah bahasa yang bersifat _dynamic typing_, artinya kita tidak harus menuliskan tipe data pada saat pembuatan variabel seperti pada bahasa **C**, **C++**, **Java**, dsb. yang bersifat _static typing_.

Ada beberapa aturan penulisan variabel dalam JavaScript:

- Penamaan variabel **tidak boleh** menggunakan angka di depannya. <br>
  contoh:

  ```js
  // salah
  var 123nama = "Polinema";

  // benar
  var nama123 = "Polinema";
  ```

- Penamaan variabel **boleh** menggunakan awal underscore. <br> contoh:

  ```js
  var _nama = "Polinema";
  ```

- Penamaan variabel **dianjurkan** menggunakan **camelCase** apabila tediri dari dua suku kata. <br>
  Contoh:

  ```js
  var fullName = "Polinema";
  ```

- Penamaan variabel **dianjurkan** menggunakan bahasa inggris <br>
  Contoh:

  ```js
  var postTitle = "Tutorial Javascript untuk Pemula";
  ```

### Tipe Data

#### Langkah Praktikum

1. Buat File baru bernama `tipedata_javascript.html` dan simpan dalam direktori belajarjavascript
2. Ketikkan kode program dibawah ini:

   ```html
   <!DOCTYPE html>
   <html>
     <body>
       <h2>JavaScript Data Types</h2>
       <p>Contoh JavaScript Data Types:</p>
       <p id="demo"></p>

       <script>
         var x; // Now x is Undefined
         x = 5; // Now x is a Number
         x = "John"; // Now x is a String

         document.getElementById("demo").innerHTML = x;
       </script>
     </body>
   </html>
   ```

3. Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

   Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/tipedata_javascript.html](http://localhost/belajarjavascript/tipedata_javascript.html)

   **Pastikan XAMPP Apache dalam keadaan hidup**

   ![tipedata_javascript](/js/img/praktikum7/datatypes.png)

   Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

   - Dalam menerapkan variabel, variabel bisa bernilai bebas / tidak terikat dengan tipe data spesifik
   - Variabel juga bisa berubah nilai dikarenakan pendeklarasian baru.
   - Contoh `var x` sudah dideklarasikan dan nilai `5`, setelahnya `x` dideklarasikan lagi dan bernilai `John` sehingga secara tidak langsung nilai dari `x` berubah

### String

#### Langkah Praktikum

1. Buat File baru bernama `string_javascript.html` dan simpan dalam direktori belajarjavascript
2. Ketikkan kode program dibawah ini:

   ```html
   <!DOCTYPE html>
   <html>
     <body>
       <h2>JavaScript Strings</h2>
       <p>Membuat JavaScript String</p>
       <p id="demo"></p>

       <script>
         var answer1 = "It's alright";
         var answer2 = "He is called 'Dilan'";
         var answer3 = 'He is called "Dilan"';

         document.getElementById("demo").innerHTML =
           answer1 + "<br>" + answer2 + "<br>" + answer3;
       </script>
     </body>
   </html>
   ```

3. Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

   Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/string_javascript.html](http://localhost/belajarjavascript/string_javascript.html)

   **Pastikan XAMPP Apache dalam keadaan hidup**

   ![string_javascript](/js/img/praktikum7/string.png)

   Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

   - Dalam menampilkan output di halaman html, bisa menggunakan penerapan `innerHTML`
   - Dalam penerapannya, pertama buat deklarasi tag `<p>` disertai atribut `id` dan beri nilai
   - Setelah itu, buat deklarasi `document.getElementById(“nilai”).innerHTML` untuk mengambil `id` dari elemen sebelumnya
   - Setelah itu beri nilai nya dengan variabel yang dideklarasikan dan hasilnya elemen `p` tadi nya kosong menjadi ber isi

### Boolean

#### Langkah Praktikum

1. Buat File baru bernama `boolean_javascript.html` dan simpan dalam direktori belajarjavascript
2. Ketikkan kode program dibawah ini:

   ```html
   <!DOCTYPE html>
   <html>
     <body>
       <h2>JavaScript Booleans</h2>
       <p>Booleans hanya memiliki nilai true dan false</p>
       <p id="demo"></p>
       <script>
         var x = 5;
         var y = 5;
         var z = 6;

         document.getElementById("demo").innerHTML =
           (x == y) + "<br>" + (x == z);
       </script>
     </body>
   </html>
   ```

3. Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

   Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/boolean_javascript.html](http://localhost/belajarjavascript/boolean_javascript.html)

   **Pastikan XAMPP Apache dalam keadaan hidup**

   ![boolean_javascript](/js/img/praktikum7/boolean.png)

   Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

   - `InnerHTML` juga bisa diberi nilai `Boolean` atau operasi logika

### Array

#### Langkah Praktikum

1. Buat File baru bernama `array_javascript.html` dan simpan dalam direktori belajarjavascript
2. Ketikkan kode program dibawah ini:

   ```html
   <!DOCTYPE html>
   <html>
     <body>
       <h2>JavaScript Arrays</h2>
       <p>Array</p>
       <p id="demo"></p>
       <script>
         var cars = ["Satu", "Dua", "Tiga"];
         document.getElementById("demo").innerHTML = cars[0];
       </script>
     </body>
   </html>
   ```

3. Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

   Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/array_javascript.html](http://localhost/belajarjavascript/array_javascript.html)

   **Pastikan XAMPP Apache dalam keadaan hidup**

   ![array_javascript](/js/img/praktikum7/array.png)

   Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

   - Variabel juga selain bisa diisi `string`, `int`, dan `Boolean`, variabel juga bisa diisi dengan `array`
   - Untuk menampilkan nilai `array`, bisa menggunakan nama `array` dan berada di index yang diinginkan
