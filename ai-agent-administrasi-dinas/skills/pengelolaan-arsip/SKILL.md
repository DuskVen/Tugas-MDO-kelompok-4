---
name: pengelolaan-arsip
description: Membantu menyarankan nama file, metadata, dan indeks untuk dokumen administrasi yang boleh diproses. Gunakan saat menata atau mencari arsip.
---

# Skill: Pengelolaan Arsip

## Tujuan
Membantu konsistensi penamaan dan pencatatan arsip, bukan menetapkan klasifikasi resmi.

## Masukan
- Jenis dokumen.
- Tanggal dokumen.
- Unit pengolah.
- Perihal singkat.
- Kode klasifikasi resmi jika telah ditentukan instansi.
- Status akses yang telah ditetapkan petugas.

## Instruksi
1. Buat usulan nama file yang konsisten: `YYYY-MM-DD_Unit_JenisDokumen_PerihalSingkat`.
2. Hindari memasukkan nama lengkap, NIK, alamat, atau data pribadi ke nama file.
3. Susun metadata: tanggal, unit, jenis dokumen, perihal, kata kunci, dan lokasi penyimpanan.
4. Jangan membuat kode klasifikasi, tingkat kerahasiaan, masa retensi, atau keputusan pemusnahan.
5. Jika metadata tidak ada, tandai `Belum tersedia`.
6. Untuk pencarian, berikan kata kunci yang relevan dari informasi yang diberikan.

## Format keluaran
| Metadata | Hasil/usulan |
|---|---|
| Nama file | |
| Tanggal | |
| Unit | |
| Jenis dokumen | |
| Perihal | |
| Kata kunci | |
| Kode klasifikasi resmi | Diisi/diverifikasi petugas |
| Hak akses | Ditetapkan petugas |
| Lokasi arsip | |

## Batasan
AI hanya memberi saran administratif. Pengelolaan arsip resmi mengikuti SOP, klasifikasi keamanan, dan jadwal retensi arsip instansi.
