# video-frame-extractor
Alat web standalone untuk mengekstrak frame (JPG) dari video lokal Anda. Pemrosesan sepenuhnya offline di browser.

Program ini adalah alat berbasis web yang memungkinkan pengguna untuk mengekstrak frame gambar (JPG) dari file video lokal mereka. Semua pemrosesan terjadi secara *offline* di *browser* (mode *standalone*), yang berarti video Anda tidak pernah diunggah ke server.

Berikut adalah deskripsi program untuk GitHub:

# 🎞 Video Frame Extractor Pro | Alat Ekstraksi Frame Offline

Sebuah alat berbasis web yang kuat dan *standalone* (tidak memerlukan *server*) untuk mengekstrak frame gambar (JPG) dari file video. Semua pemrosesan dilakukan secara lokal di browser Anda, memastikan privasi dan pemrosesan *offline*.

## ✨ Fitur Utama

* **Pemrosesan *Offline* Penuh:** Semua proses ekstraksi frame dan konversi terjadi di sisi klien (*browser*), menjamin kecepatan, privasi, dan tidak ada biaya *bandwidth* server.
* **Kontrol Frame Individual:** Navigasi video *frame-by-frame* menggunakan tombol atau *slider* frame yang presisi.
* **Ekstrak Frame Tunggal:** Ekstrak dan *download* frame yang sedang dilihat saat itu juga.
* **Ekstraksi Batch Berdasarkan Interval:** Ekstrak frame secara otomatis pada interval yang ditentukan (misalnya, setiap 10 frame).
* **Ekstraksi Batch Berdasarkan Rentang:** Tentukan frame awal dan akhir, serta interval opsional, untuk mengekstrak frame dari segmen video spesifik.
* **Output ZIP:** Secara otomatis mengkompres semua frame yang diekstrak dalam mode *batch* ke dalam file ZIP untuk kemudahan *download*.
* **Informasi Video Detail:** Menampilkan informasi penting seperti nama file, durasi, perkiraan FPS, dan total frame video.
* **Estimasi Frame:** Perkiraan jumlah total frame yang akan diekstrak berdasarkan pengaturan *batch* yang dipilih.

## 🛠 Teknologi

Program ini dibangun murni menggunakan teknologi web *client-side* (sisi klien):

* **HTML5**
* **CSS**
* **Vanilla JavaScript** (untuk semua logika pemrosesan video dan UI)
* **[JSZip](https://stuk.github.io/jszip/)** (untuk kompresi file ZIP)
* **[FileSaver.js](https://github.com/eligrey/FileSaver.js/)** (untuk memulai *download* file)

## 🚀 Cara Menggunakan (Lokal)

1.  **Clone Repositori** atau *download* file `Video To JPG.html`.
2.  Buka file **`Video To JPG.html`** di browser modern Anda (Chrome, Firefox, Edge, dll.).
3.  Klik **"📂 Pilih Video"** dan unggah file video Anda.
4.  Video akan dimuat, dan informasi total frame akan ditampilkan.
5.  Gunakan **Kontrol Frame Individual** untuk menavigasi dan mengekstrak frame spesifik, atau pilih **Mode Ekstraksi** di **Batch Ekstrak** (Interval atau Rentang).
6.  Klik **"📸 Mulai Ekstrak Batch"** untuk memulai proses.
7.  Setelah selesai, klik **"📦 Download Semua (ZIP)"** untuk mendapatkan semua frame yang diekstrak.

## ⚠️ Catatan Kinerja

Karena semua pemrosesan (termasuk *seeking* video, menggambar ke *canvas*, dan konversi ke JPG) dilakukan di browser, kinerja dapat bervariasi:

* **Video Berdurasi Panjang/Resolusi Tinggi:** Proses ekstraksi *batch* mungkin memakan waktu signifikan dan membebani sumber daya CPU/Memori browser Anda.
* **Akurasi FPS:** Tingkat *frame rate* (FPS) video diperkirakan. Jika video memiliki FPS variabel atau jika browser kesulitan mendeteksi metadata, akurasi *seeking* frame mungkin sedikit berbeda, tetapi umumnya sangat akurat untuk tujuan ekstraksi gambar.
