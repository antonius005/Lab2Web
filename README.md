# Praktikum 2 - Pemrograman Web
### Antonius Simanjuntak - 312010004
### TI.20.B.1 - PEMPROGRAMAN WEB
### UNIVERSITAS PELITA BANGSA

## LANGKAH 1
buat dokumen html dengan isi berikut :
![vc css dasar](https://user-images.githubusercontent.com/101562285/158750436-3f308d96-51fa-4faf-8a32-e7ab67effa84.png)
```
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>CSS Dasar</title>
</head>
<body>
 <header>
 <h1>CSS Internal dan <i>Inline CSS</i></h1>
 </header>
 <nav>
 <a href="lab2_css_dasar.html">CSS Dasar</a>
 <a href="lab2_css_eksternal.html">CSS Eksternal</a>
 <a href="lab1_tag_dasar.html">HTML Dasar</a>
 </nav>
 <!-- CSS ID Selector -->
 <div id="intro">
 <h1>Hello World</h1>
 <p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman
Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat
adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML
dan CSS.</p>
 <!-- CSS Class Selector -->
 <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
 </div>
</body>
</html>
```
lalu buka pada browser untuk melihat hasilnya
![css dasar - 1](https://user-images.githubusercontent.com/101562285/158751400-114e3209-15f5-4ce0-acf2-6bd8d32f75d7.png)


## LANGKAH 2
### Mendeklarasikan CSS Internal
Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen
```
<head>
 <title>CSS Dasar</title>
 <style>
 body {
 font-family:'Open Sans', sans-serif;
 }
 header {
 min-height: 80px;
 border-bottom:1px solid #77CCEF;
 }
 h1 {
 font-size: 24px;
 color: #0F189F;
 text-align: center;
 padding: 20px 10px;
 }
 h1 i {
 color:#6d6a6b;
 }
 </style>
</head>
```
![vc css dasar 2](https://user-images.githubusercontent.com/101562285/158751131-884f90bb-431c-4617-ab91-9ebbb22215e7.png)

Selanjutnya simpan perubahan yang ada, dan lakukan refresh pada browser untuk melihat
hasilnya
![css dasar - 2](https://user-images.githubusercontent.com/101562285/158751561-7e5e4a4d-6bab-4cd6-8e47-db384a3cf0f7.png)


## LANGKAH 3
### Menambahkan Inline CSS
 tambahkan deklarasi inline CSS pada tag <p> seperti berikut
 ```
 <p style="text-align: center; color: #ccd8e4;">
 ```
 before: 
  ![vc css dasar 3](https://i.imgur.com/PdQFu6Z.png)
 after:
  ![vc css dasar 3](https://user-images.githubusercontent.com/101562285/158752097-dcce749c-1a08-4a76-b42d-7936e4ff3f82.png)
 Simpan kembali dan refresh kembali browser untuk melihat perubahannya:

 ![css dasar - 3](https://user-images.githubusercontent.com/101562285/158752246-536222aa-961e-4d0d-aea3-5635b695f3e6.png)

  
 ## LANGKAH 4
 ### Membuat CSS Eksternal
 Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut
 ```
 nav {
background: #20A759;
color:#fff;
padding: 10px;
}
nav a {
color: #fff;
text-decoration: none;
padding:10px 20px;
}
nav .active,
nav a:hover {
background: #0B6B3A;
}
```
![vc css dasar 4](https://user-images.githubusercontent.com/101562285/158752489-a4b0c63e-5240-492a-9571-da93e3f60eeb.png)
Kemudian tambahkan tag `<link>`untuk merujuk file css yang sudah dibuat pada bagian `<head>`
```
<head>
 <!-- menyisipkan css eksternal -->
 <link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>
```
![vc css dasar 5](https://user-images.githubusercontent.com/101562285/158752696-ca7b8882-2ce5-44de-9926-2596fa493663.png)

Selanjutnya refresh kembali browser untuk melihat perubahannya
![css dasar - 4](https://user-images.githubusercontent.com/101562285/158752722-37340832-f4dd-4828-9c3b-82ec30495f98.png)

## LANGKAH 5
### Menambahkan CSS Selector
Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file
style_eksternal.css, tambahkan kode berikut

```
/* ID Selector */
#intro {
background: #418fb1;
border: 1px solid #099249;
min-height: 100px;
padding: 10px;
}
#intro h1 {
text-align: left;
border: 0;
color: #fff;
}
/* Class Selector */
.button {
 padding: 15px 20px;
background: #bebcbd;
color: #fff;
display: inline-block;
margin: 10px;
text-decoration: none;
}
.btn-primary {
background: #E42A42;
}
```
![vc css dasar 6](https://user-images.githubusercontent.com/101562285/158752914-8728a251-206a-45fd-a28c-87f4a40aee5c.png)
Kemudian simpan kembali dan refresh browser untuk melihat perubahannya.
![css dasar - 5](https://user-images.githubusercontent.com/101562285/158752945-fdabe014-03bb-4177-8aba-19decf687ae5.png)

# Pertanyaan dan Tugas
### 1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini
![1_pertanyaan](https://user-images.githubusercontent.com/101562285/158758896-ab070c47-4397-49ae-8126-63e997cd873f.png)

### 2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan penjelasannya!
perbedaaannya jika hanya h1{} maka akan merubah semua yang ada didalam elemen h1 sedangkan intro h1 hanya akan merubah yang memiliki tag intro

### 3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!
jika ketiga CSS merubah elemen yang sama maka deklarasi tersebut akan mengikuti aturan prioritas
dimana prioritas CSS nya seperti ini:
1. inline CSS
2. ID selector CSS
3. internal CSS
4. external CSS

contoh:

ini adalah tampilan coding pada html testing dimana terdapat 2 kalimat yang memiliki elemen yang sama yaitu h1:
 ![pertanyaan  3_1](https://user-images.githubusercontent.com/101562285/158759333-363916af-12c4-487a-b2be-c13f12db7b3e.png)

 disini bisa dilihat sudah terdapat 2 css mencoba merubah warna text h1 :
 ![pertanyaan  3_2](https://user-images.githubusercontent.com/101562285/158759372-1ac80708-e2e5-450e-8c92-721c57c40bd9.png) 

 sedangkan eksternal css berupa :
 ![pertanyaan  3_3](https://user-images.githubusercontent.com/101562285/158759408-b0ada372-f5ae-4223-8494-b7dcd1283a7b.png)

 dan hasil adalah :
 ![pertanyaan  3_4](https://user-images.githubusercontent.com/101562285/158759435-24550d08-478e-4557-a252-b0b4930d72e4.png)
jadi saya mengambil kesimpulan bahwa semakin spesifik CSS tersebut maka prioritas semakin tinggi

### 4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! ( <p id="paragraf-1" class="text-paragraf"> )
hasilnya sesuai dengan kesimpulan saya sebelumnya semakin spesifik css tersebut maka akan semakin tinggi prioritas css tersebut
![pertanyaan  4_1](https://user-images.githubusercontent.com/101562285/158759652-d0955c0b-36ff-459e-ab7b-1ba2b04fd68a.png)
disitu bisa dilihat terdapat 2 css yang merujuk ke elemen yang sama tapi 1 merujuk dengan id yang birisi font 40 dan warna emas sedangkan yang satu lagi merujuk dengan class yang berisi font 10 dan warna maroon
hasilnya adalah:
![pertanyaan  4_2](https://user-images.githubusercontent.com/101562285/158759673-2c1ae126-9617-4b24-a5fa-a107f057223f.png)
text "testing" tersebut mengikuti css selector id daripada selector class dikarenakan id lebih spesifik daripada class
