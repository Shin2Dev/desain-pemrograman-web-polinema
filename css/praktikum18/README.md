# Praktikum 18 - _CSS Grid_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_CSS grid layout module_ menawarkan _system layout_ berbasis grid dengan baris dan kolom sehingga mempermudah melakukan desain halaman web tanpa menggunakan float dan position. Merupakan modul CSS baru untuk mendefinisikan system layout berbentuk grid dalam 2 dimensi (baris dan kolom)

![Grid](/css/img/praktikum18/grid.png)

_Grid element_

Grid layout terdiri dari satu elemen induk dengan satu atau lebih elemen anak

_CSS Grid Terminology_

- _Grid container_: Element pembungkus grid, didefinisikan dengan menuliskan: `display: grid;`
- _Grid item_; element element yang berada (1 level) di dalam grid container
- _Grid line_; Garis horizontal (kolom) atau vertical (baris) yang memisahkan grid menjadi beberapa bagian dan ditandai dengan angka
- _Grid cell_; Perpotongan/pertemuan antara baris dan kolom di dalam grid
- _Grid area_; Kumpulan lebih dari satu grid cell yang membentuk kotak
- _Grid track_; Ukuran/jarak antara 2 grid line, bisa horizontal (kolom) atau vertical (baris)
- _Grid gap_; jarak antar grid track/cell

#### Langkah Praktikum

1.  Buat satu file baru bernama `grid.html` di dalam folder dasarWeb
2.  Ketikkan ke dalam file `grid.html` tersebut kode di bawah ini.

    ```html
    <!DOCTYPE html>
    <html>
      <head>
        <title>Grid</title>
        <style>
          html {
            margin: 0;
            padding: 0;
            font-size: 20px;
            font-family: Arial;
            color: white;
            text-transform: uppercase;
            text-align: center;
          }

          .container {
            width: 600px;
            margin: 50px auto;
            border: 5px solid #333;
            box-sizing: border-box;
            padding: 5px;
            display: grid;
            grid-template-areas:
              "header header"
              "aside main"
              "nav main"
              "footer footer";
            grid-template-columns: 1fr 1.5fr;
            grid-template-rows: 1fr 1fr 1.3fr;
          }

          header {
            grid-area: header;
            background-color: #b063d8;
            display: flex;
            justify-content: center;
            align-items: center;
          }

          aside {
            grid-area: aside;
            background-color: #2f93ff;
            padding: 60px 0;
          }

          nav {
            grid-area: nav;
            background-color: #e45765;
            padding: 100px 0;
          }

          main {
            grid-area: main;
            background-color: #e0aa77;
            box-sizing: border-box;
            flex: 1.5;
            display: flex;
            justify-content: center;
            align-items: center;
          }

          footer {
            grid-area: footer;
            background-color: #666;
            padding: 20px 0;
          }
        </style>
      </head>

      <body>
        <div class="container">
          <header>Header</header>
          <aside>Aside</aside>
          <nav>Nav</nav>
          <main>Main</main>
          <footer>Footer</footer>
        </div>
      </body>
    </html>
    ```

3.  Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/grid.html](http://localhost/dasarWeb/grid.html)

    **Pastikan XAMPP Apache dalam keadaan hidup**

    ![grid.html](/css/img/praktikum18/gridCSS.png)

4.  Catat di sini apa yang anda amati dari kode program di atas

    Berdasarkan hasil yang terlihat dalam halaman web diatas, dapat saya simpulkan sebagai berikut:

    - Untuk mengatur layout pada sebuah website, selain memakai `flex`, bisa menggunakan `grid`
    - Pada halaman web tersebut, terdapat lima area yaitu _Header, Aside, Nav, Main, dan Footer_
    - Untuk pengaturan nya menggunakan `display grid` ditambah dengan `grid-template-area` untuk mengatur tata letak dari website
    - Lima area yang disebutkan tadi, diberikan nama di bagian `grid-area` di masing-masing area
