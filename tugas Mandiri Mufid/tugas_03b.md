# Tugas Mandiri 03b — Wireframe HTML/CSS/JS Hitam-Putih

Nama: [Abdullah Mufid A]

## 1. Kode HTML, CSS & JS :

```html
<!DOCTYPE html>
<html lang="id">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Wireframe Kartu Produk</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1>Daftar Produk</h1>

    <div class="daftar-produk">
      <!-- Kartu 1: Produk normal -->
      <article class="kartu">
        <div class="gambar">[ Gambar Produk ]</div>
        <h2 class="nama">Nama Produk A</h2>
        <p class="harga">Rp 150.000</p>
        <p class="status">Stok tersedia</p>
        <button class="tombol" id="btn-beli">Tambah ke Keranjang</button>
      </article>

      <!-- Kartu 2: Produk Stok Habis -->
      <article class="kartu kartu-habis">
        <div class="gambar">[ Gambar Produk ]</div>
        <h2 class="nama">Nama Produk B</h2>
        <p class="harga">Rp 200.000</p>
        <p class="status">Stok Habis</p>
        <button class="tombol" disabled>Stok Habis</button>
      </article>
    </div>

    <p id="info-keranjang">Keranjang: 0 item</p>

    <script src="script.js"></script>
  </body>
</html>
```

```CSS

* {
  box-sizing: border-box;
}

body {
  font-family: sans-serif;
  color: #000;
  background: #fff;
  padding: 24px;
}

.daftar-produk {
  display: flex;
  gap: 16px;
  flex-wrap: wrap;
}

.kartu {
  width: 240px;
  border: 2px solid #000;
  padding: 16px;
}

.gambar {
  border: 1px dashed #000;
  height: 140px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 12px;
}

.nama {
  font-size: 18px;
  margin: 0 0 8px;
}

.harga {
  font-weight: bold;
  margin: 0 0 4px;
}

.status {
  margin: 0 0 12px;
}

/* Tombol aktif */
.tombol {
  width: 100%;
  padding: 10px;
  font-family: sans-serif;
  font-size: 14px;
  border: 2px solid #000;
  background: #000;
  color: #fff;
  cursor: pointer;
}

.tombol:hover {
  background: #fff;
  color: #000;
}

/* Tombol nonaktif */
.tombol:disabled {
  background: #fff;
  color: #888;
  border: 2px dashed #888;
  cursor: not-allowed;
}

/* Kartu stok habis dibuat lebih pudar */
.kartu-habis {
  border-style: dashed;
  color: #666;
}

#info-keranjang {
  margin-top: 24px;
  border: 1px solid #000;
  padding: 8px 12px;
  display: inline-block;
}
```

```JavaScript

let jumlahKeranjang = 0;

const tombolBeli = document.getElementById("btn-beli");
const infoKeranjang = document.getElementById("info-keranjang");

tombolBeli.addEventListener("click", function () {
  jumlahKeranjang++;
  infoKeranjang.textContent = "Keranjang: " + jumlahKeranjang + " item";
});

// Tombol "Stok Habis" memakai atribut disabled,
// sehingga otomatis tidak bisa diklik dan tidak butuh event listener.
```

## 2. Refleksi Singkat:

## 2. Refleksi Singkat:

Dari tugas ini, saya belajar membuat tampilan daftar produk menggunakan HTML, CSS, dan JavaScript dengan desain hitam-putih.

Saya membuat dua kartu produk, yaitu produk yang stoknya tersedia dan produk yang stoknya habis. Tombol produk yang tersedia bisa diklik untuk menambahkan barang ke keranjang, sedangkan tombol produk yang stoknya habis tidak bisa diklik.

Saya juga belajar bahwa desain aplikasi harus sederhana, jelas, dan mudah digunakan agar pengguna tidak bingung saat menggunakannya.
