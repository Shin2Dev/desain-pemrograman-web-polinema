# Tugas

### Buatlah tampilan dari hasil flex-box sebelumnya menjadi seperti ini

![Tugas 1](/css/img/tugas/tugas1.png)

#### Jawaban

**HTML (Tidak ada Perubahan)**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Latihan Flexbox</title>
    <link rel="stylesheet" href="styleFlexbox.css" />
  </head>

  <body>
    <div class="container-satu">
      <div class="kolom-utama">
        <h2>Judul Artikel</h2>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Suscipit
          eos, nostrum vero, iusto deserunt adipisci labore error facere vel
          velit quibusdam sed dolor rerum? Dolorem explicabo beatae quia impedit
          repudiandae.
        </p>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Id pariatur
          officia quasi aliquid neque vero, quibusdam quo? Asperiores pariatur
          aliquam eveniet praesentium mollitia perspiciatis culpa ea ducimus
          accusamus nulla. Minima.
        </p>
      </div>

      <div class="sidebar-satu">
        <h3>Sidebar Satu</h3>
        <ul>
          <li><a href="">Link 1</a></li>
          <li><a href="">Link 2</a></li>
          <li><a href="">Link 3</a></li>
          <li><a href="">Link 4</a></li>
          <li><a href="">Link 5</a></li>
        </ul>
      </div>

      <div class="sidebar-dua">
        <h3>Sidebar Dua</h3>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas
          nobis tenetur eaque mollitia earum debitis ratione. Consequatur enim
          ullam vel quibusdam. Voluptatem illum sequi minima velit ipsum eveniet
          dicta maiores.
        </p>
      </div>
    </div>
  </body>
</html>
```

**CSS**

```css
html,
body {
  margin: 0;
  padding: 0;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  background-color: #ddd;
  line-height: 1.65;
  padding-bottom: 1000px;
}

.sidebar-satu {
  width: 20%;
  order: 1;
}

.kolom-utama {
  order: 2;
  width: 50%;
  margin-right: 5%;
}

.sidebar-dua {
  order: 3;
  width: 25%;
}

.container-satu {
  width: 800px;
  margin: 50px auto;
  background-color: #fff;
  padding: 20px;
  box-sizing: border-box;
  display: flex;
}
```

Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/flexbox.html](http://localhost/dasarWeb/flexbox.html)

**Pastikan XAMPP Apache dalam keadaan hidup**

![flexbox.html](/css/img/tugas/jawab1.png)

### 2. Tambahkan gambar dan aplikasikan permainan warna untuk backgroundnya supaya menjadi lebih menarik

**Modifikasi HTML**

```html
<div class="kolom-utama">
  <h2>Judul Artikel</h2>
  <div class="gambar">
    <img src="img/bunga1.jpeg" alt="Bunga" />
  </div>
  <p>
    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Suscipit eos,
    nostrum vero, iusto deserunt adipisci labore error facere vel velit
    quibusdam sed dolor rerum? Dolorem explicabo beatae quia impedit
    repudiandae.
  </p>
  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Id pariatur officia
    quasi aliquid neque vero, quibusdam quo? Asperiores pariatur aliquam eveniet
    praesentium mollitia perspiciatis culpa ea ducimus accusamus nulla. Minima.
  </p>
</div>
```

**Modifikasi CSS**

```css
.gambar img {
  width: 100%;
  height: auto;
  border: 5px solid #555;
}

.container-satu {
  width: 800px;
  margin: 50px auto;
  background-color: #f5f5f5;
  padding: 20px;
  box-sizing: border-box;
  display: flex;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
```

Simpan file tersebut, kemudian buka browser dan jalankan [localhost/dasarWeb/flexbox.html](http://localhost/dasarWeb/flexbox.html)

**Pastikan XAMPP Apache dalam keadaan hidup**

![flexbox.html](/css/img/tugas/jawab2.png)
