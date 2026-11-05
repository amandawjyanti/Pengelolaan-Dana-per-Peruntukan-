# Dokumentasi Proyek: Pengelolaan Dana per Peruntukan
### Kelompok 7 — Klaster Keuangan | Baitulmal Tazkia
**Program Studi Sistem Informasi — STMIK Tazkia (Tahun Akademik Gasal 2026/2027)**  
*Mata Kuliah: MISI.302, MISI.303, MISI.304, MISI.305*

---

## 📌 Ringkasan Informasi Proyek (Sementara)

Repositori ini difokuskan sebagai **pusat dokumentasi proyek** bagi Kelompok 7 dalam menganalisis dan merancang kebutuhan sistem **Pengelolaan Dana per Peruntukan** untuk Baitulmal Tazkia.

### Latar Belakang & Masalah
Baitulmal Tazkia mengelola penghimpunan dan penyaluran dana ZISWAF (Zakat, Infak, Sedekah, dan Wakaf). Saat ini, sistem operasional pengelolaan dana masih menghadapi tantangan:
* **Pencatatan Manual**: Pembukuan peruntukan dana masih dilakukan menggunakan *spreadsheet*.
* **Pemisahan Dana ZISWAF**: Dana zakat (khusus 8 asnaf), infak, sedekah, dan kampanye terikat tidak boleh tercampur. Kesalahan pencatatan manual berisiko melanggar ketentuan syariah.
* **Konfirmasi Saldo Sebelum Penyaluran**: Masih mengandalkan percakapan grup chat, sehingga verifikasi ketersediaan dana membutuhkan waktu dan rentan keliru.
* **Perhitungan Hak Amil**: Hak operasional amil perlu dihitung dan dipisahkan secara transparan sejak dana diterima.

### Tujuan Proyek
1. Mendokumentasikan analisis proses bisnis dan tata kelola dana peruntukan saat ini serta usulan perbaikannya.
2. Menyusun spesifikasi kebutuhan sistem (*Software Requirements Specification* - SRS) dan matriks keterlacakan kebutuhan (*Requirements Traceability Matrix* - RTM).
3. Mengidentifikasi pemangku kepentingan (*stakeholder*), analisis risiko, dan studi kelayakan.
4. Menjadi dokumen acuan resmi bagi tim pengembang (*developer*) sebelum tahap pembuatan aplikasi dimulai.

---

## 📁 Struktur Folder Repositori (Fokus Dokumen)

Saat ini repositori hanya memuat dokumen proyek. Folder dan konfigurasi teknis untuk *developer* akan dibuat langsung oleh tim pengembang saat fase pemrograman/konstruksi dimulai:

```text
Pengelolaan-Dana-per-Peruntukan/
├── docs/             # Berisi seluruh dokumen proyek berformat Markdown (.md)
│                     # (Piagam Proyek, Stakeholder Register, SRS, RTM, Risk Register, dsb.)
├── CONTRIBUTING.md   # Aturan resmi kolaborasi Git, pembuatan branch, dan format .md
└── README.md         # Ringkasan informasi umum proyek
```

---

## 👥 Tim & Pembagian Tugas (Jobdesk)
Dokumen-dokumen di dalam folder `docs/` akan disusun secara bertahap oleh anggota tim sesuai perannya:
* **Business Analyst (BA)**: Memimpin elisitasi kebutuhan, analisis situasi berjalan, serta penyusunan draf SRS dan RTM.
* **System Architect / Technical Lead**: Menyusun analisis perancangan arsitektur, spesifikasi antarmuka, dan dokumen teknis perancangan.
* **Anggota Tim Lainnya**: Melengkapi stakeholder register, risk register, studi kelayakan, dan persiapan skenario pengujian.

---

## 📖 Panduan Kolaborasi
Seluruh anggota tim yang akan membuat atau memperbarui dokumen diwajibkan membaca aturan kolaborasi pada file:  
👉 **[CONTRIBUTING.md](CONTRIBUTING.md)** (Memuat aturan branch masing-masing peran, standar penulisan file `.md`, serta alur clone dan pull dari branch `main`).
