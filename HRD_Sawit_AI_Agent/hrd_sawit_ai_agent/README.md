# AI Agent HRD - Perusahaan Kelapa Sawit

Repository kumpulan skill AI Agent untuk mendukung pekerjaan repetitif HRD perusahaan kelapa sawit. Agent berperan sebagai asisten administratif, bukan pengambil keputusan final.

## Skills
1. Employee Data: merapikan dan memvalidasi data karyawan.
2. Attendance: menganalisis rekap absensi dan menandai anomali.
3. Recruitment: merangkum kandidat berdasarkan kriteria yang ditetapkan.
4. Document Check: memeriksa kelengkapan dokumen administrasi.
5. Payroll Preparation: menyusun data pendukung penggajian tanpa menetapkan pembayaran final.
6. HR Reporting: menyusun laporan dan statistik HR.
7. HR FAQ: menjawab pertanyaan umum dari sumber kebijakan yang disediakan.
8. HR Reminder: menyusun daftar pengingat untuk dokumen dan kegiatan.

## Cara menggunakan
- Buka skill yang sesuai di folder `skills/`.
- Masukkan data yang diperlukan dengan format anonim atau data yang diizinkan perusahaan.
- Ikuti instruksi skill untuk hasil, format, dan validasi.
- HRD wajib memeriksa output sebelum digunakan untuk keputusan, pengiriman, pembayaran, atau tindakan resmi.

## Privasi dan batasan
- Jangan memasukkan data pribadi, identitas, rekening, informasi medis, atau data sensitif ke layanan AI yang tidak disetujui perusahaan.
- Agent tidak membuat keputusan final terkait perekrutan, disiplin, PHK, upah, atau hak karyawan.
- Agent tidak boleh mengarang data. Jika informasi kurang, tandai sebagai `BELUM TERSEDIA`.
- Gunakan sumber kebijakan internal yang berlaku dan verifikasi aturan hukum terbaru.

## Daftar aktivitas yang dapat diotomatisasi
| Aktivitas | Input | Output |
|---|---|---|
| Rekap data karyawan | CSV/XLSX dengan akses sah | Data terstruktur, duplikasi dan kolom kosong ditandai |
| Rekap absensi | Data kehadiran | Ringkasan, anomali, daftar perlu verifikasi |
| Seleksi administratif | CV dan kriteria posisi | Matriks kecocokan berbasis kriteria, bukan keputusan |
| Kelengkapan dokumen | Checklist dan status dokumen | Daftar lengkap/kurang dan tindak lanjut |
| Persiapan payroll | Data absensi/lembur dan aturan terverifikasi | Rekap pendukung, bukan otorisasi pembayaran |
| Laporan HR | Data rekap | Ringkasan dan tabel |
| FAQ HR | Dokumen kebijakan | Jawaban dengan referensi dokumen |
| Pengingat | Daftar tanggal dan item | Daftar reminder |

## Struktur
```text
skills/
  employee-data/SKILL.md
  attendance/SKILL.md
  recruitment/SKILL.md
  document-check/SKILL.md
  payroll-preparation/SKILL.md
  reporting/SKILL.md
  hr-faq/SKILL.md
  reminder/SKILL.md
```
