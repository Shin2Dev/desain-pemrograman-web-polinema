# Praktikum 4 - Jendela Dialog

Jendela dialog merupakan jendela yang digunakan untuk berinteraksi dengan pengguna. Ada tiga macam jendela dialog pada Javascript:

1. Jendela dialog `alert()`;
2. Jendela dialog `confirm()`;
3. Jendela dialog `prompt()`;

### Alert

#### Langkah Praktikum

1. Buat File baru berana `alert_javascript.html` dan simpan dalam direktori belajarjavascript
2. Ketikkan kode program dibawah ini:

   ```html
   <!DOCTYPE html>
   <html>
     <head>
       <script type="text/javascript">
         function message() {
           alert("This alert box was called with the onload event");
         }
       </script>
     </head>

     <body onload="message()"></body>
   </html>
   ```

3. Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

   Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/alert_javascript.html](http://localhost/belajarjavascript/alert_javascript.html)

   **Pastikan XAMPP Apache dalam keadaan hidup**

   ![alert_javascript](/js/img/praktikum4/alert.png)

   Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

   - Didalam program tersebut, penerapan javascriptnya terletak pada notifikasi yang muncul seperti pada tampilan tersebut
   - Untuk menampilkan notifikasi, menggunakan alert dan jika ingin menampilkannya secara langsung, maka didalam tag `<body>` ditambah atribut `onload` dan beri nilai dengan alert tersebut

### Confirm

#### Langkah Praktikum

1. Buat file baru bernama `confirm_javascript.html` dan simpan dalam direktori belajarjavascript
2. Ketikkan kode program dibawah ini:

   ```html
   <!DOCTYPE html>
   <html>
     <head>
       <title>Dialog Confirm</title>
     </head>

     <body>
       <script>
         var yakin = confirm("Apakah kamu yakin ingin mengunjungi polinema?");

         if (yakin) {
           window.location = "https://www.polinema.ac.id";
         } else {
           document.write("Baiklah, tetap di sini saja ya :)");
         }
       </script>
     </body>
   </html>
   ```

3. Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

   Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/confirm_javascript.html](http://localhost/belajarjavascript/confirm_javascript.html)

   **Pastikan XAMPP Apache dalam keadaan hidup**

   ![confirm_javascript](/js/img/praktikum4/confirm.png)

   Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

   - Sama dengan program sebelumnya, hanya saja bedanya terdapat pilihan dari notifikasinya
   - Penerapan tersebut bukan menggunakan `alert` melainkan `confirm` sehingga notifikasi yang muncul bisa memberikan opsi
   - Jika memilih **ya**, maka halaman akan beralih ke website polinema
   - Jika memilih **tidak**, maka halaman akan menampilkan output `Baiklah, tetap di sini saja ya :)`

     ![Output Confirm JavaScript](/js/img/praktikum4/output-confirm.png)

### Prompt

#### Langkah Praktikum

1. Buat file baru bernama `prompt_javascript.html` dan simpan dalam direktori belajarjavascript
2. Ketikkan kode program dibawah ini:

   ```html
   <!DOCTYPE html>
   <html>
     <head>
       <title>Dialog Prompt</title>
     </head>

     <body>
       <script>
         var nama = prompt("Siapa nama kamu?", "");
         document.write("<p>Hello " + nama + "</p>");
       </script>
     </body>
   </html>
   ```

3. Amati apa yang terjadi pada browser? Catat hasil pengamatanmu

   Simpan file tersebut, kemudian buka browser dan jalankan [localhost/belajarjavascript/prompt_javascript.html](http://localhost/belajarjavascript/prompt_javascript.html)

   **Pastikan XAMPP Apache dalam keadaan hidup**

   ![prompt_javascript](/js/img/praktikum4/prompt.png)

   Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

   - Di program ini, notifikasi nya bisa menampilkan kotak isian seperti kotak nama untuk mengisi nama
   - Jika menulis nama disitu, dan klik **ok**, maka akan menampilkan nama anda dengan gaya sapaan seperti `Hello Imam`

     ![Output Prompt JavaScript](/js/img/praktikum4/output-prompt.png)

   - Untuk menerapkan nya, dengan menggunakan prompt dan buat pertanyaan bebas sesuai keinginan
