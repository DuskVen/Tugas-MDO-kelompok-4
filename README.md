# Digital Marketing Agency AI Agent — Praktikum #13

Repository ini berisi kumpulan **AI Agent Skills** untuk membantu pekerjaan repetitif pada digital marketing agency. Fokusnya adalah mempercepat proses produksi konten dan pelaporan, bukan menggantikan keputusan strategis maupun persetujuan klien.

## 1. Tujuan proyek

Membangun asisten operasional yang dapat menerima brief klien, menyusun ide dan kalender konten, membuat draft caption, menyiapkan kerangka artikel SEO, serta merangkum performa kampanye berdasarkan data yang diberikan.

## 2. Jobdesk dan aktivitas repetitif

| Jobdesk | Aktivitas repetitif | Bantuan AI Agent | Keputusan manusia |
|---|---|---|---|
| Account / Client Service | Merapikan brief, mencatat tujuan, audiens, kanal, dan deadline | Mengubah brief bebas menjadi brief terstruktur dan menandai data yang belum ada | Mengonfirmasi brief dengan klien |
| Social Media Specialist | Mencari ide konten, membuat variasi caption dan CTA | Menghasilkan ide, caption, hashtag, dan variasi format | Memilih ide dan menyetujui pesan/brand voice |
| Content Planner | Menyusun kalender konten dan mengisi slot publikasi | Membuat draft kalender sesuai frekuensi dan pilar konten | Menentukan prioritas, tanggal final, dan jadwal aktual |
| Copywriter / Content Writer | Membuat outline artikel, meta title, meta description, dan draft awal | Menyusun outline dan draft SEO berdasarkan keyword dan sumber | Memeriksa fakta, orisinalitas, klaim, dan kualitas editorial |
| Digital Ads Specialist | Merangkum metrik kampanye dan membandingkan periode | Menghitung metrik sederhana dan membuat ringkasan insight dari data yang tersedia | Menentukan perubahan anggaran, targeting, dan strategi iklan |
| Marketing Analyst | Membuat laporan rutin dan menulis rekomendasi awal | Menyusun laporan terstruktur serta menandai anomali/data yang kurang | Memvalidasi analisis dan menyetujui tindakan |

**Batas otomasi:** AI menghasilkan *draft* dan rekomendasi. Publikasi konten, pengiriman pesan ke klien, perubahan anggaran iklan, dan keputusan komersial harus melalui persetujuan manusia.

## 3. Struktur repository

```text
digital-marketing-agency-ai-agent/
├── README.md
├── AGENT_WORKFLOW.md
├── JOBDESK_ANALYSIS.md
├── RESPONSIBLE_USE.md
├── skills/
│   ├── brief-intake/SKILL.md
│   ├── content-ideation/SKILL.md
│   ├── social-caption/SKILL.md
│   ├── content-calendar/SKILL.md
│   ├── seo-content/SKILL.md
│   └── campaign-report/SKILL.md
├── templates/
│   ├── client-brief.md
│   ├── content-calendar.csv
│   └── campaign-report-input.csv
└── examples/
    ├── sample-client-brief.md
    └── sample-agent-output.md
```

## 4. Cara menggunakan skills

Folder `skills/` menggunakan format **Agent Skills**: setiap skill memiliki file `SKILL.md` dengan metadata YAML (`name`, `description`) dan instruksi kerja.

1. Buka platform/agent yang mendukung format Agent Skills.
2. Impor atau salin folder skill yang dibutuhkan sesuai petunjuk platform tersebut.
3. Berikan brief atau data klien yang relevan.
4. Minta agent menjalankan skill yang sesuai, misalnya: “Gunakan skill social-caption untuk membuat 3 caption Instagram dari brief ini.”
5. Periksa hasil, lalu lakukan revisi dan persetujuan manusia sebelum dipublikasikan.

Skills ini bersifat portabel sebagai instruksi. Dukungan impor langsung dapat berbeda antarplatform.

## 5. Contoh alur kerja

1. Account Executive memasukkan brief klien.
2. `brief-intake` merapikan brief dan mengidentifikasi informasi yang belum tersedia.
3. `content-ideation` membuat ide berdasarkan tujuan, audiens, dan pilar konten.
4. `content-calendar` mengatur ide ke dalam kalender draft.
5. `social-caption` menulis caption untuk konten terpilih.
6. `seo-content` membantu artikel pendukung jika dibutuhkan.
7. Setelah kampanye berjalan, `campaign-report` merangkum data performa yang diberikan.

Detail alur: [`AGENT_WORKFLOW.md`](AGENT_WORKFLOW.md).

## 6. Contoh prompt penggunaan

> Anda adalah AI Agent untuk digital marketing agency. Gunakan skill brief-intake untuk mengubah informasi klien di bawah menjadi brief terstruktur. Jangan mengarang informasi yang belum diberikan; tandai sebagai “Perlu konfirmasi”.

> Gunakan skill content-ideation. Buat 10 ide konten Instagram untuk audiens dan tujuan dalam brief. Sertakan pilar konten, format, angle, dan CTA.

> Gunakan skill campaign-report untuk menganalisis CSV performa kampanye. Hitung metrik hanya jika kolom yang dibutuhkan tersedia. Pisahkan fakta data, interpretasi, dan rekomendasi.

## 7. Catatan dan keterbatasan

- Output AI adalah draft, bukan persetujuan final.
- Jangan memasukkan password, token, data pribadi sensitif, atau data pelanggan yang tidak diperlukan.
- Jangan mengarang statistik, testimoni, hasil kampanye, sumber, maupun klaim produk.
- Untuk laporan, agent hanya boleh menyimpulkan berdasarkan data yang benar-benar diberikan.
- Penggunaan AI tidak menjamin peningkatan engagement, penjualan, atau ranking SEO.

## 8. Checklist sebelum dikumpulkan

- [ ] Repository memiliki nama dan deskripsi yang jelas.
- [ ] Semua folder dan file pada struktur di atas sudah terunggah.
- [ ] Visibilitas repository diatur menjadi **Public**.
- [ ] README dapat dibaca dan menjelaskan tujuan serta cara penggunaan.
- [ ] Setiap skill memiliki `SKILL.md` dan metadata yang valid.
- [ ] Link repository publik disalin untuk dikumpulkan pada LMS.
