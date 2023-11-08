# Praktikum 6 - Fungsi

Fungsi adalah sub-program yang bisa digunakan kembali baik di dalam program itu sendiri, maupun di program yang lain.

Fungsi di dalam Javascript adalah sebuah objek. Karena memiliki properti dan juga _method_

### Fungsi Biasa

#### Langkah Praktikum

1. Buat File baru bernama `fungsi_javascript1.html` dan simpan dalam direktori belajarjavascript
2. Ketikkan kode program dibawah ini:

   ```html
   <!DOCTYPE html>
   <html>
     <head>
       <script>
         // Membuat fungsi
         var sayHello = () => alert("Hello World!");
       </script>
     </head>

     <body>
       <!-- Memanggil fungsi saat link diklik -->
       <a href="#" onclick="sayHello()">Klik Aku!</a>
     </body>
   </html>
   ```

3. Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

   Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/fungsi_javascript1.html](http://localhost/belajarjavascript/fungsi_javascript1.html)

   **Pastikan XAMPP Apache dalam keadaan hidup**

   ![fungsi_javascript1.html](/js/img/praktikum6/fungsi1.png)

   Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

   - Dalam menerapkan atribut `onclick` dan `alert`, terdapat alternatif yang lebih kompleks yaitu menggunakan fungsi
   - Dalam penerapan fungsi sama dengan java, yaitu `function`
   - Dalam contoh, penerapan nya itu adalah penerapan lain dalam function yaitu `arrow function`
   - Untuk penerapan `arrow function`, deklarasikan variabel yang menjadi nama dari fungsi setelah itu atur parameter dan buat _arrow_ dan _alert_
   - Dengan penerapan tersebut, program dapat berjalan

### Fungsi Parameter

Parameter adalah variable yang menyimpan nilai untuk proses di dalam fungsi.

Cara memanggil parameter dalam javascript adalah :

```js
function kali(a, b) {
  hasilKali = a * b;
  console.log("Hasil kali a*b = " + hasilKali);
}
```

#### Langkah Praktikum

1. Buat File baru bernama `fungsi_javascript2.html` dan simpan dalam direktori belajarjavascript
2. Ketikkan kode program dibawah ini:

   ```html
   <!DOCTYPE html>
   <html>
     <head>
       <script type="text/javascript">
         function total(numberA, numberB) {
           return numberA + numberB;
         }
       </script>
     </head>

     <body>
       <script type="text/javascript">
         document.write(total(2, 3));
       </script>
     </body>
   </html>
   ```

3. Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

   Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/fungsi_javascript2.html](http://localhost/belajarjavascript/fungsi_javascript2.html)

   **Pastikan XAMPP Apache dalam keadaan hidup**

   ![fungsi_javascript2.html](/js/img/praktikum6/fungsi2.png)

   Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

   - Untuk menerapkan fungsi, bisa dengan menggunakan parameter atau mengambil nilai
   - Dengan adanya parameter tersebut, fungsi bisa mengembalikan nilai / _return_
   - Untuk pengembalian nilai, **tidak wajib** akan tetapi jika membutuhkan pengembalian nilai, maka _return_ harus diterapkan
