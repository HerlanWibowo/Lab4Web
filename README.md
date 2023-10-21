# Lab4Web
## Praktikum-4
## Pertanyaan dan Tugas
### 1. Menambahkan Layout untuk menu About yang berisi Deskripsi dan Portofolio
- Source Code About

![code about](image/code%20about.png)

- Hasilnya

![web about](image/About.png)

### 2. Menambahkan Layout untuk menu Contact yang berisi Form
- Source Code Contact

![code contact](image/code%20contact.png)

- Hasilnya

![web contac](image/Contact.png)

- CSS untuk Menu About dan Contact

![csstugas](image/about+contact%20css.png)

## Langkah-Langkah Praktikum 
-  Persiapan membuat dokumen HTML dengan nama file lab4_box.html
```
<!DOCTYPE html>
<html lang="en">
<head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Box Element</title>
</head>
<body>
    <header>
        <h1>Box Element</h1>
    </header>
</body>
</html>
```
- Menambahkan section dengan menggunakan tag div 
```
    <section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div>
    </section>
```
- Menambahkan CSS pada head untuk membuat float element
```
<style>
    div {
        float:left;
        padding: 10px;
        }
    .div1 {
        background: red;
        }
    .div2 {
        background: yellow;
        }
    .div3 {
        background: green;
        }
</style>
```
- Hasilnya

![gambar1](image/Web1.png)

- Menambahkan div ke-4 lalu menggunakan Clearfix element

```
<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
    <div class="div4">Div 4</div>
</section>

.div4 {
    background-color: blue;
    clear: left;
    float: none;
}
```
- Hasilnya

![gambar2](image/Web2.png)

- Membuat Layout Sederhana<br>
membuat folder lab4_layout, kemudian buatlah file baru didalamnya dengan nama home.html, dan file css dengan nama style.css
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
    </div>
    <header>
        <h1>Layout Sederhana</h1>
    </header>
    <nav>
        <a href="home.html" class="active">Home</a>
        <a href="artikel.html">Artikel</a>
        <a href="about.html">About</a>
        <a href="kontak.html">Kontak</a>
    </nav>
    <section id="hero"></section>
    <section id="wrapper">
        <section id="main"></section>
        <aside id="sidebar"></aside>
    </section>
    <footer>
        <p>&copy; 2021 - Universitas Pelita Bangsa</p>
    </footer>
</body>
</html>
```
- Hasilnya

![gambar3](image/Web3.png)

- Menambahkan code CSS untuk Layout
```
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400
;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0
,300;0,700;1,300&display=swap');

* {
    margin: 0;
    padding: 0;
}
body {
    line-height:1;
    font-size:100%;
    font-family:'Open Sans', sans-serif;
    color:#5a5a5a;
}
#container {
    width: 980px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}
header {
    padding: 20px;
}
header h1 {
    margin: 20px 10px;
    color: #b5b5b5;
}
```
- Hasilnya

![gambar4](image/Web4.png)

- Membuaat Navigasi
```
nav {
    display: block;
    background-color: #1f5faa;
}
nav a {
    padding: 15px 30px;
    display: inline-block;
    color: #ffffff;
    font-size: 14px;
    text-decoration: none;
    font-weight: bold;
}
nav a.active,
nav a:hover {
    background-color: #2b83ea;
}
```

- Hasilnya 

![gambar5](image/Web5.png)

- Membuat Hero Panel
```
<section id="hero">
    <h1>Hello World!</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
    elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
    vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
    pretium ac.</p>
    <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
```
```
/* CSS */
#hero {
    background-color: #e4e4e5;
    padding: 50px 20px;
    margin-bottom: 20px;
}
#hero h1 {
    margin-bottom: 20px;
    font-size: 35px;
}
#hero p {
    margin-bottom: 20px;
    font-size: 18px;
    line-height: 25px;
}
```
- Hasilnya

![gambar6](image/Web6.png)

- Membuat Main dan Sidebar
```
/* CSS*/
/* main content */
#wrapper {
    margin: 0;
}
#main {
    float: left;
    width: 640px;
    padding: 20px;
}
/* sidebar area */
#sidebar {
    float: left;
    width: 260px;
    padding: 20px;
}
```
- Membuat Sidebar Widget
```
<aside id="sidebar">
    <div class="widget-box">
        <h3 class="title">Widget Header</h3>
        <ul>
        <li><a href="#">Widget Link</a></li>
        <li><a href="#">Widget Link</a></li>
        <li><a href="#">Widget Link</a></li>
        <li><a href="#">Widget Link</a></li>
        <li><a href="#">Widget Link</a></li>
        </ul>
    </div>
    <div class="widget-box">
        <h3 class="title">Widget Text</h3>
        <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
        arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer
        pharetra est nunc, nec pretium nunc pretium ac.</p>
    </div>
</aside>
```
```
/* CSS widget */
.widget-box {
    border:1px solid #eee;
    margin-bottom:20px;
}
.widget-box .title {
    padding:10px 16px;
    background-color:#428bca;
    color:#fff;
}
.widget-box ul {
    list-style-type:none;
}
.widget-box li {
    border-bottom:1px solid #eee;
    }
.widget-box li a {
    padding:10px 16px;
    color:#333;
    display:block;
    text-decoration:none;
}
.widget-box li:hover a {
    background-color:#eee;
}
.widget-box p {
    padding:15px;
    line-height:25px;
}
```
- Hasilnya 

![gambar7](image/Web7.png)

- Mengatur CSS Footer
```
/* footer */
footer {
    clear:both;
    background-color:#1d1d1d;
    padding:20px;
    color:#eee;
}
```
![gambar8](image/Web8.png)

- Menambahkan  Element Main Content
```
<section id="main">
    <div class="row">
        <div class="box">
            <img src="https://dummyimage.com/120/db7d25/fff.png" alt=""
            class="image-circle">
            <h3>Heading</h3>
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
            euismod.</p>
            <a href="#" class="btn btn-default">View detail</a>
        </div>
        <div class="box">
            <img src="https://dummyimage.com/120/3e73e6/fff.png" alt=""
            class="image-circle">
            <h3>Heading</h3>
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
            euismod.</p>
            <a href="#" class="btn btn-default">View detail</a>
        </div>
        <div class="box">
            <img src="https://dummyimage.com/120/71e6d4/fff.png" alt=""
            class="image-circle">
            <h3>Heading</h3>
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
            euismod.</p>
            <a href="#" class="btn btn-default">View detail</a>
        </div>
    </div>
</section>
```
- Tambahkan CSS untuk Main Content
```
/* box */
.box {
    display:block;
    float:left;
    width:33.333333%;
box-sizing:border-box;
    -moz-box-sizing:border-box;
    -webkit-box-sizing:border-box;
    padding:0 10px;
    text-align:center;
}
.box h3 {
    margin: 15px 0;
}
.box p {
    line-height: 20px;
    font-size: 14px;
    margin-bottom: 15px;
}
box img {
    border: 0;
    vertical-align: middle;
}
.image-circle {
    border-radius: 50%;
}
.row {
    margin: 0 -10px;
    box-sizing: border-box;
    -moz-box-sizing: border-box;
    -webkit-box-sizing: border-box;
}
.row:after, .row:before,
.entry:after, .entry:before {
    content:'';
    display:table;
}
.row:after,
.entry:after {
    clear:both;
}
```
- Hasilnya 

![gambar](image/Web9.png)

- Menambahkan Content Artikel
```
<hr class="divider" />
<article class="entry">
    <h2>First featurette heading.</h2>
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
    elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
    vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
    pretium ac.</p>
</article>
<hr class="divider" />
<article class="entry">
    <h2>First featurette heading.</h2>
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt=""
    class="right-img">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
    elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
    vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
    pretium ac.</p>
</article>
```
- Menambahkan CSS Artikel
```
.divider {
    border:0;
    border-top:1px solid #eeeeee;
    margin:40px 0;
}
/* entry */
.entry {
    margin: 15px 0;
}
.entry h2 {
    margin-bottom: 20px;
}
.entry p {
    line-height: 25px;
}
.entry img {
    float: left;
    border-radius: 5px;
    margin-right: 15px;
}
.entry .right-img {
    float: right;
}
```
- Hasilnya

![gambar10](image/Web10.png)