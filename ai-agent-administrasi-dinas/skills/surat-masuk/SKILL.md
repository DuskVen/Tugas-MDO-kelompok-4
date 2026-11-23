---
name: surat-masuk
description: Membantu mencatat, mengelompokkan secara awal, dan meringkas surat masuk untuk administrasi perkantoran dinas. Gunakan saat pegawai memberikan isi atau metadata surat masuk yang boleh diproses.
---

# Skill: Pengelolaan Surat Masuk

## Tujuan
Mempercepat pencatatan administratif surat masuk tanpa menggantikan pemeriksaan dan disposisi pejabat.

## Masukan
- Teks surat atau metadata yang telah disamarkan.
- Tanggal diterima (jika tersedia).
- Unit penerima (jika boleh dibagikan).
- Format kolom buku agenda yang digunakan instansi (jika ada).

## Instruksi
1. Ekstrak hanya informasi yang benar-benar tercantum: nomor surat, tanggal surat, tanggal diterima, pengirim, tujuan, perihal, lampiran.
2. Jika informasi tidak ditemukan, isi `Belum tercantum`; jangan menebak.
3. Buat ringkasan netral maksimal 3 kalimat.
4. Berikan kategori awal, misalnya undangan, permohonan, pemberitahuan, laporan, atau lainnya. Tandai sebagai saran, bukan klasifikasi resmi.
5. Tunjukkan informasi yang perlu diverifikasi.
6. Jika diminta, buat konsep daftar tindak lanjut tanpa menetapkan disposisi atau pejabat penanggung jawab.
7. Jangan menampilkan ulang data pribadi yang tidak diperlukan.

## Format keluaran
| Kolom | Hasil |
|---|---|
| Nomor surat | |
| Tanggal surat | |
| Tanggal diterima | |
| Pengirim | |
| Tujuan/unit | |
| Perihal | |
| Lampiran | |
| Kategori awal (saran AI) | |
| Ringkasan | |
| Data yang perlu diverifikasi | |

## Batasan
- Tidak menetapkan disposisi, tingkat urgensi resmi, atau keputusan.
- Tidak membuat nomor agenda/nomor surat.
- Tidak mengirim atau meneruskan surat.
- Pegawai wajib mencocokkan hasil dengan dokumen asli.
