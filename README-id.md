# 🌐 Pilihan Bahasa / Language Options:
[English](README.md) | **Bahasa Indonesia**

---

# GRAD-System (Sistem Manajemen Data Kelulusan)

Sistem manajemen administrasi kelulusan dan yudisium berbasis web yang dibangun menggunakan **Framework Laravel**. Sistem ini dirancang untuk mengintegrasikan dan mempercepat alur verifikasi dokumen kelulusan secara *real-time* antara mahasiswa, bagian BAAK, dan berbagai departemen terkait.

## Ringkasan Proyek (Overview)

GRAD-System dirancang sebagai solusi digital terpadu untuk menggantikan proses birokrasi kelulusan konvensional di universitas yang sering kali memakan waktu. 

Sistem menyediakan dasbor kontrol khusus yang terbagi ke dalam multi-peran (*Multi-role Access Control*) dengan hak otorisasi yang ketat:
* **BAAK (Administrasi Akademik & Kemahasiswaan):** Selaku Super Admin pengawas ekosistem kelulusan.
* **Mahasiswa:** Mengajukan berkas dan memantau status validasi.
* **Staf Perpustakaan, Staf Keuangan, Staf CSDL, dan Staf Fakultas:** Bertindak sebagai tim verifikator dokumen internal sesuai bidang masing-masing.

Setiap peran beroperasi di dalam ruang lingkup kerja yang terisolasi, memastikan alur kerja verifikasi berjalan lebih cepat, terstruktur, transparan, dan aman.

---

# Fitur Utama

## Otorisasi & Autentikasi Multi-Peran
* Penyediaan dasbor kerja khusus yang disesuaikan untuk 6 hak akses berbeda.
* Pembatasan keamanan rute (*middleware*) berbasis peran pengguna.
* **Otomatisasi Akun:** Akun login mahasiswa digenerate secara massal dan otomatis oleh sistem saat data diimpor oleh BAAK.

## 📊 Manajemen Data Mahasiswa (Grup BAAK)
* Kemampuan impor dan ekspor data mahasiswa kelulusan dalam format spreadsheet secara instan.
* Sistem otomatis mengirimkan kredensial akun (*username* & *password*) langsung ke email pribadi mahasiswa begitu proses impor sukses (menggunakan *Email Automation*).

## 🎓 Manajemen Registrasi Kelulusan & Yudisium
Mahasiswa dapat melakukan pendaftaran kelulusan dan mengunggah dokumen persyaratan secara mandiri melalui sistem. 
* **Pelacakan Real-Time:** BAAK dapat memantau grafik kelulusan, penyelesaian dokumen, dan kemajuan persetujuan lintas divisi secara langsung.
* **Sistem Validasi Departemen:** Staf Perpustakaan, Keuangan, CSDL, dan Fakultas dapat langsung menyetujui dokumen atau memberikan catatan revisi jika berkas mahasiswa tidak memenuhi syarat. 
* Hak akses verifikasi terisolasi penuh; staf hanya dapat mengedit bagian validasi miliknya sendiri, sementara BAAK memegang kendali pengawasan seluruh status verifikasi.

## 🔔 Sistem Notifikasi Instan
Mahasiswa menerima pembaruan informasi secara instan pada dasbor mereka mengenai status kelulusan, persetujuan berkas, catatan revisi dari staf, hingga jadwal yudisium terbaru.

## 📄 Manajemen SKPI (Surat Keterangan Pendamping Ijazah)
* Mahasiswa dapat menginput prestasi dan mengunggah bukti dokumen SKPI langsung di sistem.
* BAAK memegang kendali peninjauan berkas, penyuntingan data cetak, pembuatan dokumen SKPI siap cetak, hingga penghapusan data.

## 📦 Pelacakan Distribusi Toga
Modul logistik digital untuk memantau status pengambilan toga. Sistem otomatis memvalidasi kelayakan pengambilan toga hanya bagi mahasiswa yang telah menyelesaikan seluruh rangkaian administrasi dan SKPI.

## 📣 Manajemen Informasi & Pengumuman
Fitur bagi BAAK untuk mempublikasikan berita yudisium resmi, mengunduh data visual grafik kelulusan, dan membagikan edaran penting kepada mahasiswa.

## ❓ Modul Manajemen Tanya Jawab (Q&A)
Menyediakan pusat bantuan interaktif *Frequently Asked Questions* (FAQ) di dalam sistem untuk menekan angka pertanyaan berulang dari mahasiswa kepada staf BAAK.

## 📝 Moderasi Testimoni Kelulusan
Mahasiswa dapat menuliskan ulasan (*feedback*) pengalaman kuliah mereka. Testimoni akan masuk ke antrean moderasi BAAK terlebih dahulu sebelum dipublikasikan secara resmi ke halaman publik.

## Dasbor Mahasiswa (Student Hub)
Pusat akses interaktif mandiri mahasiswa untuk mengajukan kelulusan, submit berkas SKPI, membaca pengumuman, mengubah profil, memantau riwayat verifikasi berkas, serta fitur pintas menghubungi BAAK via WhatsApp atau Email.

---

# Teknologi yang Digunakan

* **Framework Backend:** Laravel (PHP)
* **Pangkalan Data:** MySQL
* **Arsitektur Antarmuka:** Blade Template Engine, Bootstrap, JavaScript, HTML5 & CSS3

---

# Hak Akses & Tanggung Jawab Sistem

| Peran Pengguna | Tanggung Jawab Teknis |
| -------------- | ---------------------------------------------------- |
| BAAK           | Manajemen penuh ekosistem kelulusan, monitoring lintas divisi, moderasi data |
| Mahasiswa      | Registrasi yudisium, unggah dokumen, manajemen SKPI & profil pribadi |
| Staf Perpus    | Validasi bebas pinjam pustaka dan penyerahan tugas akhir |
| Staf Keuangan  | Validasi pelunasan tunggakan biaya kuliah & biaya wisuda |
| Staf CSDL      | Validasi pengisian tracer study / data pusat karir |
| Staf Fakultas  | Validasi kelayakan akademik dan administrasi tingkat fakultas |

---

# Sorotan Utama (Key Highlights)

* Menggunakan arsitektur dasbor multi-peran yang kompleks dan terintegrasi.
* Alur kerja verifikasi kelulusan terpusat (*Centralized Workflow*).
* Integrasi *Automated Email Delivery* untuk distribusi akun massal.
* Sistem pelacakan status dokumen interaktif secara *real-time*.
* Manajemen dokumen digital yang terstruktur tinggi.
* Desain antarmuka web responsif di berbagai ukuran perangkat.

---

# Tangkapan Layar (Screenshots)

## Halaman Autentikasi Gateway
![Halaman Login](screenshots/login-page.png)

## Dasbor Utama Super Admin BAAK
![Dasbor Admin](screenshots/admin-dashboard.png)

## Dasbor Interaktif Mahasiswa
![Dasbor Mahasiswa](screenshots/student-dashboard.png)

---

# Kontribusi Tim Pengembangan

- **Liana Syifa Fauzia:** Pengembang Utama Full-stack (Arsitektur backend, logika bisnis sistem, integrasi email, manajemen database, dan rekayasa frontend dasbor).
- **Ni'mas Subang Asih:** Pendukung Pengembangan (*Development Support*).
- **Hani Ayu Fadila:** Jaminan Kualitas (*Software Quality Assurance / Testing*) dan Umpan Balik Sistem.
- **Ririn Dwi Ariyanti:** Jaminan Kualitas (*Software Quality Assurance / Testing*) dan Analisis Pengguna.
- **Wulan Saputri:** Pengujian Sistem (*System Testing*) dan Penyusun Dokumentasi Kelayakan.
