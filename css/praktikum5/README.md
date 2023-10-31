# Praktikum 5 - Menggunakan _image_ untuk _Background_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Properti _background-image_ menetapkan satu atau lebih gambar _background_ untuk suatu elemen. Secara default, gambar latar belakang ditempatkan di sudut kiri atas elemen, dan diulang secara vertikal dan horizontal.

**Tip**:

- Latar belakang suatu elemen adalah ukuran total elemen, termasuk _padding_ dan _border_ (tetapi bukan margin).
- Selalu atur warna latar untuk digunakan jika gambar tidak tersedia

### Langkah Praktikum

1.  Pada file `style1.css` pada [praktikum 3](/css/praktikum3/) ubah value dari background menjadi [bunga2.jpeg](/css/praktikum5/dasarWeb/img/bunga2.jpeg) seperti pada potongan kode dibawah ini

    ```css
    body {
      background: url("bunga2.jpeg");
      color: white;
    }
    ```

2.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/classid.html](http://localhost/dasarWeb/classid.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![classid.html](/css/img/praktikum5/classid3.png)

3.  Catat di sini apa yang anda amati dari penambahan kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Untuk menerapkan gambar sebagai latar belakang, maka nilai dari properti `background` yang tadinya warna menjadi link url gambar.
    - Untuk gambarnya bisa dari direktori lokal / _relative path_, atau link gambar di internet / _absolute path_.
    - Tentunya penamaan dan direktori harus benar supaya background gambar muncul sesuai dengan keinginan

4.  Tambahkan file gambar bernama [field1.jpeg](/css/praktikum5/dasarWeb/img/field.jpeg) dan [tree1.png](/css/praktikum5/dasarWeb/img/tree.png) pada folder img.

5.  Ubah kode program pada `style1.css` menjadi seperti dibawah ini

    ```css
    body {
      background: url("img/tree.png"), url("img/field.jpeg");
      background-repeat: no-repeat, repeat;
      color: white;
    }
    ```

6.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/classid.html](http://localhost/dasarWeb/classid.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![classid.html](/css/img/praktikum5/classid4.png)

7.  Catat apa yang kalian pahami dari perubahan tampilan yang terjadi.

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Dalam menerapkan gambar pada background bisa lebih dari satu gambar. Seperti pada contoh penerapan dua gambar pada background html diatas yaitu pohon dan lapangan
    - Dalam tampilan website, lapangan akan duplikat terus menerus hingga menutupi latar belakang, sedangkan pohon hanya satu kali saja.
    - Hal ini dikarenakan pengulangan dari background lapangan disetel berulang ulang (_repeat_) sedangkan background pohon disetel tidak berulang atau hanya satu kali (_no-repeat_)
