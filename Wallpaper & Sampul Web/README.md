Japanese Project — Wallpaper & Sampul Web

Dokumentasi gambar latar belakang dan sampul untuk Web Admin FreeFireServer.

📁 Lokasi File

FreeFireServer/
├── admin_panel.py
└── static/
    ├── wallpaper.jpg
    └── cover.jpg

🖼️ Wallpaper Web

File: "static/wallpaper.jpg"

Wallpaper digunakan sebagai gambar latar belakang utama halaman Web Admin. Gambar ditampilkan memenuhi area browser dengan lapisan gelap agar teks dan komponen panel tetap mudah dibaca.

🎴 Sampul Web

File: "static/cover.jpg"

Sampul digunakan sebagai latar belakang bagian banner atau hero pada halaman dashboard, sesuai selector CSS yang diterapkan di "admin_panel.py".

⚙️ Konfigurasi CSS

Pengaturan gambar berada di dalam "admin_panel.py", pada bagian CSS bertanda "HANZIHAN_PANEL_IMAGES_V1".

- Wallpaper: "/static/wallpaper.jpg"
- Sampul: "/static/cover.jpg"
- Wallpaper: posisi tengah, ukuran cover, dengan lapisan gelap.
- Sampul: ukuran cover dengan posisi gambar yang disesuaikan.
- Responsif: pengaturan tampilan khusus untuk layar HP.

🔄 Cara Mengganti Gambar

1. Siapkan gambar wallpaper dan sampul baru.
2. Salin gambar ke folder "static/".
3. Gunakan nama file yang sama agar konfigurasi CSS tetap berfungsi.

Contoh perintah Termux:

cd ~/FreeFireServer || exit 1

cp "/storage/emulated/0/Download/Wallpaper Panel.jpg" \
   static/wallpaper.jpg

cp "/storage/emulated/0/Download/Sampul Panel.jpg" \
   static/cover.jpg

Penting: Perintah di atas mengganti gambar yang ada. Buat salinan cadangan terlebih dahulu jika ingin mempertahankan gambar sebelumnya.

▶️ Menjalankan Web Admin

cd ~/FreeFireServer || exit 1
python admin_panel.py

Kemudian buka:

"http://127.0.0.1:5055/login"

Jika panel sudah berjalan, muat ulang browser setelah mengganti gambar.

🛡️ Catatan

- Dokumentasi ini hanya membahas aset visual Web Admin.
- Mengganti wallpaper atau sampul tidak memerlukan perubahan database pemain.
- Jangan menghapus "wallpaper.jpg" atau "cover.jpg" jika CSS masih menggunakannya.
- Gunakan gambar yang kamu miliki atau memiliki izin untuk digunakan.

---

Japanese Project
FreeFireServer Web Admin — Wallpaper & Cover Documentation
