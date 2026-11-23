# AI Agent Administrasi Perkantoran Dinas Pemerintahan Daerah

Repository ini berisi rancangan **AI Agent untuk membantu pekerjaan administrasi perkantoran** saat magang di dinas pemerintahan daerah. Agent membantu pekerjaan rutin seperti pencatatan surat, penyusunan konsep surat, notulensi rapat, pengarsipan, agenda, dan laporan administrasi.

> **Batas penggunaan:** AI Agent adalah asisten administrasi, bukan pengambil keputusan atau pejabat penandatangan. Semua dokumen resmi wajib diperiksa dan disetujui pegawai berwenang sebelum digunakan atau dikirim. Jangan masukkan data pribadi, rahasia negara, dokumen internal terbatas, atau informasi sensitif ke layanan AI publik.

## 1. Identifikasi jobdesk dan aktivitas repetitif

| Jobdesk administrasi | Aktivitas repetitif | Bantuan AI Agent | Pemeriksaan manusia |
|---|---|---|---|
| Mengelola surat masuk | Membaca, mengelompokkan, mencatat tanggal/nomor/pengirim/perihal, membuat ringkasan | Ekstraksi metadata, klasifikasi awal, ringkasan, dan draf lembar disposisi | Cocokkan dengan surat asli; disposisi tetap oleh pejabat berwenang |
| Menyiapkan surat keluar | Membuat draf berdasarkan format dan data yang diberikan, memeriksa kelengkapan | Draf surat, pemeriksaan struktur, ejaan, dan daftar lampiran | Nomor surat, dasar hukum, isi, tujuan, tanda tangan, dan pengiriman disahkan pegawai |
| Notulensi rapat | Menyusun catatan rapat, keputusan, PIC, dan tenggat | Mengubah catatan/transkrip yang diizinkan menjadi notulen terstruktur | Peserta, keputusan, dan tenggat diverifikasi pimpinan/notulis |
| Pengarsipan dokumen | Menamai file, memberi kategori, membuat indeks dan daftar arsip | Rekomendasi nama file, metadata, kategori, dan indeks | Klasifikasi resmi, retensi, akses, dan pemusnahan mengikuti aturan instansi |
| Mengelola agenda | Menyalin jadwal rapat/kegiatan, membuat pengingat dan daftar persiapan | Menyusun agenda harian/mingguan dan checklist | Konfirmasi jadwal, undangan, dan perubahan dilakukan petugas |
| Membuat laporan administrasi | Menghitung rekap surat/kegiatan dan menyusun narasi laporan | Merapikan data yang diberikan menjadi tabel dan draf laporan | Angka, sumber data, dan laporan final divalidasi penanggung jawab |

## 2. Tujuan dan alur kerja agent

**Nama:** Asisten Administrasi Dinas (AAD)

**Tujuan:** Mengurangi waktu untuk pengetikan, pengelompokan, peringkasan, dan penyusunan draf administrasi.

**Alur umum:**
1. Pegawai memberikan instruksi dan data yang memang boleh diproses.
2. Agent mengidentifikasi jenis pekerjaan dan memilih skill yang sesuai.
3. Agent menghasilkan draf/rekap dengan menandai bagian yang belum diketahui.
4. Pegawai memeriksa hasil dengan dokumen sumber.
5. Pegawai berwenang menyetujui, menandatangani, menyimpan, atau mengirim dokumen.

## 3. Daftar AI Agent Skills

Setiap folder skill berisi `SKILL.md` dengan instruksi kapan skill digunakan, masukan, langkah kerja, format keluaran, dan batasan.

- `skills/surat-masuk/` — pencatatan, klasifikasi awal, ringkasan surat masuk.
- `skills/surat-keluar/` — penyusunan draf surat keluar.
- `skills/notulensi-rapat/` — notulen dan daftar tindak lanjut.
- `skills/pengelolaan-arsip/` — penamaan, metadata, dan indeks arsip.
- `skills/agenda-kegiatan/` — agenda dan checklist kegiatan.
- `skills/laporan-administrasi/` — rekap dan draf laporan.

## 4. Contoh prompt penggunaan

**Surat masuk**
> Bantu catat surat berikut. Ambil tanggal, nomor, pengirim, perihal, kategori awal, ringkasan, dan tindak lanjut yang disarankan. Jika data tidak ada, tulis "Belum tercantum". Jangan membuat nomor surat atau disposisi.

**Surat keluar**
> Buat draf surat undangan berdasarkan informasi yang saya berikan. Gunakan bahasa dinas yang sopan. Tandai data yang belum tersedia dengan `[PERLU DIISI]`. Jangan mengarang dasar hukum atau nomor surat.

**Notulensi**
> Susun catatan rapat berikut menjadi notulen, keputusan, daftar tugas, PIC, dan tenggat. Jangan menambahkan keputusan yang tidak disebutkan.

## 5. Cara menggunakan

1. Buka folder skill yang sesuai.
2. Baca `SKILL.md`.
3. Salin instruksi skill ke konfigurasi AI Agent/platform yang digunakan, atau unggah file skill jika platform mendukung Agent Skills.
4. Berikan data yang sudah disamarkan dan diizinkan untuk diproses.
5. Periksa seluruh hasil sebelum menjadi dokumen resmi.

## 6. Prinsip keamanan dan tata kelola

- Terapkan prinsip **data minimum**: hanya berikan informasi yang benar-benar diperlukan.
- Samarkan nama, NIK, alamat, nomor telepon, tanda tangan, nomor rekening, dan data pribadi lainnya.
- Jangan unggah dokumen rahasia, data kepegawaian sensitif, data warga, atau dokumen berklasifikasi ke AI publik tanpa persetujuan dan pengamanan resmi.
- AI tidak boleh menetapkan disposisi, memberi persetujuan, menandatangani, mengirim surat resmi, mengubah arsip, atau memutuskan hak/layanan masyarakat secara otomatis.
- Jangan mengarang nomor surat, tanggal, dasar hukum, nama pejabat, keputusan rapat, atau data statistik.
- Simpan jejak pemeriksaan dan gunakan prosedur kearsipan serta kebijakan keamanan informasi instansi.

## 7. Struktur repository

```text
ai-agent-administrasi-dinas/
├── README.md
├── JOBDESK.md
├── .gitignore
└── skills/
    ├── surat-masuk/SKILL.md
    ├── surat-keluar/SKILL.md
    ├── notulensi-rapat/SKILL.md
    ├── pengelolaan-arsip/SKILL.md
    ├── agenda-kegiatan/SKILL.md
    └── laporan-administrasi/SKILL.md
```

## 8. Catatan

Ini adalah prototipe tugas pembelajaran. Penerapan nyata harus menyesuaikan SOP, klasifikasi keamanan informasi, tata naskah dinas, jadwal retensi arsip, dan kebijakan teknologi informasi pemerintah daerah terkait.
