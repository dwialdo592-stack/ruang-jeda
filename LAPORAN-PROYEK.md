# LAPORAN SINGKAT PROYEK — RUANG JEDA

## 1. Judul
**Ruang Jeda: Website Pendamping untuk Membentuk Kebiasaan Digital yang Lebih Seimbang**

## 2. Masalah
Penggunaan game dan media sosial secara berlebihan dapat membuat waktu untuk belajar, beristirahat, bergerak, dan berinteraksi langsung menjadi berkurang. Pengguna membutuhkan pengingat dan alternatif kegiatan yang sederhana.

## 3. Konsep solusi
Ruang Jeda menyediakan jurnal durasi penggunaan digital, indikator batas 5 jam, pengingat untuk beristirahat, saran kegiatan ketika website dibuka, checklist kegiatan non-digital, dan timer jeda singkat.

## 4. Fitur utama
- Pencatatan manual/simulasi durasi media sosial, video, game, dan aktivitas lain.
- Peringatan visual ketika total catatan mencapai 5 jam.
- Notifikasi browser jika pengguna telah memberi izin dan website aktif saat batas tercapai.
- Rekomendasi kegiatan yang tampil setiap kali halaman dibuka.
- Checklist lima kegiatan sederhana dan timer jeda satu menit.

## 5. Pemanfaatan AI
AI digunakan sebagai alat bantu untuk:
- Membantu menyusun ide solusi dan alur fitur berdasarkan masalah yang dipilih.
- Membantu membuat struktur HTML, CSS, dan JavaScript.
- Membantu menyusun desain responsif, teks motivasi, panduan GitHub Pages, dan skenario pengujian.

Hasil akhir tetap perlu diperiksa dan dipahami oleh pembuat proyek. Penggunaan AI tidak menggantikan pengujian langsung.

## 6. Pengujian dan pemeriksaan awal

Pemeriksaan yang dapat dilakukan pada berkas proyek:

| No. | Pemeriksaan | Hasil |
|---|---|---|
| 1 | Pemeriksaan sintaks JavaScript menggunakan Node.js | Lulus, tidak ditemukan kesalahan sintaks |
| 2 | Pemeriksaan format `manifest.json` | Lulus, JSON valid |
| 3 | Pemeriksaan elemen HTML yang dipanggil JavaScript | Lulus, ID elemen yang dirujuk tersedia |
| 4 | Pemeriksaan keberadaan logika batas 300 menit (5 jam), penyimpanan lokal, dan permintaan izin notifikasi | Lulus pemeriksaan kode |
| 5 | Uji browser langsung untuk notifikasi, tampilan perangkat, dan penyimpanan | Perlu dilakukan pada browser pengguna setelah website dijalankan melalui localhost atau GitHub Pages HTTPS |

### Skenario uji manual saat demonstrasi

1. Tambahkan 180 menit media sosial, 90 menit video, dan 30 menit game. Total harus menjadi 5 jam dan peringatan batas tampil.
2. Centang satu kegiatan. Penghitung kegiatan harus berubah dari `0/5` menjadi `1/5`.
3. Jalankan timer jeda. Hitung mundur dimulai dari `01:00`.
4. Muat ulang halaman pada hari yang sama. Catatan tetap tersimpan pada browser yang sama.
5. Izinkan notifikasi browser, lalu ulangi pencatatan hingga total 5 jam untuk menguji pemberitahuan.

## 7. Batasan dan pengembangan
Website ini tidak dapat membaca durasi penggunaan semua aplikasi lain, memantau aktivitas HP di latar belakang, atau mendeteksi setiap kali perangkat dibuka. Pencatatan masih manual/simulasi. Untuk pemantauan Android yang sebenarnya, pengembangan berikutnya harus berupa aplikasi native dengan izin sistem yang sesuai. Notifikasi web pada proyek ini memerlukan izin pengguna dan tidak dijamin berjalan setelah halaman ditutup.

## 8. Publikasi
- Repository GitHub: **[isi setelah membuat repository]**
- Website GitHub Pages: **[isi setelah GitHub Pages aktif]**
- Google Apps Script: **Tidak digunakan**. Website menggunakan HTML, CSS, JavaScript, dan penyimpanan lokal browser.

## 9. Kesimpulan
Ruang Jeda merupakan prototipe website interaktif yang membantu pengguna mengevaluasi waktu digital dan mencoba kegiatan alternatif. Website ini ditujukan sebagai alat bantu membangun kebiasaan, bukan alat diagnosis atau pemantauan otomatis seluruh perangkat.
