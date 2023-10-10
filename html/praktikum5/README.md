# Praktikum 5 - Karakter Khusus

Dalam HTML, kita juga bisa menampilkan karakter-karakter khusus dengan memanfaatkan nama entitas. Tabel berikut memperlihatkan beberapa jenis karakter khusus yang dapat digunakan beserta nama entitasnya.

![Tabel Karakter Khusus](/html/img/praktikum5/tabelKarakter.png)

### Langkah Praktikum

1.  Buat sebuah file bernama `karakter.html` dan simpan file tersebut di dalam folder dasarWeb.
2.  Ketikkan kode dibawah ini dalam `karakter.html`

    ```html
    <html>
      <head>
        <title>Karakter Khusus</title>
      </head>

      <body>
        &pound; Pound <br />
        &euro; Euro <br />
        &copy; Copyright <br />
        &reg; Registered <br />
        &trade; Trademark <br />
      </body>
    </html>
    ```

3.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/karakter.html](http://localhost/dasarWeb/karakter.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![karakter.html](/html/img/praktikum5/karakter.png)

4.  Amati apa yang muncul pada browser. Catat hasil pengamatanmu

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Untuk membuat karakter khusus seperti pada halaman website diatas, menggunakan entitas khusus yang mewakili karakter khusus tersebut. Jika entitas khusus ada, maka karakter khusus bisa dibuat.
    - Seperti contoh untuk membuat karakter copyright &copy;, maka harus mengetik entitas khususnya untuk memanggilnya yaitu `&copy;`.
