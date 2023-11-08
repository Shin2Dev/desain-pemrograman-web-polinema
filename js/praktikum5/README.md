# Praktikum 5 - Variabel

Cara membuat variabel yang umum digunakan di javascript adalah menggunakan kata kunci `var` lalu diikuti dengan nama variabel dan nilainya.

Contoh:

```js
var title = "Belajar Pemrograman Javascript";
```

### Menampilkan isi Variabel

Untuk menampilkan isi variabel, kita bisa memanfaatkan fungsi-fungsi untuk menampilkan output seperti:

- Fungsi `console.log()` menampilkan output ke console javascript;
- Fungsi `document.write()` menampilkan output ke dokumen HTML;
- Fungsi `alert()` menampilkan output ke jendela dialog.

#### Langkah Praktikum

1. Buat File baru bernama `variabel_javascript.html` dan simpan dalam direktori belajarjavascript
2. Ketikkan kode program dibawah ini:

   ```html
   <!DOCTYPE html>
   <html lang="en">
     <head>
       <title>Belajar Variabel dalam Javascript</title>
       <script>
         var name = "Javascript";
         var visitorCount = 50322;
         var isActive = true;

         alert("Selamat datang di " + name);

         document.write("Nama Situs: " + name + "<br>");
         document.write("Jumlah Pengunjung: " + visitorCount + "<br>");
         document.write("Status Aktif: " + isActive + "<br>");
       </script>
     </head>
   </html>
   ```

3. Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

   Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/variabel_javascript.html](http://localhost/belajarjavascript/variabel_javascript.html)

   **Pastikan XAMPP Apache dalam keadaan hidup**

   ![variabel_javascript](/js/img/praktikum5/variabel1.png)

   ![variabel_javascript](/js/img/praktikum5/variabel2.png)

   Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

   - Untuk membuat variabel, dengan mendeklarasikan `var` dan beri nilai
   - Untuk nilai nya bebas dan tidak terikat oleh tipe data spesifik
   - Dengan variabel, output nya bisa dimanipulasi berdasarkan nilai dari variabelnya

### Menghapus Variabel

Penghapusan variabel dalam Javscript memang jarang dilakukan. Namun, untuk program yang membutuhkan ketelitian dalam alokasi memori, penghapusan variabel perlu dilakukan agar penggunaan memori lebih optimal.

Penghapusan variabel dapat dilakukan dengan katakunci `delete`.

Contoh:

```js
bookTitle = "Belajar Pemrograman Javascript";
delete bookTitle;
```

Maka variabel bookTitle akan menghilang dari memori.
