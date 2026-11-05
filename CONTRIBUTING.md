# Panduan dan Aturan Kolaborasi (CONTRIBUTING.md)
## Proyek: Pengelolaan Dana per Peruntukan (Kelompok 7 — Baitulmal Tazkia)

Selamat datang di repositori dokumentasi **Kelompok 7 — Baitulmal Tazkia (Klaster Keuangan)**. Seluruh anggota tim yang akan berkontribusi dan melakukan push ke repositori ini **wajib mematuhi 3 aturan utama** berikut:

---

## 1. Aturan Branching: Setiap Orang Memiliki Branch Masing-Masing

Untuk menjaga keteraturan repositori dan menghindari bentrok pekerjaan (*merge conflict*), **setiap anggota tim bekerja di branch masing-masing sesuai perannya (jobdesk)**:

* **Dilarang keras melakukan commit atau push langsung ke branch `main`!**
* Setiap orang wajib membuat branch kerja sendiri saat menyusun atau merevisi dokumen:
  * **Business Analyst (BA)** memiliki branch tersendiri, contoh:  
    `docs/ba-stakeholder-register`, `docs/ba-srs-draft`, `docs/ba-rtm-matrix`
  * **Peran Lainnya (Architect, Technical Lead, QA/Reviewer)** juga memiliki branch tersendiri, contoh:  
    `docs/lead-project-charter`, `docs/tech-feasibility-study`, `docs/qa-test-plan`
* **Format Penamaan Branch**:
  `docs/<peran>-<nama-tugas-atau-dokumen>`
* **Penggabungan ke `main`**:
  Setelah dokumen di branch Anda selesai disusun, lakukan push ke remote branch Anda lalu ajukan **Pull Request (PR)** ke branch `main`. Anggota tim lain akan meninjau (review) sebelum di-merge ke branch `main`.

---

## 2. Standar Format Dokumen Harus Berbentuk File `.md` (Markdown)

Seluruh dokumentasi proyek (seperti Piagam Proyek, Stakeholder Register, SRS, RTM, Risk Register, Laporan Analisis, dsb.) **wajib berbentuk file berekstensi `.md` (Markdown)**.

### Ketentuan Format:
1. **Sebelum Diubah ke File `.md`**:
   * Pastikan draft naskah atau bahan tulisan (misalnya dari hasil wawancara, catatan riset, atau hasil olahan data) formatnya sudah rapi dan terstruktur (penomoran bab, subbab, poin daftar, dan tabel).
2. **Saat dan Setelah Diubah ke File `.md`**:
   * **Pastikan kembali filenya tidak merubah format penulisan sama sekali**.
   * Periksa apakah baris tabel Markdown tertutup rapi (`| Kolom 1 | Kolom 2 |`).
   * Periksa susunan heading hierarkis (`# Judul Utama`, `## Sub-bab`, `### Sub-bagian`) agar tidak melompat.
   * Periksa indentasi daftar bertingkat (bullet points / numbering) agar tidak berantakan atau menyatu dalam satu baris.
   * Gunakan fitur **Markdown Preview** di editor teks Anda (seperti di VS Code) sebelum melakukan commit untuk memastikan tampilan visual dokumen sudah persis sesuai yang diinginkan.
3. **Kerahasiaan Data (Zero Credentials)**:
   * Sesuai ketentuan pelindungan data pribadi (UU No. 27/2022), dilarang memasukkan password, data donatur pribadi riil, atau data rahasia lainnya ke dalam dokumen.

---

## 3. Aturan Clone dan Pull: Selalu ke/dari Branch `main`

Seluruh proses sinkronisasi repositori berpusat pada branch `main` sebagai acuan versi stabil:

### 3.1 Aturan Kloning (Clone)
* Siapa pun yang ingin meng-clone repositori ini **harus selalu meng-clone ke branch `main`**:
  ```bash
  git clone https://github.com/amandawjyanti/Pengelolaan-Dana-per-Peruntukan-.git
  cd Pengelolaan-Dana-per-Peruntukan-
  git checkout main
  ```

### 3.2 Aturan Menarik Pembaruan (Pull)
* Setiap kali sebelum mulai menulis dokumen baru atau sebelum membuat branch baru, anggota **wajib melakukan pull dari branch `main`** agar selalu mendapatkan versi dokumen paling mutakhir:
  ```bash
  # Pindah ke main dan tarik update terbaru
  git checkout main
  git pull origin main
  ```
* Saat sedang bekerja di branch kerja masing-masing dan ingin menyinkronkan dokumen terbaru yang sudah masuk ke `main`:
  ```bash
  git fetch origin main
  git merge origin/main
  ```

---

## 4. Ringkasan Alur Kerja Harian (Workflow)

```bash
# 1. Update branch main lokal
git checkout main
git pull origin main

# 2. Buat branch baru sesuai peran Anda
git checkout -b docs/ba-srs-kebutuhan

# 3. Buat / edit dokumen .md di folder docs/
# Pastikan formatting sudah rapi dan tidak ada format yang berubah

# 4. Simpan dan commit di branch Anda
git add docs/
git commit -m "docs(ba): tambah draf kebutuhan fungsional SRS"

# 5. Push ke remote branch Anda
git push -u origin docs/ba-srs-kebutuhan

# 6. Buka GitHub dan buat Pull Request (PR) ke branch main untuk direview oleh tim
```
