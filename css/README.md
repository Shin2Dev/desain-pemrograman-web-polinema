# CSS (_Cascading Style Sheets_)

## Topik

- CSS

## Tujuan

Mahasiswa diharapkan dapat:

1. Mahasiswa mampu membuat web statis menggunakan HTML dan CSS
2. Mahasiswa mampu menerapkan konsep CSS Display
3. Mahasiswa mampu menerapkan konsep CSS Box Model
4. Mahasiswa mampu menerapkan konsep CSS Flex Box
5. Mahasiswa mampu menerapkan konsep CSS Grid

## Pendahuluan

### Apakah CSS?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CSS merupakan singkatan dari “_Cascading Style Sheets_“. Sesuai dengan namanya CSS memiliki sifat ”_style sheet language_” yang berarti bahasa pemrograman yang di gunakan untuk web design. CSS adalah bahasa pemrograman yang di gunakan untuk mendesign sebuah halaman website. Dalam mendesign halaman website, CSS menggunakan penanda yaitu `id` dan `class`. CSS dapat mengubah font, ukuran font, warna dan format font, mengatur ukuran layout, lebar, tinggi dan warna element, mengubah tampilan form, membuat halaman website yang _responsive_ dan masih banyak lagi.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Untuk mendesain font dapat dilakukan dengan mendefinisikan font, untuk mengatur warna bisa menggunakan color, margins digunakan untuk mengatur jarak pada luar element tertentu. mengatur warna atau gambar pada latar belakang bisa menggunakan “_background_”. mengatur ukuran _font_ gunakan “_font size_”. jenis _font_ menggunakan “_font-family_” dan banyak lagi lainnya.

### Cara Menggunakan CSS

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;File css di simpan dengan ekstensi .css. kemudian di import atau di hubungkan kedalam file HTML atau PHP yang ingin kita design dengan CSS menggunakan syntax berikut ini:

```html
<link rel="stylesheet" type="text/css" href="style.css" />
```

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Tag atas di gunakan untuk menghubungkan file HTML dengan file CSS. Syntax di letakkan pada file html. Pada atribut `rel` dan `type` di tag `link` di gunakan untuk mendefinisikan bahwa yang di panggil atau yang di hubungkan adalah file `stylesheet` atau CSS, kemudian atribut `href` di gunakan untuk meletakkan letak file CSS. pada contoh di atas file `style.css` terletak satu folder atau satu direktori dengan file html. jika file css terletak di luar folder maka bisa menghubungkanya dengan:

```html
href="../style.css"
```

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Jika file css terletak dalam sebuah folder, misalkan nama foldernya adalah ”assets“, maka untuk menghubungkannya dengan:

```html
href="../assets/style.css"
```

## Daftar Praktikum

1. [Menghubungkan HTML dengan CSS](/css/praktikum1/)
2. [Penggunaan div](/css/praktikum2/)
3. [Mengenal class dan id pada HTML](/css/praktikum3/)
4. [Mengubah _Background_ Halaman Web dengan CSS](/css/praktikum4/)
5. [Menggunakan _image_ untuk Background](/css/praktikum5/)
6. [Margin dan Padding pada CSS](/css/praktikum6/)
7. [Pengaturan Font pada CSS](/css/praktikum7/)
8. [Mengatur _Hyperlink_ dengan CSS](/css/praktikum8/)
9. [Mengatur Format Text dengan CSS](/css/praktikum9/)
10. [Mengenal Position CSS](/css/praktikum10/)
11. [Menggunakan Float](/css/praktikum11/)
12. [CSS _Layouting_](/css/praktikum12/)
13. [Display _Inline_](/css/praktikum13/)
14. [Display _inline-block_](/css/praktikum14/)
15. [Display _block_](/css/praktikum15/)
16. [_Box Model: Margin_](/css/praktikum16/)
17. [_Flex Box_](/css/praktikum17/)
18. [_CSS Grid_](/css/praktikum18/)
19. [Tugas](/css/tugas/)

## Referensi

1. Jason Beaird, The principles of Beautiful Web Design
2. Rian Ariona, Belajar HTML dan CSS (Tutorial Fundamental dalam mempelajari HTML dan CSS)
3. Adi Hadisaputra, HTML dan CSS Fundamental dari Akar menuju Daun John Duckett,HTML dan CSS design and build websites
4. https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements
5. https://css-tricks.com/almanac/properties/d/display
6. http://www.w3.org/TR/CSS2/box.html
7. http://www.w3schools.com/css/css_boxmodel.asp
