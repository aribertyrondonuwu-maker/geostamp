# GeoStamp KNMP 2027 – FPIK UNSRAT

Aplikasi kamera untuk foto dokumentasi berkoordinat (geotagging) pada kegiatan Survei, Verifikasi, Penilaian, dan Fasilitasi Kesiapan Calon Lokasi KNMP 2027. Bisa dipakai di Android dan iPhone.

Setiap foto diberi stempel berisi:
- jenis foto
- desa/kelurahan, kecamatan, kabupaten/kota, dan kode lokasi
- tanggal, jam, dan zona waktu
- koordinat GPS beserta akurasinya
- tahap kegiatan, nama surveyor, dan keterangan
- peta mini

Koordinat dan waktu juga ditulis ke metadata EXIF, sehingga bisa dicocokkan dengan titik KoBoCollect.

Daftar 32 lokasi, surveyor, dan koordinator wilayah diambil dari Tabel 1 dan Tabel 4 Laporan Pendahuluan. Ada juga pilihan "Lainnya" untuk kegiatan di luar 32 lokasi, seperti pembekalan atau rapat.

## Memasang di GitHub Pages
1. Unggah semua file di folder ini ke root repositori `geostamp`: Add file → Upload files → Commit.
2. Buka Settings → Pages → Deploy from a branch → `main` / root → Save.
3. Aplikasi aktif di `https://aribertyrondonuwu-maker.github.io/geostamp/`.

## Untuk surveyor (bagikan bagian ini)
1. **Sebelum berangkat, saat masih ada sinyal:** buka tautan aplikasi di HP.
   - Android/Chrome: menu ⋮ → *Instal aplikasi*.
   - iPhone/Safari: Bagikan → *Tambahkan ke Layar Utama*.
   - Izinkan akses **Kamera** dan **Lokasi**. Langkah ini juga menyimpan aplikasi agar bisa dipakai offline.
2. Ketuk **✎**, lalu pilih **lokasi penugasan** Anda. Nama surveyor terisi otomatis.
3. Di layar kamera, pilih **tahap kegiatan** dan **jenis foto**. Isi keterangan bila perlu melalui ✎.
4. Tunggu titik GPS berwarna **hijau** (±20 m atau lebih baik), lalu ambil foto.
5. Simpan foto ke galeri HP lewat **Bagikan → Simpan Gambar**, agar bisa dilampirkan di pertanyaan foto KoBoCollect.
6. Di akhir hari, buka **Galeri**, pilih lokasi, lalu tekan **ZIP**. Unggah file ZIP ke penyimpanan daring bersama tim.

## Hasil ekspor
- **ZIP** dengan struktur `KNMP_07_BMS_Dudepo_Barat/Batas_lahan/KNMP_07_BMS_Dudepo_Barat_Batas_lahan_20261110_093015.jpg`. Di dalamnya juga ada `rekap_foto.csv`, `titik_foto.kml`, dan `data.json`.
- **Laporan**: halaman HTML berisi foto, dikelompokkan per lokasi. Buka → Cetak → Simpan sebagai PDF.
- **Excel (CSV)**: rekap per foto berisi kode, kabupaten, kecamatan, desa, tahap, jenis, waktu, koordinat, akurasi, surveyor, koordinator, dan nama file.
- **KML**: titik foto untuk Google Earth atau Google My Maps.

## Catatan
- Foto tersimpan di penyimpanan browser HP. **Ekspor dan unggah setiap hari.**
- Tanpa sinyal, kamera, GPS, dan stempel tetap berfungsi. Peta mini hanya muncul untuk area yang pernah dibuka saat ada internet.
- Aplikasi akan memperingatkan jika GPS belum terkunci atau akurasinya rendah.
- GeoStamp adalah pelengkap KoBoCollect. Titik koordinat resmi tetap diisi di KoBoCollect.
