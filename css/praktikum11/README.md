# Praktikum 11 - Menggunakan Float

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Teknik Floating pada bagian web design merupakan sebuah kebutuhan yang paling banyak di perlukan. Properti `float` digunakan untuk memposisikan dan memformat konten.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Misalnya membuat gambar melayang ke sebelah kiri teks dalam kontainer. Salah satu contoh penggunaan float yang paling sering di temukan adalah ketika kita ingin membuat gambar postingan website yang terletak di bagian samping tulisan konten. Properti float dapat memiliki salah satu dari nilai berikut:

- kiri - Elemen mengapung di sebelah kiri wadahnya
- kanan- Elemen mengapung di sebelah kanan wadahnya
- tidak ada - Elemen tidak mengambang (akan ditampilkan tepat di tempat teks tersebut muncul). Ini standar
- _inherit_ - Elemen ini mewarisi nilai float dari induknya

Dalam penggunaannya yang paling sederhana, properti `float` dapat digunakan untuk membungkus teks di sekitar gambar.

### Langkah Praktikum

1.  Buat satu file baru bernama `floatCSS.html` di dalam folder dasarWeb
2.  Ketikkan ke dalam file `floatCSS.html` tersebut kode di bawah ini.

    ```html
    <html>
      <head>
        <title>Menggunakan Float</title>
        <link rel="stylesheet" type="text/css" href="styleFloat.css" />
      </head>

      <body>
        <h2>Float Kiri</h2>
        <br />
        <div class="float1">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium
            doloribus sequi commodi optio voluptatibus cum ratione eveniet
            tempora, neque quia alias aliquam impedit odio est! Deserunt
            excepturi aspernatur ullam quidem!
            <img class="gambar" src="img/polinema.png" />
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum
            minus iusto ratione officia labore. Fugiat sapiente consequatur
            voluptas possimus, mollitia eaque non magnam temporibus nulla
            placeat deleniti distinctio officiis corrupti. Lorem ipsum dolor sit
            amet consectetur adipisicing elit. Voluptatum earum blanditiis
            suscipit minima repellendus reprehenderit magni totam voluptatibus
            illo odit rem enim deleniti quidem dicta eligendi excepturi,
            provident cupiditate aperiam? Lorem ipsum dolor sit amet consectetur
            adipisicing elit. Eligendi deserunt officia distinctio veniam unde
            iure ab, pariatur delectus cumque accusantium illo suscipit tenetur
            odit consequuntur molestiae autem obcaecati sequi dolores!
          </p>
        </div>
      </body>
    </html>
    ```

3.  Buat satu file baru bernama `styleFloat.css` di dalam folder dasarWeb
4.  Ketikkan ke dalam file `styleFloat.css` tersebut kode di bawah ini.

    ```css
    h2 {
      text-align: center;
      color: blueviolet;
    }

    .gambar {
      width: 100px;
      float: left;
      margin-right: 10px;
    }
    ```

5.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/floatCSS.html](http://localhost/dasarWeb/floatCSS.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![floatCSS.html](/css/img/praktikum11/floatCSS.png)

6.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Dengan adanya float, gambar bisa diatur posisinya dengan menggunakan properti float
