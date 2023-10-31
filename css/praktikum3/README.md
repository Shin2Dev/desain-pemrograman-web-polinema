# Praktikum 3 - Mengenal class dan id pada HTML

### Mengenal _class_ dan _id_ pada HTML

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`Class` dan `id` digunakan sebagai penanda pada `html`, yang dimaksud dengan penanda di sini adalah element-element `html` dapat di beri tanda dengan `class` atau `id`. Elemen-elemen dalam `HTML` diberi tanda agar dapat di manipulasi menggunakan `css` atau `javascript`.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Bayangan sederhananya jika anda memiliki lima buah kotak, semua kotak yang anda miliki berwarna biru, kemudian anda ingin mengubah warna kotak yang ketiga, nah di sinilah letak kegunaan `class` dan `id`, untuk memberikan tanda atau nama pada kotak anda agar bisa di ubah dan kotak yang lain tidak akan berubah.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Perbedaan dari `class` dan `id` adalah `class` di panggil pada css atau javascript dengan menggunakan tanda titik “.”, dan `id` di panggil pada css atau javascript dengan tanda pagar “#”, ada kelebihan di sini untuk `class`, yaitu `class` dapat di berikan pada banyak element `html` dan dapat di panggil sekaligus, sedangkan `id` hanya dapat bekerja pada satu penandaan saja, maksudnya satu nama `id` hanya bisa di berikan pada satu element saja.

#### Langkah Praktikum

1.  Buat satu file baru bernama `classid.html` di dalam folder dasarWeb
2.  Ketikkan ke dalam file `classid.html` tersebut kode di bawah ini.

    ```html
    <html>
      <head>
        <title>Main Page</title>
        <link rel="stylesheet" href="style1.css" />
      </head>

      <body>
        <h2>Welcome To DasarWeb</h2>
        <br /><br />
        <!-- Contoh penggunaan class -->
        <div class="kotak">kotak 1</div>
        <div class="kotak">kotak 2</div>
        <div class="kotak">kotak 3</div>
        <!-- Contoh penggunaan id -->
        <div id="kotak">kotak 4</div>
      </body>
    </html>
    ```

3.  Buat lagi satu file baru di dalam direktori dasarWeb, beri nama `style1.css`. Ketikkan kode di bawah ini di dalam file `style1.css`.

    ```css
    h2 {
      color: orange;
      font-family: "Trebuchet MS";
      text-align: center;
    }

    .kotak {
      padding: 50px;
      width: 100px;
      color: #fff;
      margin: 10px;
      background: orange;
    }

    #kotak {
      width: 400px;
      color: #fff;
      background: blue;
      padding: 50px;
    }
    ```

4.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/classid.html](http://localhost/dasarWeb/classid.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![classid.html](/css/img/praktikum3/classid.png)

5.  Apa yang anda pahami dari penggunaan class dan id pada file tersebut. Catat di bawah ini pemahaman anda

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Fungsi dari `id` adalah identitas dari satu elemen, sedangkan `class` adalah identitas kelas yang bisa lebih dari satu elemen.
    - Untuk menerapkan css berdasarkan `id` dimulai dari `#<nama-id>` dan `class` dimulai dari `.<nama-class>`
    - Dengan adanya `id` dan `class`, penerapan css bisa dari sebagian elemen global.
    - Misal nya dalam halaman html terdapat 4 div. 1 dari 4 div diberi `class / id`. Maka jika penerapan css berdasarkan `class / id`, maka yang berdampak adalah div yang punya `class / id` itu sendiri dan bukan dari div yang tanpa `class / id`.
