# Praktikum 8 - Operator

Operator adalah simbol yang digunakan untuk melakukan operasi pada suatu nilai dan variabel. Operator dalam pemrograman terbagi dalam 6 jenis:

1. Operator aritmatika;
2. Operator Penugasan (Assignment);
3. Opeartor relasi atau perbandingan;
4. Operator Logika;
5. Operator Bitwise;
6. Operator Ternary;
7. Operator aritmatika merupakan operator untuk melakukan operasi aritmatika seperti penjumlahan, pengurangan, pembagian, perkalian, dsb.
8. Operator aritmatika terdiri dari:

   | Operator    | Simbol |
   | ----------- | ------ |
   | Penjumlahan | +      |
   | Pengurangan | -      |
   | Perkalian   | \*     |
   | Pemangkatan | \*\*   |
   | Pembagian   | /      |
   | Sisa Bagi   | %      |

### Langkah Praktikum

1. Buat File baru bernama `operator_javascript.html` dan simpan dalam direktori belajarjavascript
2. Ketikkan kode program dibawah ini:

   ```html
   <!DOCTYPE html>
   <html>
     <body>
       <h2>JavaScript Operators</h2>
       <p>x = 5, y = 2, menghitung z = x + y, dan tampil z:</p>
       <p id="demo"></p>
       <script>
         var x = 5;
         var y = 2;
         var z = x + y;
         document.getElementById("demo").innerHTML = z;
       </script>
     </body>
   </html>
   ```

3. Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

   Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/operator_javascript.html](http://localhost/belajarjavascript/operator.html)

   **Pastikan XAMPP Apache dalam keadaan hidup**

   ![operator](/js/img/praktikum8/operator.png)

   Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

   - Javascript bisa menerapkan operator matematika seperti penambahan, pengurangan, perkalian, dsb
