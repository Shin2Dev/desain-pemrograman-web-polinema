# Praktikum 4 - Mengubah _Background_ Halaman Web dengan CSS

### Cara Penulisan CSS

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`CSS` menggunakan selector (`id` dan `class`) untuk menentukan element yang akan di modifikasi atau yang akan di beri sentuhan `css`, jika di ibaratkan HTML sebagai tiang pada sebuah bangunan rumah, maka CSS berfungsi sebagai cat dan dekorasi pada bangunan rumah tersebut. Ada tiga teknik metode penulisan CSS, yaitu:

- _Inline CSS Style_

  Adalah CSS yang dibuat dalam sebuah tag HTML yang hanya berlaku untuk dokumen yang diapitnya saja. Biasanya teknik ini digunakan pada pemformatan khusus pada sebuah elemen HTML dan tidak digunakan untuk memformat seluruh elemen dalam dokumen web. <br>
  Contoh:

  ```html
  <h1 style="color: blue; margin-left: 30px;">This is a heading.</h1>
  ```

- _Internal CSS Style_

  Sebuah internal style sheet untuk sebuah halaman web hanya berlaku pada sebuah halaman web tersebut saja. Internal style sheet didefinisikan pada bagian `HEAD` sebuah halaman `HTML`, di dalam tag `<style>` seperti berikut:

  ```html
  <head>
    <style>
      body {
        background-color: lime;
      }

      h1 {
        color: maroon;
        margin-left: 40px;
      }
    </style>
  </head>
  ```

- _External CSS Style_

  Sangat ideal digunakan pada web dengan banyak halaman. Dengan menggunakan _External Style Sheet_ tampilan seluruh isi website dapat diubah hanya dengan mengubah satu file. _External Style Sheet_ tidak boleh mengandung tag html, dan disimpan dalam file dengan ekstensi \*.css <br>
  Contoh:

  ```css
  body {
    background-color: lightblue;
  }

  h1 {
    color: navy;
    margin-left: 20px;
  }
  ```

  Cara pemanggilan _External Style Sheet_ dalam sebuah halaman web yaitu dengan menggunakan tag `<link>` dengan atribut rel yang diletakkan pada `section head`. Contoh:

  ```html
  <head>
    <link rel="stylesheet" href="style.css" />
  </head>
  ```

#### Langkah Praktikum

1.  Tambahkan potongan kode program di bawah ini pada file `style1.css` pada [praktikum sebelumnya](/css/praktikum3/)

    ```css
    body {
      background: lightcyan;
      color: white;
    }
    ```

2.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/classid.html](http://localhost/dasarWeb/classid.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![classid.html](/css/img/praktikum4/classid2.png)

3.  Catat di sini apa yang anda amati dari penambahan kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Untuk mengubah warna latar belakang / background pada html, maka penerapan css nya adalah properti `background` didalam tag `<body>`.
    - Untuk nilai warnanya bisa menggunakan nama warna dalam Bahasa inggris, kode hex, atau rgb / hsb.
