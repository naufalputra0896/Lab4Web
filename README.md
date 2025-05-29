# Lab4Web
Struktur Utama Website
✅ <!DOCTYPE html> dan <html lang="id">
Menentukan bahwa dokumen ini adalah HTML5.
Atribut lang="id" menunjukkan bahwa bahasa utama dokumen ini adalah Bahasa Indonesia.
✅ <head>
Bagian <head> berisi metadata dan link penting untuk tampilan website:
<meta charset="UTF-8">: Mendukung karakter Unicode.
<meta name="viewport"...>: Membuat website lebih responsif di perangkat mobile.
<title>: Judul halaman yang tampil di tab browser.
<link href="https://fonts.googleapis.com...>: Mengimpor font Open Sans dari Google Fonts.
<style>: Berisi CSS internal untuk mengatur desain tampilan halaman.
🎨 Penjelasan CSS
🌐 Global Style
css
Salin
Edit
* {
  margin: 0;
  padding: 0;
}
Reset default bawaan browser agar tampilan seragam.
💻 body
Mengatur font, warna teks, dan warna latar belakang.
Menggunakan font Open Sans.
📦 .container
Lebar tetap 980px.
Posisi tengah dengan margin: 0 auto.
Diberi bayangan (ox-shadow) dan latar putih.
🔹 .header, .nav, dan #hero
Header: Menampilkan judul situs.

Nav: Navigasi menu (Home, Artikel, About, Kontak).

Hero: Bagian sambutan/intro dengan tombol "Learn More".

📑 #main dan #sidebar
#main: Konten utama (lebar 640px).
#sidebar: Sidebar di sebelah kanan (lebar 260px).
🧱 .row dan .box
.row: Container tiga kolom.
.box: Masing-masing fitur dengan gambar bulat (.image-circle), heading, teks,
🧱 1. Deklarasi Dokumen HTML
html
Salin
Edit
<!DOCTYPE html>
<html lang="id">
<!DOCTYPE html>: Menyatakan bahwa dokumen menggunakan HTML5.
<html lang="id">: Tag pembuka HTML dengan atribut lang="id" yang menunjukkan bahwa bahasa halaman ini adalah Bahasa Indonesia.
🧠 2. Bagian <head>
html
Salin
Edit
<head>
  ...
</head>
Berisi informasi tentang dokumen, tidak ditampilkan langsung di halaman.

Langkah-langkah:
<meta charset="UTF-8" />: Mengatur encoding karakter agar bisa menampilkan huruf dan simbol dengan benar.

<meta name="viewport" content="width=device-width, initial-scale=1.0" />: Supaya halaman tampil responsif di perangkat mobile.

<title>: Judul halaman yang muncul di tab browser.

<link href=...>: Menghubungkan font Open Sans dari Google Fonts.

<style>...</style>: Menyisipkan CSS internal untuk mendesain layout.

🎨 3. CSS Styling
CSS bertanggung jawab untuk mempercantik tampilan HTML.

Langkah-langkah:
3.1 Reset default browser
css
Salin
Edit
* {
  margin: 0;
  padding: 0;
}
3.2 Mengatur tampilan dasar body
css
Salin
Edit
body {
  font-family: "Open Sans", sans-serif;
  color: #5a5a5a;
  background: #f4f4f4;
}
3.3 .container
css
Salin
Edit
.container {
  width: 980px;
  margin: 0 auto;
  box-shadow: 0 0 1em #cccccc;
  background: #fff;
}
Pusatkan halaman

Tambahkan bayangan (efek depth)

3.4 Navigasi (.nav)
css
Salin
Edit
.nav {
  background-color: #1f5faa;
}
.nav a {
  color: white;
  padding: 15px 30px;
  ...
}
Menu horizontal dengan warna biru

Saat hover, warna berubah agar interaktif

3.5 Hero section (#hero)
css
Salin
Edit
#hero {
  background: #eaeaea;
  padding: 30px;
}
Area sambutan yang berisi judul dan paragraf

Disertai tombol "Learn More"

3.6 Layout dua kolom (#main & #sidebar)
css
Salin
Edit
#main { float: left; width: 640px; }
#sidebar { float: left; width: 260px; }
Kolom kiri untuk konten utama

Kolom kanan untuk widget

📄 4. Bagian <body>
html
Salin
Edit
<body>
  <div class="container">
    ...
  </div>
</body>
Semua isi halaman berada di dalam <div class="container">.

Langkah-langkah:
4.1 Header
html
Salin
Edit
<div class="header">
  <h1>Layout Sederhana</h1>
</div>
4.2 Navigasi
html
Salin
Edit
<div class="nav">
  <a href="#" class="active">Home</a>
  ...
</div>
4.3 Hero Section
html
Salin
Edit
<section id="hero">
  <h1>Hello World!</h1>
  <p>...</p>
  <a href="home.html" class="btn">Learn more »</a>
</section>
4.4 Main Content (#main)
html
Salin
Edit
<section id="main">
  <div class="row">
    <div class="box">...</div>
    ...
  </div>
Tiga fitur dengan gambar bulat (image-circle)

Teks dan tombol “View detail”

4.5 Artikel/Entry
html
Salin
Edit
<article class="entry">
  <h2>First featurette heading.</h2>
  <img src="..." alt="" />
  <p>...</p>
</article>
Ada dua artikel

Gambar pertama di kiri, kedua di kanan (pakai class="right-img")

4.6 Sidebar
html
Salin
Edit
<aside id="sidebar">
  <div class="widget-box">
    <h3 class="title">Widget Header</h3>
    <ul>...</ul>
  </div>
  <div class="widget-box">
    <h3 class="title">Widget Text</h3>
    <p>...</p>
  </div>
</aside>
Widget navigasi dan widget teks

4.7 Footer
html
Salin
Edit
<footer>&copy; 2021 - Universitas Pelita Bangsa</footer>
Penutup halaman dengan warna gelap

✅ Kesimpulan
Struktur layout ini sudah lengkap dan responsif dasar, terdiri dari:
Header
Navigasi menu
Hero section
Konten utama 3 kolom
Artikel dengan gambar
Sidebar (widget link & teks)
Footer
