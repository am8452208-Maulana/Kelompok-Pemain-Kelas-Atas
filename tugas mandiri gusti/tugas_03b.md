# Tugas Mandiri 03b — Wireframe HTML/CSS Hitam-Putih
Nama: Gusti Dimas Achmad

## 1. Kode HTML & CSS:
```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wireframe Kartu Produk</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Kartu Produk</h1>

    <div class="container">
        <div class="card">
            <div class="gambar">Gambar Produk</div>
            <h3>Produk 1</h3>
            <p>Deskripsi produk sederhana.</p>
            <p>Harga: Rp50.000</p>
            <button class="aktif">Beli Sekarang</button>
        </div>

        <div class="card">
            <div class="gambar">Gambar Produk</div>
            <h3>Produk 2</h3>
            <p>Deskripsi produk sederhana.</p>
            <p>Harga: Rp75.000</p>
            <p class="stok">Stok Habis</p>
            <button disabled>Stok Habis</button>
        </div>
    </div>
</body>
</html>
```
```css
body {
    font-family: sans-serif;
    background-color: white;
    color: black;
    padding: 20px;
}
.container {
    display: flex;
    gap: 20px;
}
.card {
    border: 1px solid black;
    padding: 15px;
    width: 200px;
}
.gambar {
    border: 1px solid black;
    height: 120px;
    display: flex;
    justify-content: center;
    align-items: center;
}
.button {
    padding: 10px;
    width: 100%;
    border: 1px solid black;
}
.aktif {
    background-color: black;
    color: white;
    cursor: pointer;
}
.button:disabled {
    background-color: white;
    color: gray;
    border: 1px solid gray;
    cursor: not-allowed;
}
.stok {
    border: 1px solid black;
    padding: 5px;
    text-align: center;
}
```
## 2. Refleksi Singkat:
Mengubah wireframe menjadi HTML/CSS hitam-putih membantu saya melihat struktur komponen secara nyata—termasuk cara membedakan tampilan tombol saat stok masih ada vs saat stok habis untuk persiapan React di Bulan 2.