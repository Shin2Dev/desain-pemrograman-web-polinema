# Praktikum 12 - Bekerja dengan Form pada HTML

Form merupakan tempat penginputan data sebelum diproses oleh sistem. salah satunya adalah form login, form comment, form data user, dan lain sebagainya. untuk proses penginputan data dari form akan kita bahas di materi PHP, MYSQL, dan JavaScript. tag yang digunakan untuk membuat form ini adalah tag `<form>` yang didalamnya bisa berupa `<input>`, `<textarea>`, `<option>` dan `<select>`.

Form memiliki atribut berupa `action` dan `method`. Atribut `action` menentukan URL yang akan dijalankan dan menerima semua masukan pada formulir. Jika action tidak disebutkan akan dikirim ke URL yang sama dengan halaman web itu sendiri, sedangkan atribut `method` berisikan metode form melakukan proses pengiriman (GET/POST).

- **GET** -> informasi dikirim dengan URLnya
- **POST** -> informasi dikirim terpisah dengan URLnya.

Sintaks:

```html
<form action="action" method="GET|POST">......</form>
```

### Elemen INPUT

Elemen `input` berfungsi untuk mendefinisikan input yang akan dimasukkan pengguna. Elemen ini mempunyai atribut yaitu `name`, `size`, `type`, `value`, `checked`.

- `name` mendefinisikan nama dari input kontrol form
- `size` mendefinisikan ukuran teks pada input kontrol
- `type` mendefinisikan bentuk-bentuk input kontrol
- `value` mendefinisikan nilai awal/reset/submit
- `checked` mendefinisikan pilihan terpilih pada type radio/checkbox.

Elemen ini tidak mempunyai tag penutup dan harus berada di dalam elemen `FORM`.

Sintaks:

```html
<input
  name="name"
  size="number"
  type="value"
  value="isi yang ditampilkan di browser"
  checked
/>
```

Atribut type dapat berisi:
| Value | Deskripsi |
|-------|-----------|
| button | Mendefinisikan sebuah tombol yang bisa diklik (biasanya digunakan dengan sebuah script Javascript) |
| checkbox |Mendefinisikan sebuah checkbox |
| color (HTML5) | Mendefinisikan _color picker_ |
| date (HTML5) | Mendefinisikan pengaturan tanggal (year, month, day(no time)) |
| datetime-local (HTML5) | Mendefinisikan sebuah pengaturan tanggal dan waktu (year, month, day, time (no timezone)) |
| email (HTML5) | Mendefinisikan sebuah tempat untuk sebuah alamat email. |
| file | Mendefinisikan sebuah area untuk memilih sebuah file dan sebuah tombol “**Browse**” (untuk upload file) |
| hidden | Mendefinisikan sebuah area input yang disembunyikan |
| image | Mendefinisikan sebuah gambar sebagai tombol
| month (HTML5) | Mendefinisikan sebuah pengaturan bulan dan tahun (no timezone) |
| number (HTML5) | Mendefinisikan sebuah area untuk memasukkan sebuah angka |
| password | Mendefinisikan sebuah area password |
| radio | Mendefinisikan sebuah radio button |
| range (HTML5) | Mendefinisikan sebuah pengaturan _range_ (seperti _slide control_) |
| reset | Mendefinisikan tombol reset |
| search (HTML5) | Mendefinisikan sebuah text area untuk memasukkan string pencarian |
| submit | Mendefinisikan tombol submit |
| tel (HTML5) | Mendefinisikan text area untuk memasukkan sebuah nomor telepon |
| text | Default. Mendefinisikan sebuah text area satu baris. |
| time (HTML5) | Mendefinisikan sebuah pengaturan untuk memasukkan waktu (no timezone) |
| url (HTML5) | Mendefinisikan sebuah area untuk memasukkan alamat URL |
| week | Mendefinisikan sebuah pengaturan minggu dan tahun (no timezone) |

### Elemen SELECT

Elemen `select` berfungsi untuk mendefinisikan opsi pilihan pada form kontrol. Element ini mempunyai attribute yaitu `name`, `size`, `multiple` (diizinkan banyak pilihan). Element ini harus berada di dalam elemen `FORM`.

Sintaks :

```html
<select name="name" size="number" multiple>
  ......
</select>
```

### Elemen OPTION

Elemen `option` mendefinisikan opsi pilihan pada menu `select`. Elemen ini mempunyai atribut `selected` dan `value`. Atribut `Selected` berisi opsi terpilih dan atribut `value` berisi nilai elemen option.

Sintaks :

```html
<option selected value="number">.....................</option>
```

### Elemen TEXTAREA

Elemen `textarea` berfungsi sebagai input kontrol form untuk memasukkan teks lebih dari satu baris. Elemen ini mempunyai attribute yaitu `name`, `cols`, `rows`.

- `name` mendefinisikan nama input kontrol form elemen textarea
- `cols` mendefinisikan jumlah kolom textarea yang terlihat
- `rows` mendefinisikan jumlah baris textarea yang terlihat.

Element ini harus berada di dalam element FORM

Sintaks:

```html
<textarea name="name" cols="number" rows="number">
.....................
</textarea>
```

### Langkah Praktikum

1.  [Form Dasar (Text, Checkbox, Radio, Submit dan Reset)](#bagian-satu-form-dasar-text-checkbox-radio-submit-dan-reset)
2.  [Modifikasi Text dan Checkbox](#bagian-dua-modifikasi-text-dan-checkbox)
3.  [Select dan Option](#bagian-tiga-select-dan-option)
4.  [Modifikasi Select dan Option](#bagian-empat-modifikasi-select-dan-option)
5.  [Password](#bagian-lima-password)
6.  [Textarea](#bagian-enam-textarea)
7.  [GET dan POST](#bagian-tujuh-get-dan-post)

#### Bagian Satu: Form Dasar (Text, Checkbox, Radio, Submit dan Reset)

1.  Buat sebuah file bernama `buatForm.html` dan simpan file tersebut di dalam folder dasarWeb
2.  Ketikkan kode di bawah ini dalam buatForm.html

    ```html
    <html>
      <head>
        <title>Membuat Form</title>
      </head>

      <body>
        <form method="POST" action="gambar.html">
          <h4>FORM</h4>
          <input
            type="text"
            name="var1"
            size="30"
            value="Enter your name here."
          />
          <br /><br />
          <b>Are you a student?</b>
          <input type="checkbox" name="var2" />
          <br /><br />
          <b>How old are you?</b>
          <br />
          <input type="radio" name="var3" value="r1" />10 - 15 <br />
          <input type="radio" name="var3" value="r2" />16 - 20 <br />
          <input type="radio" name="var3" value="r3" />21 - 25 <br /><br />
          <input type="submit" name="var4" value="Send" />
          <input type="reset" name="var5" value="Clear" />
        </form>
      </body>
    </html>
    ```

3.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatForm.html](http://localhost/dasarWeb/buatForm.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatForm.html](/html/img/praktikum12/form1.png)

4.  Amati apa yang tampil pada browser. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Didalam tampilan website tersebut, berisi tentang form tentang nama, menanyakan murid atau tidak, dan umur dari responden.
    - Untuk membuat form, diawali dengan tag `<form>` diikuti dengan implementasi tag `<input>` yang berfungsi untuk menyediakan area yang diisi sesuai dengan fungsinya.
    - Jika sudah mengisi, maka bisa menekan tombol `send` dan akan mengarahkan ke `gambar.html` dan jika ingin membatalkan isi form tersebut, maka menekan tombol `clear` sehingga form kosong.

#### Bagian Dua: Modifikasi Text dan Checkbox

5.  Tambahkan satu input text yang akan digunakan untuk memasukkan alamat, letakkan di bawah elemen input text untuk memasukkan nama.

    ```html
    <form method="POST" action="gambar.html">
      <h4>FORM</h4>
      <input type="text" name="var1" size="30" value="Enter your name here." />
      <br /><br />
      <input
        type="text"
        name="var6"
        size="30"
        value="Enter your address here."
      />
      <br /><br />
      ...
    </form>
    ```

6.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatForm.html](http://localhost/dasarWeb/buatForm.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatForm.html](/html/img/praktikum12/form2.png)

7.  Amati apa yang tampil pada browser. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Yang berubah adalah penambahan kotak pengisian berupa alamat yang diisi.

8.  Tambahkan kode program berikut ini di bawah radio button yang terakhir, di atas tombol submit dan clear.

    ```html
    <form method="POST" action="gambar.html">
      ...
      <input type="radio" name="var3" value="r3" />21 - 25 <br /><br />
      <br />

      <!-- Vehicle Checkbox-->
      <b>Which one do you have?</b>
      <br /><br />
      <input type="checkbox" name="vehicle1" value="Bike" checked /> I have a
      bike
      <br />
      <input type="checkbox" name="vehicle2" value="Car" /> I have a car <br />
      <input type="checkbox" name="vehicle3" value="Boat" /> I have a boat
      <br />
      ...
    </form>
    ```

9.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatForm.html](http://localhost/dasarWeb/buatForm.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatForm.html](/html/img/praktikum12/form3.png)

10. Tambahkan satu input checkbox yang akan menampilkan pilihan berisi “**I have a plane**” dan tanda centang (v) pindah dari opsi “**I have a bike**” ke opsi checkbox “**I have a plane**”.

    ```html
    <form method="POST" action="gambar.html">
      ...
      <b>Which one do you have?</b>
      <br /><br />
      <input type="checkbox" name="vehicle1" value="Bike" /> I have a bike
      <br />
      <input type="checkbox" name="vehicle2" value="Car" /> I have a car <br />
      <input type="checkbox" name="vehicle3" value="Boat" /> I have a boat
      <br />
      <input type="checkbox" name="vehicle4" value="Plane" checked /> I have a
      plane
      <br />
      ...
    </form>
    ```

11. Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatForm.html](http://localhost/dasarWeb/buatForm.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatForm.html](/html/img/praktikum12/form4.png)

12. Tuliskan di sini kode seluruh pengaturan checkbox termasuk kode pengaturan checkbox yang baru saja anda tambahkan.

    ```html
    <html>
      <head>
        <title>Membuat Form</title>
      </head>

      <body>
        <form method="POST" action="gambar.html">
          <h4>FORM</h4>
          <input
            type="text"
            name="var1"
            size="30"
            value="Enter your name here."
          />
          <br /><br />
          <input
            type="text"
            name="var6"
            size="30"
            value="Enter your address here."
          />
          <br /><br />
          <b>Are you a student?</b>
          <input type="checkbox" name="var2" />
          <br /><br />
          <b>How old are you?</b>
          <br />
          <input type="radio" name="var3" value="r1" />10 - 15 <br />
          <input type="radio" name="var3" value="r2" />16 - 20 <br />
          <input type="radio" name="var3" value="r3" />21 - 25 <br /><br />
          <br />

          <b>Which one do you have?</b>
          <br /><br />
          <input type="checkbox" name="vehicle1" value="Bike" /> I have a bike
          <br />
          <input type="checkbox" name="vehicle2" value="Car" /> I have a car
          <br />
          <input type="checkbox" name="vehicle3" value="Boat" /> I have a boat
          <br />
          <input type="checkbox" name="vehicle4" value="Plane" checked /> I have
          a plane
          <br />
          <input type="submit" name="var4" value="Send" />
          <input type="reset" name="var5" value="Clear" />
        </form>
      </body>
    </html>
    ```

#### Bagian Tiga: Select dan Option

13. Tambahkan kode program ini dan tempatkan di bawah pengaturan checkbox dan di atas pengaturan tombol

    ```html
    <form method="POST" action="gambar.html">
      ...
      <input type="checkbox" name="vehicle4" value="Plane" checked /> I have a
      plane
      <br />
      <br />
      <b>Where are you from?</b>
      <br />
      <select name="var7" size="1">
        <option value="BG">Bulgaria</option>
        <option value="UK">United Kingdom</option>
        <option value="USA" selected>USA</option>
      </select>
      <br /><br />
      ...
    </form>
    ```

14. Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatForm.html](http://localhost/dasarWeb/buatForm.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatForm.html](/html/img/praktikum12/form5.png)

15. Amati apa yang tampil pada browser. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Program tersebut akan menampilkan pilihan tempat dimana anda berasal.
    - Dengan adanya tag `<select>` yang akan menyediakan kotak pilihan dan tag `<option>` yang akan menyediakan pilihan nya sesuai dengan programnya yaitu tiga negara seperti Bulgaria, United Kingdom, dan USA.

16. Tambahkan satu pilihan negara yaitu Indonesia dan default pilihan berada di negara Indonesia.

    ```html
    <form method="POST" action="gambar.html">
      ...
      <select name="var7" size="1">
        <option value="BG">Bulgaria</option>
        <option value="UK">United Kingdom</option>
        <option value="USA">USA</option>
        <option value="INA" selected>Indonesia</option>
      </select>
      ...
    </form>
    ```

17. Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatForm.html](http://localhost/dasarWeb/buatForm.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatForm.html](/html/img/praktikum12/form6.png)

18. Amati apa yang tampil pada browser. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Perubahannya adalah nilai defaultnya dari USA ke Indonesia karena atribut `selected` didalam elemen option dari Indonesia

#### Bagian Empat: Modifikasi Select dan Option

19. Ubah nilai `size=1` menjadi `size=2`.
    ```html
    <form method="POST" action="gambar.html">
      ...
      <select name="var7" size="2">
        <option value="BG">Bulgaria</option>
        <option value="UK">United Kingdom</option>
        <option value="USA">USA</option>
        <option value="INA" selected>Indonesia</option>
      </select>
      ...
    </form>
    ```
20. Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatForm.html](http://localhost/dasarWeb/buatForm.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatForm.html](/html/img/praktikum12/form7.png)

21. Amati apa yang tampil pada browser. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Perubahannya adalah kotak pilihan nya menjadi lebar dan tampilannya menjadi dua pilihan.
    - Akan tetapi, nilai defaultnya tetap Indonesia dan dipilih hanya satu pilihan
    - Karena tampilan demikian, alhasil pengguna akan merasa kebingungan dari pilihannya.

22. Kembalikan nilai `size=1` dari program sebelumnya
    ```html
    <form method="POST" action="gambar.html">
      ...
      <select name="var7" size="1">
        <option value="BG">Bulgaria</option>
        <option value="UK">United Kingdom</option>
        <option value="USA">USA</option>
        <option value="INA" selected>Indonesia</option>
      </select>
      ...
    </form>
    ```

#### Bagian Lima: Password

23. Tambahkan sebuah _single text area_ untuk memasukkan password, menggunakan `input` dengan tipe `password`.

    ```html
    <form method="POST" action="gambar.html">
      ...
      <br /><br />
      <b>Enter your private code</b>
      <input type="password" name="pass" />
      <br /><br />
      ...
    </form>
    ```

24. Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatForm.html](http://localhost/dasarWeb/buatForm.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatForm.html](/html/img/praktikum12/form8.png)

#### Bagian Enam: Textarea

25. Tambahkan sebuah text area untuk mengetik komentar panjang dengan menggunakan tag `<textarea>` dan `</textarea>`

    ```html
    <form method="POST" action="gambar.html">
      ...
      <br /><br />
      <b>Enter your comment</b>
      <textarea name="var8" cols="30" rows="5" placeholder="Fill this area">
      <br /><br />
      ...
    </form>
    ```

26. Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatForm.html](http://localhost/dasarWeb/buatForm.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatForm.html](/html/img/praktikum12/form9.png)

#### Bagian Tujuh: GET dan POST

27. Perhatikan pada tag `<form>` terdapat atribut `method=”POST”`.

    ```html
    <form method="POST" action="gambar.html">...</form>
    ```

28. Jalankan kembali pada browser alamat berikut: [localhost/dasarWeb/buatForm.html](http://localhost/dasarWeb/buatForm.html), isi form, lalu klik pada tombol Send. <br>
    **Perhatikan pada alamat URL di halaman yang di tuju setelah tombol Send diklik.**

    ![buatForm.html](/html/img/praktikum12/form10.png)

29. Buka kembali kode program `buatForm.html`, ubah method dari `POST` menjadi `GET`.

    ```html
    <form method="GET" action="gambar.html">...</form>
    ```

30. Simpan dan jalankan kembali pada browser alamat berikut: [localhost/dasarWeb/buatForm.html](http://localhost/dasarWeb/buatForm.html), isi form seperti sebelumnya, lalu klik pada tombol Send.
    **Perhatikan pada alamat URL di halaman yang di tuju setelah tombol send diklik.**

31. Amati dan bandingkan perbedaan antara method **GET** dan **POST**. Catat hasil pengamatanmu di sini.

    ![buatForm.html](/html/img/praktikum12/form11.png)
    **METHOD POST**

    ![buatForm.html](/html/img/praktikum12/form12.png)
    **METHOD GET**

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Dari perbedaan tersebut dapat disimpulkan bahwa **POST** tidak akan menampilkan data yang kita masukkan ke dalam URL. Sedangkan **GET** sebaliknya akan menampilkan nya ke dalam URL.
    - Jika demikian, maka method **POST** lebih aman daripada **GET** jika ingin memasukkan form ke internet. Selain itu, data akan disembunyikan dari URL.
