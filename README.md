# Lab4Web
Dita Tiara Putri (312310131)
TI 23 A1

# 1 Membuat Box Element dan CSS Float Property   
membuat tiga div yang akan ditampilkan berdampingan menggunakan properti CSS float.   
Semua elemen div diatur untuk mengapung ke kiri.   
Masing-masing div diberikan warna latar belakang berbeda untuk membedakan antara satu dengan yang lain.   
```sh
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
    
    <section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div>
        </section>

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
</body>
</html>
```
![image](https://github.com/user-attachments/assets/f1db0c65-8575-4512-b368-400bb649b600)   

# 2. Mengatur Clearfix Element    
Menambahkan div keempat yang akan digunakan untuk menunjukkan cara mengatur clearfix.   
```sh
<section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div>
        <div class="div4">Div 4</div>
        </section>
```
Menambahkan ``.div4 {
        background-color: blue;
        clear: left;
        float: none;
        }``   
Properti clear: left; digunakan untuk memastikan div4 muncul di bawah semua elemen yang mengapung sebelumnya (div 1, 2, dan 3).   
float: none; memastikan bahwa div4 tidak mengapung.   

![image](https://github.com/user-attachments/assets/629e506d-ef44-4a12-928c-de9743894d41)   

# 3 Membuat Layout Sederhana  
Struktur dasar halaman web, termasuk header, navigasi, konten utama, sidebar, dan footer.   
#container mengatur lebar kontainer dan mengatur margin agar berada di tengah halaman.
Menambahkan bayangan untuk memberi efek visual.   
```sh
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
</head>
<body>
    <div id="container">
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
    </div>
    
</body>
</html>
```
![image](https://github.com/user-attachments/assets/7b6cd35f-c8a4-495d-8818-84dc01e298ff)   

Menambahkan Style CSS   
```sh
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');

/* Reset CSS */
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

/* header */
    header {
    padding: 20px;
}

header h1 {
    margin: 20px 10px;
    color: #b5b5b5;
}
```
![image](https://github.com/user-attachments/assets/8d4e973d-4c13-4746-b2cd-ebadce45cf65)   

# 5 Membuat navigasi   
Menyusun menu navigasi dengan warna latar belakang dan gaya teks.   
Mengubah warna saat mouse hover atau saat link aktif.   
Menambahkannya di file CSS   
```sh   
/* navigasi */
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

![image](https://github.com/user-attachments/assets/a8e20979-e2fb-4759-b6cb-e9ee1ea94804)   

# 6 Membuat Hero Panel   
Menambahkan judul utama dan deskripsi pada panel hero.   
```sh
<h1>Hello World!</h1>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
                elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
                vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
                pretium ac.</p>
            <a href="home.html" class="btn btn-large">Learn more &raquo;</a>`` pada `` <section id="hero">``   
```
Lalu, menambahkan CSS dibawah navigasi  
Memberikan warna latar belakang dan padding untuk tampilan yang lebih baik.   
```sh
/* Hero Panel */
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
![image](https://github.com/user-attachments/assets/1cf0b96f-9fd0-4010-afb1-7d53c45704a4)   

# 7 Mengatur Layout Main dan Sidebar    
Menambahkan sidebar yang berisi widget.   
```sh
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
```   

Selanjutnya menambahkan di CSS   
Mengatur gaya untuk setiap widget agar terpisah dengan border.   
```sh
/* widget */
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
![image](https://github.com/user-attachments/assets/ecdf1718-849b-42c6-8f9b-4d1802730aa8)   

# 8 Mengatur footer   
Mengatur footer agar muncul di bawah semua elemen lain dengan clear: both;.   
Mengatur gaya teks dan warna latar belakang.   
```sh
/* footer */
footer {
    clear:both;
    background-color:#1d1d1d;
    padding:20px;
    color:#eee;
    }
```
![image](https://github.com/user-attachments/assets/b4f922b8-23e7-4328-9ac2-d43462dd2e30)   

# 9 Menambahkan elemen lainnya pada  main content   
Menyusun konten utama dengan beberapa kotak.   
```sh
<section id="main">
            <div class="row">
                <div class="box">
                    <img src="https://dummyimage.com/120/db7d25/fff.png" alt="" class="image-circle">
                    <h3>Heading</h3>
                    <p>Donec sed odio dui. Etiam porta sem malesuada magna molliseuismod.</p>
                <a href="#" class="btn btn-default">View detail</a>
                </div>
                <div class="box">
                    <img src="https://dummyimage.com/120/3e73e6/fff.png" alt="" class="image-circle">
                <h3>Heading</h3>
                <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
                euismod.</p>
                    <a href="#" class="btn btn-default">View detail</a>
                </div>
                <div class="box">
                    <img src="https://dummyimage.com/120/71e6d4/fff.png" alt="" class="image-circle">
                <h3>Heading</h3>
                <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
                euismod.</p>
                <a href="#" class="btn btn-default">View detail</a>
                </div>
                </div>
        </section>
```   

dan css   
Mengatur setiap kotak untuk mengapung ke kiri dan berbagi lebar secara merata.   
```sh
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

.image-circle{
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
![image](https://github.com/user-attachments/assets/c0953f4b-c4ea-4cdf-9d41-a603cfa19b5c)   

# 10 Menambahkan content artikel   
Mengatur konten artikel dengan gambar dan teks   
```sh
 <section id="main">
            <hr class="divider" />
            <article class="entry">
                <h2>First featurette heading.</h2>
                <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum loremelit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nuncpretium ac.</p>
            </article>
            <hr class="divider" />
            <article class="entry">
                <h2>First featurette heading.</h2>
                <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" class="right-img">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
            </article>
        </section>
```
dan di css   
Gambar dalam artikel mengapung ke kiri dengan margin agar teks tidak menempel pada gambar.   
```sh
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


![image](https://github.com/user-attachments/assets/ef8d3249-30de-4948-b7db-6356707f6018)   

# Tugas
1. Tambahkan Layout untuk menu About
=> buat single layout yang berisi deskripsi, portfolio, dll
``<section id="about-content">...</section>``
 Membuat konten tentang diri dan portofolio.   
```sh
 <section id="about-content">
            <h2>Our Story</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor Maecenas nisl est, ultrices nec congue eget, auctor vitae massa.</p>

            <h2>Portfolio</h2>
            <div class="portfolio">
                <div class="portfolio-item">
                    <img src="https://dummyimage.com/200/71e6d4/fff.png" alt="Project 1">
                    <h3>Project Title 1</h3>
                    <p>Brief description of project 1.</p>
                </div>
                <div class="portfolio-item">
                    <img src="https://dummyimage.com/200/db7d25/fff.png" alt="Project 2">
                    <h3>Project Title 2</h3>
                    <p>Brief description of project 2.</p>
                </div>
                <div class="portfolio-item">
                    <img src="https://dummyimage.com/200/3e73e6/fff.png" alt="Project 3">
                    <h3>Project Title 3</h3>
                    <p>Brief description of project 3.</p>
                </div>
            </div>
        </section>
```
dan css nya  
``.portfolio {
    display: flex;
    justify-content: space-between;
}`` Mengatur portofolio agar tampil dalam satu baris dengan ruang di antara item.   

```sh
/* About Page Styles */
#about-content {
    padding: 20px;
}

#about-content h2 {
    margin-top: 20px; /* Spasi di atas judul */
    margin-bottom: 15px; /* Spasi di bawah judul */
}

#about-content p {
    margin-bottom: 20px; /* Spasi di bawah paragraf */
}

.portfolio {
    display: flex;
    justify-content: space-between;
}

.portfolio-item {
    width: 30%;
    text-align: center;
}

.portfolio-item img {
    width: 100%;
    border-radius: 5px;
    margin-bottom: 10px; /* Spasi di bawah gambar */
}
```
![image](https://github.com/user-attachments/assets/4eb0d278-7d7f-4a30-836f-96ff2d31424b)   
![image](https://github.com/user-attachments/assets/a0c87412-d493-4616-a558-491181808362)


# 2 Tambahkan layout untuk menu Contact
=> yang berisi form isian: nama, email, message, dll
``<section id="contact-content">...</section>``   
Membuat form kontak untuk pengunjung.   
```sh
  <section id="contact-content">
            <h2>Get in Touch</h2>
            <p>If you have any questions, feel free to contact us using the form below:</p>
            <form action="#" method="post">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>

                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="4" required></textarea>

                <button type="submit" class="btn btn-submit">Send Message</button>
            </form>
        </section>
```
dan css   
``form {
    display: flex;
    flex-direction: column;
    gap: 15px;
}``
Mengatur form agar elemen-elemen dalam form ditampilkan secara vertikal dengan jarak antara elemen.   
```sh
/* Gaya untuk Halaman Contact */
#contact-content {
    padding: 20px;
}

#contact-content h2 {
    margin-top: 20px; /* Spasi di atas judul */
    margin-bottom: 15px; /* Spasi di bawah judul */
}

#contact-content p {
    margin-bottom: 20px; /* Spasi di bawah paragraf */
}

form {
    display: flex;
    flex-direction: column;
    gap: 15px; /* Spasi antar elemen form */
}

label {
    font-weight: bold; /* Membuat label lebih tegas */
}

input[type="text"],
input[type="email"],
textarea {
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 4px;
    font-size: 14px;
}

input[type="text"]:focus,
input[type="email"]:focus,
textarea:focus {
    border-color: #1f5faa; /* Mengubah warna border saat fokus */
}

.btn-submit {
    background-color: #1f5faa;
    color: #ffffff;
    padding: 10px 15px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 16px;
}

.btn-submit:hover {
    background-color: #2b83ea; /* Mengubah warna saat hover */
}
```
![image](https://github.com/user-attachments/assets/c9a084c4-2c59-4845-b68e-5a7dda90a8df)   
![image](https://github.com/user-attachments/assets/99d1e56e-fd40-44ef-8534-47868de6dc9e)









      








  














