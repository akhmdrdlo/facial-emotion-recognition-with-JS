# Deteksi Emosi Secara Real-Time

Aplikasi berbasis web ini dirancang untuk mendeteksi emosi dari video atau gambar menggunakan **face-api.js**. Aplikasi ini memanfaatkan model deep learning yang telah dilatih sebelumnya untuk menganalisis ekspresi wajah dan mengklasifikasikannya ke dalam emosi seperti **senang**, **sedih**, **terkejut**, **marah**, dan lainnya.

![Screenshot 2025-04-23 182230](https://github.com/user-attachments/assets/adad1070-dcb7-48f8-af59-052321deb632)

## Fitur

- **Deteksi Emosi Real-Time**: Mendeteksi emosi langsung dari kamera webcam.
- **Beragam Emosi**: Menampilkan emosi dengan tingkat kepercayaan tertinggi dan menambahkan overlay wajah yang terdeteksi pada video.
- **Penanganan Kesalahan**: Memberikan pesan peringatan jika kamera tidak tersedia atau akses ditolak.

## Teknologi yang Digunakan

- **HTML5**: Untuk struktur halaman web.
- **CSS3**: Untuk desain tampilan aplikasi.
- **JavaScript**: Untuk pengelolaan video dan logika deteksi emosi.
- **face-api.js**: Library untuk deteksi wajah dan pengenalan emosi berbasis deep learning.

## Panduan Instalasi

### 1. Kloning Repositori

```bash
git clone https://github.com/BaseMax/face-emotion-detection-web-live.git
cd face-emotion-detection-web-live
```

### 2. Pasang Server Web Lokal

Untuk menjalankan aplikasi ini secara lokal, Anda memerlukan server web lokal.

**Menggunakan http-server (via npm):**

Jika Anda sudah menginstal Node.js, gunakan http-server untuk menjalankan aplikasi.

```bash
npm install -g http-server
http-server .
```

### 3. Unduh Model

Aplikasi ini menggunakan model yang telah dilatih dari `face-api.js`. Anda perlu mengunduh model-model ini dan meletakkannya di folder `models` di direktori utama proyek.

Kunjungi direktori model face-api.js.

Unduh model berikut:
- ssdMobilenetv1
- faceLandmark68Net
- faceRecognitionNet (opsional)
- ageGenderNet (opsional)
- faceExpressionNet

Setelah mengunduh model dari direktori `/weights` (https://github.com/justadudewhohacks/face-api.js), letakkan di folder `/models` dalam direktori proyek Anda.

### 4. Jalankan Aplikasi

Setelah model tersedia dan server berjalan, buka browser Anda dan akses:

```bash
http://localhost:8080
```

Anda dapat mengunggah gambar dan melihat emosi yang terdeteksi dari wajah.

## Cara Kerja

- Pengguna mengunggah gambar melalui input file.
- Gambar diproses menggunakan library `face-api.js`.
- Library mendeteksi wajah, memproses landmark wajah, dan menganalisis emosi.
- Emosi dengan tingkat kepercayaan tertinggi akan ditampilkan.

## Deteksi Emosi

Aplikasi ini dapat mendeteksi emosi berikut:

- Senang
- Sedih
- Terkejut
- Marah
- Jijik
- Takut

### Kontribusi

Jika Anda ingin berkontribusi pada proyek ini, silakan fork repositori, buat branch baru, dan kirimkan pull request. Langkah-langkahnya adalah:

- Fork repositori.
- Buat branch baru.
- Lakukan perubahan.
- Kirimkan pull request.


