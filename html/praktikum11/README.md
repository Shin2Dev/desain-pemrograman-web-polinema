# Praktikum 11 - Tabel dan Pengaturannya

Dalam sebuah halaman web, tabel dijadikan kerangka untuk meletakkan komponen-komponen isi web, sehingga isi dalam sebuah web dapat diatur dengan rapi. <br>
Contoh gambaran struktur desain tabel :

![Contoh Tabel Web](/html/img/praktikum11/tabel-web.png)

### Pembuatan Tabel

Pembuatan tabel dalam HTML dimulai dengan tag `<table>` dan diakhiri dengan tag `</table>`.

- `<table>` : tag yang menerangkan kepada browser bahwa itu adalah sebuah tabel
- `<tr>` : tag Tabel Row yang digunakan untuk membuat baris dalam tabel
- `<td>` : tag Tabel Data yang digunakan untuk meletakkan data yang ingin kita isikan dalam tabel, TD dapat juga kita artikan sebagai kolom.

  ![Struktur Tabel](/html/img/praktikum11/struktur-tabel.png)

  Sintaks pembuatan tabel adalah sebagai berikut :

  ```html
  <table atribut="”value”">
    <tr>
      <td atribut="”value">……ISI….</td>
      <td atribut="”value">……ISI1….</td>
    </tr>
    <tr>
      …… ……
    </tr>
  </table>
  ```

### Pengaturan Tabel

Berikut ini adalah atribut-atribut yang dapat dipergunakan untuk pengaturan tabel dan baris.

- Atribut pada Tabel
  | Atribut | Keterangan |
  |---------|------------|
  | align | Digunakan untuk meratakan tabel ke kiri, ke tengah, ke kanan, atau kanan kiri |
  | border | Digunakan untuk mengatur ketebalan garis pembatas antar sel dalam tabel |
  | width | Digunakan untuk menentukan lebar tabel, anda dapat menentukan lebar tabel dengan nilai persen(%) |
  | cellspacing | Digunakan untuk menyatakan jarak (spasi) antar sel serta antara sel dengan batas |
  | cellpadding | Menyatakan jarak (spasi) antara isi sel dengan batas sel (border) |
  | bgcolor | Menyatakan warna background untuk semua cell pada tabel |
  | bordercolor | Digunakan untuk membuat warna pada garis/border |

- Atribut pada Baris
  | Atribut | Keterangan |
  |---------|------------|
  | align | Digunakan untuk meratakan tabel ke kiri, ke tengah, ke kanan, atau kanan kiri |
  | valign | Digunakan untuk melakukan perataan yang bersifat horizontal(alignment), valign menggunakan nilai top(atas halaman), center(tengah halaman), bottom(bawah) atau baseline(standar) |
  | bgcolor | Menunjukkan warna background pada baris (row) |

### Merger Cell

Untuk melakukan penggabungan cell digunakan :

- `Rowspan` : digunakan untuk menggabungkan antar baris, jika hendak menggabungkan 3 baris maka value kita beri angka 3
- `Colspan` : digunakan untuk menggabungkan antar kolom, jika hendak menggabungkan 3 kolom maka value kita beri angka 3

### Langkah Praktikum

1. [Tabel Dasar](#bagian-satu-tabel-dasar)
2. [Border](#bagian-dua-border)
3. [Width dan Height](#bagian-tiga-width-dan-height)
4. [% vs px](#bagian-empat--vs-px)
5. [Cellpadding](#bagian-lima-cellpadding)
6. [Cellspacing](#bagian-enam-cellspacing)
7. [Align](#bagian-tujuh-align)
8. [Valign](#bagian-delapan-valign)
9. [Font Face](#bagian-sembilan-font-face)
10. [Font Color dan Font Size](#bagian-sepuluh-font-color-dan-font-size)
11. [Colspan dan Rowspan](#bagian-sebelas-colspan-dan-rowspan)
12. [Modifikasi Rowspan](#bagian-duabelas-modifikasi-rowspan)

#### Bagian Satu: Tabel Dasar

1.  Buat sebuah file bernama `buatTabel.html` dan simpan file tersebut di dalam folder dasarWeb.
2.  Ketikkan kode di bawah ini dalam `buatTabel.html`

    ```html
    <html>
      <head>
        <title>Membuat tabel</title>
      </head>

      <body>
        <table>
          <tr>
            <td>Ini baris pertama kolom pertama</td>
            <td>Ini baris pertama kolom kedua</td>
          </tr>
        </table>
      </body>
    </html>
    ```

3.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatTabel.html](http://localhost/dasarWeb/buatTabel.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatTabel.html](/html/img/praktikum11/tabel1.png)

4.  Amati apa yang tampil pada browser. Catat hasil pengamatanmu
    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:
    - Dari halaman website diatas, memang tidak tampak seperti tabel. Akan tetapi, dalam struktur halaman html sudah menerapkan elemen `<table>`.
    - Selain itu sudah menerapkan `<tr>` yang mendefinisikan baris dan `<td>` yang mendefinisikan kolom dan sudah disertai dengan isi.

#### Bagian Dua: Border

5.  Tambahkan atribut `border = 1` pada tag `<table>`. Simpan file lalu jalankan melalui browser : [localhost/dasarWeb/buatTabel.html](localhost/dasarWeb/buatTabel.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ```html
    <body>
      <table border="1">
        <tr>
          <td>Ini baris pertama kolom pertama</td>
          <td>Ini baris pertama kolom kedua</td>
        </tr>
      </table>
    </body>
    ```

    ![buatTabel.html](/html/img/praktikum11/tabel2.png)

6.  Amati apa yang berubah pada tampilan. Catat hasil pengamatanmu.

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Jika ditambahkan atribut `border`, maka akan membentuk garis tepi didalam tabel sehingga yang tadinya tidak tampak sekarang lebih tampak seperti tabel.

#### Bagian Tiga: Width dan Height

7.  Tambahkan satu baris dalam tabel yang dibuat sebelumnya dan tambahkan satu kolom di dalamnya.

    ```html
    <body>
      <table border="1">
        <tr>
          <td>Ini baris pertama kolom pertama</td>
          <td>Ini baris pertama kolom kedua</td>
        </tr>
        <tr>
          <td>Ini baris kedua kolom pertama</td>
        </tr>
      </table>
    </body>
    ```

8.  Tambahkan atribut pada tag `<table>` berupa `height=100% width=40%`.

    ```html
    <body>
      <table border="1" height="100%" width="40%">
        <tr>
          <td>Ini baris pertama kolom pertama</td>
          <td>Ini baris pertama kolom kedua</td>
        </tr>
        <tr>
          <td>Ini baris kedua kolom pertama</td>
        </tr>
      </table>
    </body>
    ```

9.  Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatTabel.html](http://localhost/dasarWeb/buatTabel.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatTabel.html](/html/img/praktikum11/tabel3.png)

10. Catat di sini perubahannya.

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Perubahan yang terjadi adalah melebar dan memanjang nya tabel yang tadinya sempit sekarang menjadi lebih luas.
    - Width adalah panjang dan Height adalah lebar.
    - Dikarenakan nilai nya berupa persen, maka lebar dan panjang dari tabel akan menjadi dinamis dan mengikuti panjang dan lebar halaman website itu sendiri.

#### Bagian Empat: % vs px

11. Hapus tanda % pada `height` dan `width`, sehingga menjadi `height=100 width=40`.

    ```html
    <body>
      <table border="1" height="100" width="40">
        <tr>
          <td>Ini baris pertama kolom pertama</td>
          <td>Ini baris pertama kolom kedua</td>
        </tr>
        <tr>
          <td>Ini baris kedua kolom pertama</td>
        </tr>
      </table>
    </body>
    ```

12. Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatTabel.html](http://localhost/dasarWeb/buatTabel.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatTabel.html](/html/img/praktikum11/tabel4.png)

13. Apa yang anda pahami dari perbedaan penggunaan % dan penghilangan % pada kode program tersebut. Catat di sini.

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Perbedaannya adalah jika menggunakan %, ukuran tabel akan menjadi dinamis mengikuti halaman website
    - Sedangkan jika tanpa menggunakan %, ukuran tabel akan menjadi statis dan tetap sehingga walaupun halaman diperbesar / fullscreen, ukuran tabel tidak berubah.

#### Bagian Lima: Cellpadding

14. Tambahkan atribut `cellpadding = 20`.

    ```html
    <body>
      <table border="1" height="100" width="40" cellpadding="20">
        <tr>
          <td>Ini baris pertama kolom pertama</td>
          <td>Ini baris pertama kolom kedua</td>
        </tr>
        <tr>
          <td>Ini baris kedua kolom pertama</td>
        </tr>
      </table>
    </body>
    ```

15. Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatTabel.html](http://localhost/dasarWeb/buatTabel.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatTabel.html](/html/img/praktikum11/tabel5.png)

16. Catat di sini perubahannya.

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Perubahannya adalah jarak antara elemen / tulisan dengan garis tepi menjadi lebih lebar dan longgar sehingga enak dipandang mata.
    - Untuk menggunakan jarak tersebut menggunakan atribut `cellpadding` khusus untuk tabel.

#### Bagian Enam: Cellspacing

17. Tambahkan atribut `cellspacing = 5`.

    ```html
    <body>
      <table
        border="1"
        height="100"
        width="40"
        cellpadding="20"
        cellspacing="5"
      >
        <tr>
          <td>Ini baris pertama kolom pertama</td>
          <td>Ini baris pertama kolom kedua</td>
        </tr>
        <tr>
          <td>Ini baris kedua kolom pertama</td>
        </tr>
      </table>
    </body>
    ```

18. Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatTabel.html](http://localhost/dasarWeb/buatTabel.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatTabel.html](/html/img/praktikum11/tabel6.png)

19. Catat di sini perubahannya.

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Perubahannya adalah jarak antara garis tepi dalam tabel dan garis tepi luar tabel terlihat lebih lebar / longgar dengan menggunakan atribut `cellspacing`.

#### Bagian Tujuh: Align

20. Pada kode program yang digunakan untuk mengatur kolom 1 dari baris 1, tambahkan atribut `align="right"`, sehingga kode pada bagian tersebut menjadi `<td align="right">`.

    ```html
    <body>
      <table
        border="1"
        height="100"
        width="40"
        cellpadding="20"
        cellspacing="5"
      >
        <tr>
          <td align="right">Ini baris pertama kolom pertama</td>
          <td>Ini baris pertama kolom kedua</td>
        </tr>
        <tr>
          <td>Ini baris kedua kolom pertama</td>
        </tr>
      </table>
    </body>
    ```

21. Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatTabel.html](http://localhost/dasarWeb/buatTabel.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatTabel.html](/html/img/praktikum11/tabel7.png)

22. Catat di sini hasil pengamatanmu.

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Didalam tabel bisa diatur perataan tulisan nya dengan atribut `align` didalam tag `<td>`.
    - Dari dalam tulisan “**Ini baris pertama kolom pertama**”, perataannya menjadi kanan.

#### Bagian Delapan: Valign

23. Tambahkan % pada `height` dan `width`, sehingga menjadi `height=100% width=40%`.
24. Selanjutnya pada kode program yang digunakan untuk mengatur kolom 1 dari baris 1, tambahkan atribut `valign="bottom"`, sehingga kode pada bagian tersebut menjadi `<td align="right" valign="bottom">`.

    ```html
    <body>
      <table
        border="1"
        height="100%"
        width="40%"
        cellpadding="20"
        cellspacing="5"
      >
        <tr>
          <td align="right" valign="bottom">Ini baris pertama kolom pertama</td>
          <td>Ini baris pertama kolom kedua</td>
        </tr>
        <tr>
          <td>Ini baris kedua kolom pertama</td>
        </tr>
      </table>
    </body>
    ```

25. Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatTabel.html](http://localhost/dasarWeb/buatTabel.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatTabel.html](/html/img/praktikum11/tabel8.png)

26. Catat di sini hasil pengamatanmu.

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Tampilan dari tabel tersebut pada baris pertama kolom pertama, tulisan nya berada di bawah tabel karena atribut dari `valign` dan nilai nya bottom / bawah.

#### Bagian Sembilan: Font Face

27. Tambahkan pengaturan font pada isi baris pertama kolom pertama dengan menambahkan tag `<font>` di dalam tag `<td>`.

    ```html
    <body>
      <table
        border="1"
        height="100%"
        width="40%"
        cellpadding="20"
        cellspacing="5"
      >
        <tr>
          <td align="right" valign="bottom">
            <font face="courier">Ini baris pertama kolom pertama</font>
          </td>
          <td>Ini baris pertama kolom kedua</td>
        </tr>
        <tr>
          <td>Ini baris kedua kolom pertama</td>
        </tr>
      </table>
    </body>
    ```

28. Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatTabel.html](http://localhost/dasarWeb/buatTabel.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatTabel.html](/html/img/praktikum11/tabel9.png)

29. Catat di sini hasil pengamatanmu.

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Gaya penulisan dari baris pertama dan kolom pertama dari tabel berubah menjadi gaya _Courier_. Hal ini bisa diimplementasikan dengan tag `<font>` disertai dengan atribut `face` yang berfungsi untuk mengubah gaya tulisan.

#### Bagian Sepuluh: Font Color dan Font Size

30. Ubah warna tulisan “**ini baris pertama kolom pertama**” menjadi warna merah, ukuran=15
31. Tulis kode yang berubah sesuai dengan langkah 30 pada file `buatTabel.html`.

    ```html
    <body>
      <table
        border="1"
        height="100%"
        width="40%"
        cellpadding="20"
        cellspacing="5"
      >
        <tr>
          <td align="right" valign="bottom">
            <font face="courier" color="red" size="15"
              >Ini baris pertama kolom pertama</font
            >
          </td>
          <td>Ini baris pertama kolom kedua</td>
        </tr>
        <tr>
          <td>Ini baris kedua kolom pertama</td>
        </tr>
      </table>
    </body>
    ```

    Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatTabel.html](http://localhost/dasarWeb/buatTabel.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatTabel.html](/html/img/praktikum11/tabel10.png)

#### Bagian Sebelas: Colspan dan Rowspan

32. Tambahkan atribut `colspan=”2”` pada baris kedua kolom 1.

    ```html
    <body>
      <table
        border="1"
        height="100%"
        width="40%"
        cellpadding="20"
        cellspacing="5"
      >
        <tr>
          <td align="right" valign="bottom">
            <font face="courier" color="red" size="15"
              >Ini baris pertama kolom pertama</font
            >
          </td>
          <td>Ini baris pertama kolom kedua</td>
        </tr>
        <tr>
          <td colspan="2">Ini sekarang menjadi gabungan 2 kolom</td>
        </tr>
      </table>
    </body>
    ```

    Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatTabel.html](http://localhost/dasarWeb/buatTabel.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatTabel.html](/html/img/praktikum11/tabel11.png)

33. Tambahkan 1 kolom pada baris pertama dan baris kedua

    ```html
    <body>
      <table
        border="1"
        height="100%"
        width="40%"
        cellpadding="20"
        cellspacing="5"
      >
        <tr>
          <td align="right" valign="bottom">
            <font face="courier" color="red" size="15"
              >Ini baris pertama kolom pertama</font
            >
          </td>
          <td>Ini baris pertama kolom kedua</td>
          <td>Ini baris pertama kolom ketiga</td>
        </tr>
        <tr>
          <td colspan="2">Ini sekarang menjadi gabungan 2 kolom</td>
          <td>Ini baris kedua kolom ketiga</td>
        </tr>
      </table>
    </body>
    ```

34. Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatTabel.html](http://localhost/dasarWeb/buatTabel.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatTabel.html](/html/img/praktikum11/tabel12.png)

35. Tambahkan atribut `rowspan=”2”` pada baris pertama kolom kedua.

    ```html
    <body>
      <table
        border="1"
        height="100%"
        width="40%"
        cellpadding="20"
        cellspacing="5"
      >
        <tr>
          <td align="right" valign="bottom">
            <font face="courier" color="red" size="15"
              >Ini baris pertama kolom pertama</font
            >
          </td>
          <td rowspan="2">Ini baris pertama kolom kedua</td>
          <td>Ini baris pertama kolom ketiga</td>
        </tr>
        <tr>
          <td colspan="2">Ini sekarang menjadi gabungan 2 kolom</td>
          <td>Ini baris kedua kolom ketiga</td>
        </tr>
      </table>
    </body>
    ```

    Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatTabel.html](http://localhost/dasarWeb/buatTabel.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatTabel.html](/html/img/praktikum11/tabel13.png)

36. Catat hasil pengamatanmu di sini.

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Didalam tabel, tulisan didalamnya bisa diubah gaya, warna, dan ukuran dari tulisan dengan bantuan tag `<font>`.
    - Untuk menggabungkan dua kolom menggunakan atribut `colspan`, sedangkan untuk menggabungkan dua baris menggunakan atribut `rowspan`.
    - Dalam tampilan tabel tersebut, terdapat tabrakan antara gabungan dua kolom dibawah dan gabungan baris di kolom “**Ini baris pertama kolom kedua**” sehingga tampilannya tidak dipandang mata.

#### Bagian Duabelas: Modifikasi Rowspan

36. Hapus `rowspan=”2”` pada baris kedua kolom pertama dan tambahkan `rowspan=”2”` pada baris pertama kolom pertama

    ```html
    <body>
      <table
        border="1"
        height="100%"
        width="40%"
        cellpadding="20"
        cellspacing="5"
      >
        <tr>
          <td align="right" valign="bottom" rowspan="2">
            <font face="courier" color="red" size="15"
              >Ini baris pertama kolom pertama</font
            >
          </td>
          <td>Ini baris pertama kolom kedua</td>
          <td>Ini baris pertama kolom ketiga</td>
        </tr>
        <tr>
          <td colspan="2">Ini sekarang menjadi gabungan 2 kolom</td>
          <td>Ini baris kedua kolom ketiga</td>
        </tr>
      </table>
    </body>
    ```

37. Buka browser Anda lalu ketikkan alamat: [localhost/dasarWeb/buatTabel.html](http://localhost/dasarWeb/buatTabel.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![buatTabel.html](/html/img/praktikum11/tabel14.png)

38. Catat hasil pengamatanmu di sini.
    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Perbedaan yang paling mencolok adalah kerapian dari tabelnya.
