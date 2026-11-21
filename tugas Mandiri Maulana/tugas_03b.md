# Tugas Mandiri 03b — Wireframe HTML/CSS Hitam-Putih

# Nama: [Nama Lengkap Kamu]

# 1. Kode HTML & CSS

* Berikut adalah kode HTML dan CSS untuk membuat dua kartu produk sederhana dengan tampilan wireframe hitam-putih. Kartu pertama menampilkan produk dengan stok tersedia, sedangkan kartu kedua menampilkan produk dengan stok habis.

HTML
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wireframe Kartu Produk</title>

    <style>
        /* Pengaturan dasar halaman */
        body {
            font-family: sans-serif;
            background-color: white;
            color: black;
            margin: 20px;
            padding: 20px;
        }

        h1 {
            text-align: center;
        }

        /* Container kartu produk */
        .container {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        /* Desain kartu produk */
        .card {
            width: 250px;
            border: 2px solid black;
            padding: 15px;
            text-align: center;
        }

        /* Area gambar produk */
        .gambar {
            height: 120px;
            border: 1px solid black;
            display: flex;
            justify-content: center;
            align-items: center;
            margin-bottom: 15px;
        }

        /* Informasi produk */
        .harga {
            font-weight: bold;
        }

        .status {
            border: 1px solid black;
            padding: 8px;
            margin: 10px 0;
        }

        /* Tombol aktif */
        .btn-aktif {
            width: 100%;
            padding: 10px;
            background-color: black;
            color: white;
            border: 1px solid black;
            cursor: pointer;
            font-family: sans-serif;
        }

        /* Tombol nonaktif */
        .btn-disabled {
            width: 100%;
            padding: 10px;
            background-color: white;
            color: gray;
            border: 1px solid gray;
            cursor: not-allowed;
            font-family: sans-serif;
        }
    </style>
</head>

<body>

    <h1>Daftar Produk</h1>

    <div class="container">

        <!-- KARTU PRODUK 1: STOK TERSEDIA -->
        <div class="card">

            <div class="gambar">
                Gambar Produk 1
            </div>

            <h2>Kaos Polos</h2>

            <p class="harga">Rp75.000</p>

            <p>
                Kaos polos berbahan katun yang nyaman
                digunakan untuk aktivitas sehari-hari.
            </p>

            <div class="status">
                Stok Tersedia
            </div>

            <button class="btn-aktif">
                Tambah ke Keranjang
            </button>

        </div>


        <!-- KARTU PRODUK 2: STOK HABIS -->
        <div class="card">

            <div class="gambar">
                Gambar Produk 2
            </div>

            <h2>Hoodie Polos</h2>

            <p class="harga">Rp150.000</p>

            <p>
                Hoodie polos berbahan lembut dan nyaman
                digunakan untuk kegiatan sehari-hari.
            </p>

            <div class="status">
                Stok Habis
            </div>

            <button class="btn-disabled" disabled>
                Stok Habis
            </button>

        </div>

    </div>

</body>
</html>

# 2. Refleksi Singkat

* Setelah mengerjakan tugas ini, saya memahami bahwa rancangan wireframe dapat diubah menjadi tampilan nyata menggunakan HTML dan CSS.

* HTML berfungsi untuk membuat struktur halaman, seperti kartu produk, gambar, nama produk, harga, deskripsi, status stok, dan tombol. Sedangkan CSS digunakan untuk mengatur tampilan agar lebih rapi melalui border, padding, ukuran, warna, dan jenis font.

* Saya juga belajar membedakan dua kondisi produk, yaitu stok tersedia dan stok habis. Ketika stok tersedia, tombol dapat digunakan untuk menambahkan produk ke keranjang. Sebaliknya, ketika stok habis, tombol dibuat nonaktif menggunakan atribut disabled sehingga pengguna tidak dapat menekan tombol tersebut.

* Dari tugas ini, saya menjadi lebih memahami bagaimana HTML dan CSS bekerja sama dalam membangun tampilan antarmuka pengguna (UI). Hal ini menjadi bekal penting untuk mempelajari React pada Bulan 2.