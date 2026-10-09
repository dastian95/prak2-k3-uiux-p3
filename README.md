# Kelompok 3 - Desain UI/UX Pemrograman Web
## Anggota
| Nama | NIM | Peminatan |
|---|---|---|
| Arga Uzumaki Dwiyan | 0110226086 | Artificial Intelligence |
| Arkan Zahran Ramadhan | 0110226139 | Cyber Security |
| Asyifa Fauziah | 0110226132 | Cyber Security |
| Aufa Dzaky Zuhdi Wicaksono | 0110226021 | Cyber Security |
| Christian Soya Niron | 0110226118 | Cyber Security |

## Penjelasan Setiap Bagian

```
prak2_uiux.html     halaman utama
assets/style.css    gaya halaman
assets/img/         logo dan foto anggota (PNG)
```

### prak2_uiux.html

- **Header** - judul kampus dan prodi, tampil sebagai topbar.
- **Main** - berisi logo, judul "Kelompok 3", dan kotak Intro.
- **Members** - pembungkus lima kartu anggota.
- **Card** - satu kartu per anggota: foto, nama, label "Anggota", daftar data (NIM, Prodi, Hobi, Kelas, Peminatan), dan motto.
- **Footer** - hak cipta dan nama kampus.
- Tautan CSS diberi nomor versi supaya browser selalu memuat CSS terbaru.

### style.css

- **Dasar** - font, warna latar, dan `.container` sebagai kotak putih selebar maksimal 1200px.
- **Topbar** - header memakai `position: sticky`, jadi menempel di atas saat halaman di-scroll.
- **Kartu** - memakai CSS Grid: foto di kolom kiri, teks di kolom kanan.
- **Daftar data** - memakai Flexbox, sehingga kelima data berjajar dalam satu baris dan turun ke baris berikutnya kalau tidak muat.
- **Layar kecil** - kartu berjajar ke samping dan digeser dengan `scroll-snap`. Khusus HP (lebar ≤ 600px), isi kartu bertumpuk: foto di atas, data di bawah.
- **Layar besar** - aturan `@media` di bagian paling bawah memadatkan semuanya supaya muat satu layar. Tinggi halaman dipatok setinggi layar, dan kelima kartu membagi sisa tinggi secara merata.