# RUANG JEDA — Digital Wellbeing

Website sederhana bertema motivasi, tenang, dan minimalis untuk membantu pengguna mengenali kebiasaan digital serta membangun rutinitas di luar layar.

## Fitur yang dapat didemonstrasikan

- Ringkasan total durasi yang dicatat pada hari ini.
- Batas harian 5 jam dengan indikator progres dan peringatan visual ketika batas tercapai.
- Notifikasi browser setelah izin diberikan. Pada versi statis ini, notifikasi dipicu ketika website sedang aktif dan pencatatan membuat total mencapai 5 jam.
- Tambah durasi manual melalui formulir atau tombol cepat untuk media sosial, video, dan game.
- Checklist lima kegiatan non-digital.
- Saran kegiatan yang berubah setiap kali halaman dibuka.
- Timer jeda napas selama satu menit.
- Data demo disimpan di `localStorage` pada browser/perangkat pengguna dan direset otomatis saat tanggal berganti.
- Tampilan responsif untuk layar komputer dan ponsel serta cache offline dasar melalui service worker.

## Catatan teknis dan batasan

Ini adalah **website demonstrasi berbasis data simulasi/manual**, bukan aplikasi pemantau sistem operasi. Browser biasa tidak memberi website izin untuk membaca total penggunaan semua aplikasi, mendeteksi setiap kali HP dibuka, atau menjalankan pemantauan terus-menerus ketika tab ditutup. Pengingat browser juga bergantung pada izin pengguna, dukungan browser, dan kondisi halaman/perangkat.

Karena itu, durasi dimasukkan secara manual atau melalui tombol simulasi. Website menampilkan saran ketika website dibuka. Untuk pemantauan sungguhan lintas aplikasi Android dibutuhkan aplikasi Android native dengan izin Usage Access dan mekanisme background yang sesuai kebijakan Android; iOS memiliki batasan Screen Time/Family Controls tersendiri. Fitur tersebut berada di luar cakupan website statis ini.

## Cara menjalankan secara lokal

1. Unduh atau ekstrak folder proyek.
2. Buka `index.html` melalui browser untuk mencoba fitur utama. Beberapa fitur PWA/notifikasi memerlukan HTTPS atau localhost.
3. Untuk pengujian service worker, jalankan server lokal sederhana, misalnya `python -m http.server 8000`, lalu buka `http://localhost:8000` di folder proyek.

## Cara mengunggah ke GitHub dan menerbitkan dengan GitHub Pages

1. Masuk ke GitHub dan buat repository baru, misalnya `ruang-jeda`.
2. Unggah **semua isi folder proyek** ke root repository: `index.html`, `manifest.json`, `sw.js`, `icon.svg`, `README.md`, dan `LAPORAN-PROYEK.md`.
3. Buka **Settings → Pages** pada repository.
4. Pada **Build and deployment**, pilih **Deploy from a branch**.
5. Pilih branch `main` dan folder `/(root)`, lalu klik **Save**.
6. Tunggu proses publikasi GitHub Pages selesai. Tautan umumnya berbentuk `https://USERNAME.github.io/ruang-jeda/`.
7. Buka tautan menggunakan browser yang mendukung notifikasi. Izinkan notifikasi melalui tombol di bagian atas website.

> Tautan GitHub dan website baru akan tersedia setelah repository dibuat dan GitHub Pages diaktifkan pada akun pemilik. File proyek ini sudah disiapkan, tetapi belum dipublikasikan ke akun GitHub pengguna.

## Cara demonstrasi singkat

1. Buka website.
2. Klik tombol cepat **Media sosial +30 menit** beberapa kali atau pilih **Tambah catatan**.
3. Untuk memperlihatkan peringatan 5 jam dengan cepat, tambahkan durasi simulasi: `Media sosial` 180 menit, `Video` 90 menit, dan `Game` 30 menit. Total menjadi 300 menit sehingga peringatan batas muncul.
4. Izinkan notifikasi browser sebelum menguji notifikasi.
5. Centang beberapa kegiatan pada **Rencana hari ini** dan lihat penghitung kegiatan berubah.
6. Klik **Mulai jeda 1 menit** untuk mencoba timer.
7. Klik **Reset data simulasi** untuk mengembalikan kondisi awal.

## Teknologi

HTML, CSS, JavaScript murni, Web Notifications API, localStorage, Web App Manifest, dan Service Worker. Tidak menggunakan server, API key, akun, atau pengumpulan data pribadi. Tidak menggunakan Google Apps Script.
