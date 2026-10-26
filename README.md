# Vape Store Catalog Demo

Website katalog statis dari versi lokal `websitevape2`. Versi ini dipilih karena mencakup katalog, detail produk, keranjang, FAQ, halaman tentang, dan kontak. Berkas `home.html` dijadikan `index.html` agar halaman pembuka mudah ditemukan. Ini tidak memiliki backend, autentikasi, stok, atau pembayaran.

## Menjalankan

Gunakan server statis dari folder proyek:

```powershell
python -m http.server 8089 --bind 127.0.0.1
```

Buka `http://127.0.0.1:8089`. Tidak diperlukan Node.js atau instalasi dependency aplikasi. Aset CSS, font, JavaScript, dan gambar yang dirujuk halaman dipertahankan sebagai aset statis sumber.

## Halaman

`index.html` membuka halaman utama, `products.html` dan `produk.html` memuat katalog, `hexohm.html` memuat detail, `cart.html` memuat keranjang, sedangkan `about.html`, `faq.html`, dan `contact.html` menyediakan halaman informasi. Data contoh berada di `data.json`.

## Batas implementasi

Keranjang adalah demonstrasi di browser. Kontak pada ekspor memakai alamat contoh dan tidak terhubung ke layanan bisnis. Tidak ada janji pemesanan, pembayaran, atau pengiriman yang diproses. Sebagian struktur HTML berasal dari template lama; fungsi yang belum terhubung perlu dilengkapi sebelum digunakan sebagai toko.

## Verifikasi dan sumber

Referensi aset lokal diperiksa secara statis pada halaman yang diekspor. Pemeriksaan ini tidak menggantikan uji semua kontrol di browser. Sumber lain dalam keluarga vape tetap disimpan terpisah pada koleksi lokal dan tidak digabung tanpa pembandingan.

Riwayat Git `vape_store_ccit` tidak disertakan karena remote-nya menunjuk repo kopikuyweb yang berbeda aplikasi. Aset dan template pihak ketiga tetap mengikuti hak pemiliknya; lihat `NOTICE.md`. Tidak ada lisensi baru yang diberikan untuk merek, foto, atau font bawaan sumber.
