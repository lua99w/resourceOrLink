# CSS Grid

**CSS Grid Layout** adalah teknik layout dua dimensi (2D) yang memungkinkan kita untuk mengatur elemen-elemen di dalam kontainer dalam bentuk baris dan kolom. Dengan menggunakan CSS Grid, kita dapat membuat layout yang lebih kompleks dengan lebih sedikit kode dan lebih fleksibel daripada menggunakan metode lain seperti Flexbox atau float.

## Fungsi CSS Grid

CSS Grid digunakan untuk:
1. **Membuat layout dua dimensi**: Grid memungkinkan kita untuk mengatur elemen-elemen baik dalam baris maupun kolom.
2. **Membuat desain responsif**: Grid mempermudah pembuatan layout yang dapat menyesuaikan ukuran layar dengan kontrol yang lebih besar atas penataan elemen.
3. **Menata elemen secara lebih terstruktur**: Dengan Grid, kita bisa mengatur posisi elemen dengan menentukan baris dan kolom secara eksplisit.

## Kapan Menggunakan CSS Grid?

CSS Grid digunakan saat Anda ingin:
- Membuat layout yang lebih kompleks yang melibatkan pengaturan elemen-elemen di dalam baris dan kolom.
- Mengatur elemen-elemen di dalam kontainer secara eksplisit dalam grid 2D.
- Membuat desain responsif yang dapat menyesuaikan ukuran layar dengan mudah.
  
CSS Grid sangat cocok digunakan pada layout yang melibatkan banyak kolom dan baris, seperti grid gambar, tabel, atau desain web yang lebih kompleks.

## Cara Kerja CSS Grid

Untuk menggunakan CSS Grid, Anda hanya perlu menetapkan properti `display: grid;` pada kontainer, dan kemudian mengatur elemen-elemen di dalamnya menggunakan properti seperti `grid-template-columns`, `grid-template-rows`, `grid-gap`, dan lainnya.

### Properti Utama CSS Grid

- **`display: grid;`**: Menyatakan bahwa elemen kontainer akan menggunakan grid layout.
- **`grid-template-columns`**: Menentukan jumlah dan ukuran kolom dalam grid.
- **`grid-template-rows`**: Menentukan jumlah dan ukuran baris dalam grid.
- **`grid-gap`**: Menentukan jarak antar baris dan kolom.
- **`grid-column`**: Menentukan posisi elemen dalam kolom grid.
- **`grid-row`**: Menentukan posisi elemen dalam baris grid.

## Contoh Penggunaan CSS Grid

### 1. Membuat Layout Grid Sederhana

```html
<div style="display: grid; grid-template-columns: repeat(3, 1fr); grid-gap: 10px;">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
    <div>Item 4</div>
    <div>Item 5</div>
    <div>Item 6</div>
</div>
```

---

### penjelasan

`display: grid;` mengubah kontainer menjadi `grid`.
`grid-template-columns: repeat(3, 1fr);` membuat tiga kolom dengan lebar yang sama.
`grid-gap: 10px;` memberi jarak 10px antara baris dan kolom.

---

### 2. Menentukan Ukuran Kolom dan Baris

---

```html

<div style="display: grid; grid-template-columns: 200px 1fr 2fr; grid-template-rows: 100px auto;">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
    <div>Item 4</div>
</div>
```
---

### Penjelasan:

- `grid-template-columns: 200px 1fr 2fr;` membuat tiga kolom: kolom pertama memiliki lebar `200px`, kolom kedua `1fr` (ruang fleksibel), dan kolom ketiga `2fr` (ruang fleksibel dua kali lebih banyak dari kolom kedua).

- `grid-template-rows: 100px auto;` membuat dua baris: baris pertama memiliki tinggi `100px`, dan baris kedua memiliki tinggi otomatis berdasarkan konten.

---

### 3. Menggunakan `grid-column` dan `grid-row` untuk Menata Elemen
```html

<div style="display: grid; grid-template-columns: 1fr 1fr 1fr; grid-gap: 20px;">
    <div style="grid-column: span 2;">Item 1 (lebar 2 kolom)</div>
    <div>Item 2</div>
    <div>Item 3</div>
    <div>Item 4</div>
</div>
```
### Penjelasan:

- `grid-column: span 2;` membuat elemen pertama (Item 1) melebar hingga dua kolom.
- `grid-template-columns: 1fr 1fr 1fr;` membagi kontainer menjadi tiga kolom dengan lebar yang sama.

---

### 4. Membuat Layout Responsif dengan  `CSS Grid`
```html
<div style="display: grid; grid-template-columns: repeat(auto-fill, minmax(200px, 1fr)); grid-gap: 20px;">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
    <div>Item 4</div>
    <div>Item 5</div>
</div>
```
### Penjelasan:

- `grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));` membuat grid yang secara otomatis menyesuaikan jumlah kolom berdasarkan lebar kontainer, dengan setiap kolom memiliki lebar minimal `200px` dan fleksibel hingga ukuran maksimal `1fr` (fraksi dari ruang yang tersedia).

---


Ini memungkinkan layout untuk responsif, sehingga jumlah kolom akan berubah tergantung pada ukuran layar.
Keuntungan Menggunakan CSS Grid

Lebih fleksibel: CSS Grid memungkinkan pengaturan layout dua dimensi (baris dan kolom) secara lebih mudah, yang tidak bisa dilakukan oleh Flexbox.

Responsif secara otomatis: Grid bisa menyesuaikan ukuran kolom dan baris untuk memberikan layout yang sesuai dengan ukuran layar.

Lebih sedikit kode: Dibandingkan dengan menggunakan teknik lain seperti float atau position, CSS Grid memungkinkan kita membuat layout yang lebih kompleks dengan lebih sedikit kode.

Kontrol penuh atas elemen: Grid memberikan kontrol yang lebih besar atas posisi dan ukuran elemen-elemen dalam layout.

---
# Kesimpulan


`CSS Grid` adalah teknik layout yang sangat powerful untuk membuat desain web dua dimensi yang lebih kompleks dan fleksibel. Dengan menggunakan properti seperti `grid-template-columns`, `grid-template-rows`, `grid-gap`, serta `grid-column` dan `grid-row`, Anda dapat mengatur layout dengan cara yang lebih efisien dan responsif.

`CSS Grid` sangat cocok digunakan ketika Anda ingin mengatur banyak elemen dalam baris dan kolom secara eksplisit, membuat layout responsif yang lebih mudah dikelola, dan membuat desain yang lebih fleksibel dengan kontrol penuh atas elemen-elemen yang ada

## Terima Kasih Telah Membaca!

- Hak Cipta &copy; 2024 oleh `citr.UsDev`
- Ikuti saya di [instagram](https://www.instagram.com/citr.usdev/), [GitHub](https://github.com/lua99w)
- Materi Oleh [w3school.com](https://www.w3school.com)
---

**adios semangat YA😁😹😹**

