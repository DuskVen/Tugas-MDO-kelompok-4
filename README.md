# Clinic Intake Assistant — AI Agent Skills

AI Agent berbasis instruksi untuk membantu pekerjaan repetitif di bagian registrasi dan anamnesa awal klinik. Proyek ini merupakan demonstrasi konsep/workflow dan **bukan aplikasi rekam medis** atau pengganti petugas/dokter.

## Tujuan
- Membantu petugas mengumpulkan data registrasi pasien secara terstruktur.
- Mengajukan pertanyaan anamnesa awal secara bertahap.
- Memeriksa kelengkapan informasi dan meminta klarifikasi bila perlu.
- Menghasilkan ringkasan anamnesa untuk ditinjau petugas klinik.

## Jobdesk yang dianalisis
| Jobdesk | Aktivitas repetitif | Dukungan agent |
|---|---|---|
| Registrasi | Mengumpulkan identitas dan status pasien baru/lama | Formulir data terstruktur, pemeriksaan kolom wajib |
| Pengecekan data | Memeriksa kolom kosong/ketidaksesuaian | Checklist kelengkapan, permintaan klarifikasi |
| Anamnesa awal | Mengumpulkan keluhan, durasi, gejala terkait, alergi, obat, riwayat relevan | Tanya-jawab bertahap dan pencatatan jawaban |
| Dokumentasi kunjungan | Merapikan hasil wawancara | Ringkasan terstruktur untuk petugas/dokter |
| Informasi alur layanan | Menjawab pertanyaan umum proses pendaftaran | Jawaban FAQ hanya berdasarkan informasi klinik yang disediakan |

## Skills dalam repo
- `SKILL.md`: instruksi utama agent dan router tugas.
- `skills/patient-registration/SKILL.md`: skill registrasi.
- `skills/initial-anamnesis/SKILL.md`: skill anamnesa awal.
- `skills/anamnesis-summary/SKILL.md`: skill ringkasan dan handoff.
- `examples/sample-conversation.md`: simulasi memakai data fiktif.
- `jobdesk-analysis.md`: analisis jobdesk dan peluang otomasi.

## Cara menggunakan
1. Baca `SKILL.md` sebagai instruksi utama.
2. Jika tersedia lingkungan AI yang mendukung skill Markdown, gunakan folder skill ini sesuai format dan instruksi platform tersebut.
3. Jika hanya ingin mencoba, salin instruksi ke AI assistant dan gunakan data **fiktif**. Jalankan simulasi registrasi/anamnesa.
4. Tinjau output untuk kelengkapan, konsistensi, dan apakah agent mematuhi batasan keselamatan.

Skill Markdown ini adalah instruksi yang dapat dipakai/adaptasi oleh AI, bukan agent otonom yang sudah terhubung ke sistem klinik, database, WhatsApp, atau rekam medis.


## Privasi, keselamatan, dan batasan
- Jangan menguji menggunakan data pasien asli atau identitas sensitif.
- Jangan membuat diagnosis, menyimpulkan kondisi, menyarankan obat, atau menentukan terapi.
- Jangan mengarang informasi pasien; tandai yang belum ditanyakan atau belum dikonfirmasi.
- Ringkasan harus ditinjau dan dikonfirmasi petugas klinik/dokter.
- Bila pasien menyebut tanda bahaya, hentikan wawancara rutin dan arahkan agar segera mendapatkan pertolongan medis. Agent tidak melakukan triase klinis mandiri.
- Jangan menyalin data pribadi atau medis ke repository publik.

## Repository
Proyek ini dibuat sebagai contoh tugas pengelolaan AI Agent Skills. Gunakan data simulasi untuk demonstrasi.
