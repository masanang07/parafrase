# Deteksi & Parafrase AI

Aplikasi web ringan berbasis browser (100% statis, tanpa server & tanpa API berbayar) untuk mendeteksi pola tulisan AI serta memparafrase teks **per kalimat** maupun **per paragraf**.

## Fitur Utama
- **Upload File Langsung di Browser**: Mendukung format `.pdf`, `.docx`, `.txt`, `.md`, dan `.csv` (diproses lokal menggunakan `pdf.js` dan `mammoth.js`).
- **Deteksi Pola AI Gratis**: Menganalisis *burstiness* (variasi panjang kalimat), keragaman kosakata (*lexical diversity*), serta mendeteksi frasa transisi klise yang umum dihasilkan AI.
- **Parafrase Granular (Per Kalimat / Per Paragraf)**: Pecah dokumen menjadi unit kalimat atau paragraf, parafrase bagian tertentu saja atau sekaligus, edit manual, lalu unduh hasilnya ke `.txt`.
- **Zero Setup & Siap GitHub Pages**: Cukup satu file `index.html` tanpa perlu instalasi *backend* atau konfigurasi *environment*.
- **Opsional BYOK**: Tetap menyediakan opsi penggunaan *Gemini API Key* pribadi melalui `localStorage` browser (opsional, secara default berjalan 100% lokal).

## Cara Menjalankan
1. **Lokal**: Unduh atau *clone* repositori ini, lalu buka `index.html` langsung di browser.
2. **GitHub Pages**:
   - Buka **Settings** > **Pages** pada repositori ini.
   - Pada bagian **Build and deployment**, pilih **Deploy from a branch**.
   - Pilih branch `main` dan folder `/ (root)`, lalu klik **Save**.

## Catatan
Hasil deteksi merupakan estimasi probabilistik berbasis pola linguistik dan tidak dimaksudkan sebagai vonis mutlak. Seluruh proses pembacaan file berjalan sepenuhnya di sisi klien (*browser*) pengguna.