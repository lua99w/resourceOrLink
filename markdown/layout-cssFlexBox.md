# CSS Flexbox

**CSS Flexbox** (Flexible Box Layout) adalah sebuah model layout di CSS yang memungkinkan kita untuk mendistribusikan ruang di antara elemen-elemen dalam kontainer dengan cara yang lebih efisien dan fleksibel. Flexbox sangat berguna untuk desain responsif dan mengatur elemen-elemen di dalam kontainer dengan mudah, baik dalam satu baris (row) maupun dalam satu kolom (column).

## Fungsi Flexbox

Flexbox digunakan untuk:
1. **Menyusun elemen dalam satu baris atau kolom**: Flexbox memungkinkan kita untuk mengatur elemen dalam satu baris atau kolom, bahkan ketika ukuran elemen-elemen tersebut tidak tetap.
2. **Membuat layout responsif**: Flexbox secara otomatis menyesuaikan elemen-elemen agar tampil rapi meski dalam ukuran layar yang berbeda.
3. **Mengatur ruang antar elemen**: Flexbox memberikan kontrol yang mudah untuk mengatur jarak antar elemen, sejajar, dan meratakan elemen di dalam kontainer.

## Kapan Menggunakan Flexbox?

Flexbox digunakan saat Anda ingin:
- Membuat layout satu dimensi (seperti baris atau kolom).
- Menyusun elemen secara responsif tanpa perlu menggunakan posisi absolut atau float.
- Membuat desain yang dapat menyesuaikan ruang yang tersedia di layar, seperti kolom dengan ukuran yang fleksibel atau tombol yang otomatis merata.

## Cara Kerja Flexbox

Untuk menggunakan Flexbox, Anda perlu mengatur dua properti utama:
1. **`display: flex;`** pada kontainer.
2. Kemudian, Anda dapat mengatur berbagai properti untuk elemen-elemen di dalam kontainer seperti `justify-content`, `align-items`, dan `flex-wrap`.

### Properti Utama Flexbox

- **`display: flex;`**: Menyatakan bahwa elemen kontainer akan menggunakan Flexbox layout.
- **`justify-content`**: Mengatur penyusunan elemen-elemen utama (horizontal jika `flex-direction` adalah `row`).
  - Nilai yang umum digunakan: `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `space-evenly`.
- **`align-items`**: Menyusun elemen-elemen secara vertikal dalam kontainer.
  - Nilai yang umum digunakan: `flex-start`, `flex-end`, `center`, `baseline`, `stretch`.
- **`flex-direction`**: Mengatur arah penyusunan elemen (baris atau kolom).
  - Nilai yang umum digunakan: `row` (default), `column`, `row-reverse`, `column-reverse`.
- **`flex-wrap`**: Menentukan apakah elemen-elemen yang tidak muat dalam satu baris akan melanjutkan ke baris berikutnya.
  - Nilai yang umum digunakan: `nowrap` (default), `wrap`, `wrap-reverse`.

## Contoh Penggunaan Flexbox

### 1. Membuat Layout Satu Baris

```html
<div style="display: flex; justify-content: space-between;">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
</div>
```

### penjelasan
`display: flex;` membuat elemen dalam kontainer disusun dalam satu baris.
`justify-content:` space-between; memberikan jarak antar elemen dengan ruang kosong di antara mereka.


---

### 2. Membuat Layout Kolom
```html
<div style="display: flex; flex-direction: column; align-items: center;">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
</div>
```

---

### Penjelasan:

`flex-direction: column;` mengubah arah penyusunan elemen menjadi kolom.
`align-items: center;` meratakan elemen secara vertikal di tengah kontainer.

### 3. Membuat Layout Responsif dengan flex-wrap
```html
<div style="display: flex; flex-wrap: wrap; justify-content: space-around;">
    <div style="flex: 1 1 200px;">Item 1</div>
    <div style="flex: 1 1 200px;">Item 2</div>
    <div style="flex: 1 1 200px;">Item 3</div>
    <div style="flex: 1 1 200px;">Item 4</div>
</div>
```
---

### Penjelasan:

`flex-wrap: wrap;` memungkinkan elemen-elemen untuk membungkus ke baris baru jika tidak cukup ruang dalam satu baris.
`justify-content: space-around;` memberi jarak antar elemen.
`flex: 1 1 200px;` mengatur elemen agar memiliki lebar fleksibel, dengan lebar dasar 200px.

---

### 4. Menyusun Elemen dengan Ruang Sama Rata
```html

<div style="display: flex; justify-content: space-evenly;">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
</div>
```

---

### Penjelasan:

`justify-content: space-evenly;` mengatur elemen-elemen agar tersebar secara merata dengan jarak yang sama di antara mereka.

---

### Keuntungan Menggunakan `Flexbox`

Mudah digunakan: `Flexbox` lebih mudah dan fleksibel dibandingkan dengan teknik layout lama seperti `float` atau `positioning`.

Kontrol yang lebih besar: Anda dapat dengan mudah mengatur jarak, penyusunan, dan pengaturan elemen tanpa perlu mengandalkan ```css
@media query``` atau perhitungan manual.

Responsif secara otomatis: Elemen-elemen di dalam kontainer akan menyesuaikan dengan ukuran layar, tanpa perlu banyak CSS tambahan.

Mengurangi kode `CSS: Flexbox` memudahkan pembuatan layout tanpa perlu banyak menggunakan kelas tambahan atau mengatur posisi elemen secara manual.

---

# Kesimpulan

Flexbox adalah cara yang efisien dan mudah digunakan untuk membuat layout yang responsif dan fleksibel. Dengan Flexbox, Anda dapat mengatur elemen dalam baris atau kolom, mengatur jarak antar elemen, dan membuat desain yang fleksibel yang bisa menyesuaikan ukuran layar.

Dengan memanfaatkan properti seperti `justify-content`, `align-items`, `flex-direction`, dan `flex-wrap`, Flexbox memberikan kontrol penuh atas layout halaman Anda.

---
## Terima Kasih Telah Membaca!

- Hak Cipta &copy; 2024 oleh `citr.UsDev`
- Ikuti saya di [instagram](https://www.instagram.com/citr.usdev/), [GitHub](https://github.com/lua99w)
- Materi Oleh [w3school.com](https://www.w3school.com)
---

**adios semangat YA😁😹😹**

