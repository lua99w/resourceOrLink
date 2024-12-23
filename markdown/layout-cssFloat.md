# CSS `float` Property

Properti **CSS `float`** digunakan untuk mengatur posisi elemen di halaman web, dengan memungkinkan elemen untuk mengapung ke kiri atau kanan, sementara elemen lainnya mengalir di sekitarnya. Ini sering digunakan untuk menata layout dan membuat elemen seperti gambar atau kolom teks saling berdampingan.

## Kapan `float` Digunakan?

Properti `float` biasanya digunakan ketika Anda ingin:
- Menyusun gambar di samping teks.
- Membuat layout dua kolom atau lebih.
- Menyelaraskan elemen seperti tombol atau gambar agar teks dapat mengalir di sekitarnya.

## Sintaks `float`

```css
elemen {
    float: left | right | none;
}
```
- `left`: Elemen akan mengapung ke kiri dan konten lainnya akan mengalir di sebelah kanan elemen tersebut.
- `right`: Elemen akan mengapung ke kanan dan konten lainnya akan mengalir di sebelah kiri elemen tersebut.
- `none`: Ini adalah nilai default. Elemen tidak mengapung dan berada dalam aliran normal dokumen.

---

## Contoh Pengggunaan `float` 
### 1. Menempatkan Gambar dengan Teks Mengelilinginya
Dengan `float`, Anda bisa membuat teks mengalir di sekitar gambar, seperti pada artikel.
```html
<img src="gambar.jpg" style="float: left; margin-right: 15px;" alt="Gambar">
<p>Ini adalah contoh teks yang mengalir di sekitar gambar. Gambar akan berada di sebelah kiri, dan teks akan mengalir ke sebelah kanan gambar.</p>
```
Pada contoh ini, gambar akan mengapung ke kiri, dan teks akan mengalir di sebelah kanannya. `margin-right: 15px;` memberi jarak antara gambar dan teks.
___
### 2. Membuat Layout Dua Kolom
`float` juga sering digunakan untuk membuat layout dua kolom. Misalnya, membuat kolom kiri dan kanan pada halaman web.

```html

<div style="float: left; width: 50%; background-color: lightblue;">Kolom Kiri</div>
<div style="float: left; width: 50%; background-color: lightgreen;">Kolom Kanan</div>
```
Pada contoh di atas, dua elemen `<div>` akan mengapung berdampingan `(left float)`, menciptakan layout dua kolom. Setiap kolom mengambil 50% dari lebar kontainer.

---

### Masalah yang Muncul dengan float
Meskipun `float` sangat berguna, ada beberapa masalah yang bisa muncul, seperti **kontainer yang kolaps**. Ini terjadi ketika elemen-elemen yang di-float keluar dari aliran normal dokumen dan kontainer tidak dapat mengukur tinggi elemen yang ada di dalamnya.

### Solusi untuk Kontainer yang Kolaps
Untuk mencegah kontainer kolaps, kita bisa menggunakan teknik yang disebut clearfix.
```css
.container::after {
    content: "";
    clear: both;
    display: table;
}
```
**apa maksud code ini?**
### 1.container::after:

Ini adalah pseudo-elemen `::after` yang diterapkan ke elemen dengan kelas `.container`. Pseudo-elemen `::after` digunakan untuk menambahkan konten setelah elemen yang ditargetkan tanpa perlu menambah elemen baru dalam HTML.
Dalam hal ini, `::after` akan membuat elemen setelah kontainer yang digunakan untuk mengatasi kolaps pada kontainer.

### 2.`content: "";`:

Properti `content` digunakan untuk mendefinisikan apa yang akan ditambahkan oleh pseudo-elemen `::after`. Di sini, content diberikan nilai string kosong `""`, yang berarti tidak ada teks atau elemen yang akan ditambahkan setelah kontainer.
Namun, menambahkan `content: ""` sangat penting agar pseudo-elemen ini benar-benar dihasilkan, meskipun tidak menambahkan konten secara visual.

### 3.`clear: both;`:

Properti `clear` digunakan untuk mengatur bagaimana elemen tersebut berinteraksi dengan elemen yang mengapung (`floated elements`).
Nilai `both` berarti bahwa elemen ini akan "membersihkan" (`clear`) elemen-elemen yang mengapung baik ke kiri (`left`) maupun ke kanan (`right`), memastikan bahwa elemen berikutnya tidak akan mengalir di sebelah elemen yang mengapung.


### 4.`display: table;`:

Properti `display: table;` digunakan untuk membuat pseudo-elemen tersebut bertindak seperti elemen tabel. Ini memaksa elemen `::after` untuk mengambil tinggi dan lebar yang dibutuhkan oleh kontainer dan memastikan kontainer tidak kolaps.
Dengan `display: table;`, elemen `::after` akan bertindak sebagai pembungkus untuk elemen-elemen yang ada dalam kontainer, mencegah kontainer tersebut menjadi kolaps setelah menggunakan `float`.


### Mengapa Menggunakan Teknik `clearfix`?
Saat kita menggunakan properti `float` pada elemen di dalam sebuah kontainer, elemen-elemen yang di-`float` tersebut "keluar" dari aliran normal dokumen. Ini menyebabkan kontainer tidak menghitung tinggi elemen-elemen yang mengapung dan kontainer tersebut bisa menjadi kolaps.

Contohnya:

```html
<div class="container">
    <div style="float: left; width: 50%;">Kolom Kiri</div>
    <div style="float: right; width: 50%;">Kolom Kanan</div>
</div>
```
Dalam kasus ini, kontainer `.container` tidak akan menghitung tinggi kedua kolom karena kolom-kolom tersebut mengapung. Tanpa `clearfix`, tinggi kontainer akan kolaps, yang akan menyebabkan layout halaman terlihat berantakan.

Untuk mengatasi masalah ini, kita menambahkan teknik `clearfix` seperti yang dijelaskan sebelumnya:

```css
Salin kode
.container::after {
    content: "";
    clear: both;
    display: table;
}
```
Dengan menambahkan kode `clearfix` ini, kita memastikan bahwa kontainer `.container` akan "memahami" tinggi dari elemen yang di-`float` di dalamnya, sehingga kontainer akan memiliki tinggi yang sesuai dengan elemen-elemen di dalamnya.

# Kesimpulan
`clearfix` adalah teknik untuk mengatasi masalah kolaps pada kontainer yang mengandung elemen-elemen yang di-float.
Dengan menggunakan pseudo-elemen `::after` bersama dengan properti `clear:` `both;` dan `display: table;`, kita memastikan bahwa kontainer tetap memiliki tinggi yang sesuai meskipun ada elemen yang mengapung di dalamnya.



Dengan teknik ini, kita memastikan bahwa kontainer akan mengukur tinggi elemen-elemen yang di-`float` dengan benar.

---

## Terima Kasih Telah Membaca!

- Hak Cipta &copy; 2024 oleh `citr.UsDev`
- Ikuti saya di [instagram](https://www.instagram.com/citr.usdev/), [GitHub](https://github.com/lua99w)
- Materi Oleh [w3school.com](https://www.w3school.com)
---

**adios semangat YA😁😹😹**

