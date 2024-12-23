# Apa Itu Tag `<section>`, `<article>`, dan `<aside>`?

Ketiga tag ini digunakan untuk mengorganisir dan menyusun konten dalam halaman web. Masing-masing memiliki tujuan yang berbeda, dan mereka membantu pengunjung serta mesin pencari memahami struktur halaman dengan lebih baik. Berikut penjelasan lebih mendalam tentang setiap tag:
<hr>

### 1. `<section>`: Untuk Bagian Tematik

Tag `<section>` digunakan untuk membagi halaman web menjadi beberapa bagian atau tema yang memiliki hubungan. Setiap bagian ini biasanya memiliki topik atau subtopik tertentu dan sering kali dilengkapi dengan judul untuk menjelaskan apa yang ada di dalamnya.

### Contoh dalam Kehidupan Sehari-hari
Bayangkan Anda membaca buku yang memiliki beberapa bab. Setiap bab memiliki topik yang berbeda, seperti "Sejarah Dunia", "Teknologi Modern", dan "Sains Alam". Nah, setiap bab ini adalah sebuah bagian tematik yang dapat Anda kelompokkan dengan `<section>`.

### Contoh HTML
Misalnya, dalam sebuah halaman tentang website restoran, Anda dapat membagi halaman menjadi beberapa bagian, seperti "Menu", "Lokasi", dan "Testimoni".

```html
<section>
  <h2>Menu</h2>
  <p>Di sini kami menyediakan berbagai pilihan makanan lezat, mulai dari nasi goreng hingga pasta.</p>
</section>

<section>
  <h2>Lokasi</h2>
  <p>Restoran kami terletak di pusat kota, dekat dengan taman kota.</p>
</section>

<section>
  <h2>Testimoni</h2>
  <p>Pengunjung kami menyukai makanan di sini. "Makanannya luar biasa!" - John Doe</p>
</section>
```
### penjelasan
Setiap bagian `<section>` membahas topik yang berbeda: menu, lokasi, dan testimoni. Ini memudahkan pengunjung untuk menemukan informasi yang mereka butuhkan.

<hr>

### 2. `<article>`: Konten yang Berdiri Sendiri
Tag `<article>` digunakan untuk konten yang dapat berdiri sendiri, yang berarti konten tersebut bisa dipahami dan dipublikasikan secara terpisah dari halaman utama. Biasanya, konten ini berupa **artikel**, **berita**, atau **posting** **blog**.

**Contoh dalam Kehidupan Sehari-hari**: Misalnya, Anda membaca sebuah artikel di koran atau blog tentang "5 Tips Sehat untuk Hidup Lebih Baik". Artikel tersebut adalah **konten mandiri** yang bisa dipahami dan bermanfaat meskipun tanpa konteks halaman yang lebih besar.

**Contoh HTML**: Dalam website yang membahas tentang kesehatan, setiap artikel yang membahas topik kesehatan tertentu bisa dibungkus dengan `<article>`
```html
<article>
  <h2>5 Tips Sehat untuk Hidup Lebih Baik</h2>
  <p>Pola makan yang sehat sangat penting untuk tubuh kita. Berikut adalah 5 tips sederhana untuk hidup lebih sehat...</p>
</article>

<article>
  <h2>Cara Mengatasi Stres dengan Yoga</h2>
  <p>Stres bisa mempengaruhi kesehatan mental kita. Yoga adalah salah satu cara efektif untuk meredakan stres...</p>
</article>
```
### penjelasan
Setiap `<article>` adalah artikel terpisah yang bisa dibaca dan dipahami sendiri. Meskipun berada dalam satu halaman yang sama, setiap artikel ini tidak bergantung pada artikel lain.

<hr>

### 3. `<aside>`: Konten Tambahan yang Tidak Utama

Tag `<aside>` digunakan untuk **informasi yang berkaitan dengan konten utama**, tetapi bukan bagian inti dari konten tersebut. Konten ini bisa berupa informasi tambahan, seperti **sidebar**, **link** terkait, atau **kutipan** yang mendukung topik utama, tapi tidak langsung menjadi bagian dari cerita utama.


**Contoh dalam Kehidupan Sehari-hari**: Bayangkan Anda membaca sebuah artikel di majalah tentang "Tips Berkebun di Rumah". Di sebelah artikel utama, ada informasi tambahan di sidebar seperti "Alat Berkebun yang Direkomendasikan" atau "Panduan Merawat Tanaman Indoor". Sidebar ini adalah **informasi tambahan**, tetapi tetap relevan dengan artikel utama.


**Contoh HTML**: Misalnya, di sebuah artikel tentang resep masakan, Anda bisa menambahkan tips tambahan atau link ke resep lainnya dalam `<aside>`.
```html
<article>
  <h2>Resep Nasi Goreng Spesial</h2>
  <p>Inilah resep nasi goreng spesial yang mudah dibuat di rumah...</p>
</article>

<aside>
  <h3>Tips Memasak Nasi Goreng</h3>
  <ul>
    <li>Gunakan nasi yang sudah dingin agar lebih enak.</li>
    <li>Tambahkan sedikit kecap manis untuk rasa yang lebih kaya.</li>
  </ul>
</aside>

<aside>
  <h3>Resep Terkait</h3>
  <ul>
    <li><a href="#">Resep Mie Goreng Spesial</a></li>
    <li><a href="#">Resep Ayam Goreng Crispy</a></li>
  </ul>
</aside>
```

**Penjelasan**:

Artikel utama tentang Nasi Goreng dibungkus dengan `<article>`.
- Informasi tambahan, seperti tips memasak atau resep terkait, dibungkus dengan `<aside>` karena mereka memberikan 
- informasi tambahan tetapi tidak langsung menjadi bagian dari artikel utama.

<hr>

### Ringkasan Perbedaan

| **Tag**     | **Tujuan**                                                                 | **Kapan Digunakan**                                                       | **Contoh dalam Kehidupan Sehari-hari**                           |
|-------------|---------------------------------------------------------------------------|---------------------------------------------------------------------------|-------------------------------------------------------------------|
| `<section>` | Membagi halaman menjadi bagian tematik yang memiliki hubungan.            | Digunakan untuk mengelompokkan konten berdasarkan topik besar atau subtopik. | Bab dalam buku atau bagian dalam website (Menu, Testimoni, dll.)  |
| `<article>` | Untuk konten yang berdiri sendiri dan dapat dipahami tanpa konteks lebih lanjut. | Digunakan untuk artikel atau konten independen yang bisa dibaca secara terpisah. | Artikel di blog, berita, atau postingan mandiri                  |
| `<aside>`   | Untuk informasi tambahan atau sampingan yang relevan tetapi tidak utama.   | Digunakan untuk sidebar, cuplikan, atau link terkait.                     | Sidebar, tips tambahan, atau link terkait dengan artikel utama   |


<hr>

### Kesimpulan 
- `<section>` adalah untuk mengorganisir bagian besar dari halaman berdasarkan topik atau tema.
- `rticle>` digunakan untuk konten yang bisa berdiri sendiri, seperti artikel, berita, atau postingan blog.
- `<aside>` digunakan untuk menampilkan informasi tambahan yang relevan tetapi tidak menjadi bagian utama dari halaman.

Dengan memahami ketiga tag ini, Anda bisa menyusun halaman web yang lebih terstruktur dan memudahkan pengunjung untuk menemukan informasi yang mereka butuhkan.

```css

Dokumen ini telah disusun dengan lengkap, mencakup penjelasan tentang tag `<section>`, `<article>`, dan `<aside>` beserta contoh penggunaannya dalam HTML, dan penjelasan ringkas perbedaan antara ketiganya.
```

## Terima Kasih Telah Membaca!

- Hak Cipta &copy; 2024 oleh `citr.UsDev`
- Ikuti saya di [instagram](https://www.instagram.com/citr.usdev/), [GitHub](https://github.com/lua99w)
- Materi Oleh [w3school.com](https://www.w3school.com)
---

**adios semangat YA😁😹😹**

