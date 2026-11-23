---
name: campaign-report
description: Meringkas data performa kampanye digital menjadi laporan yang memisahkan angka, interpretasi, keterbatasan, dan rekomendasi awal.
---

# Campaign Report Skill

## Tujuan
Mempercepat laporan rutin kampanye berdasarkan data yang diberikan tim.

## Input
CSV/tabel metrik, periode laporan, kanal/kampanye, definisi KPI, dan target (jika ada).

## Instruksi
1. Identifikasi kolom, periode, satuan, dan data kosong/duplikat.
2. Jangan mengarang angka. Jika metrik tidak tersedia, tulis “Tidak tersedia”.
3. Hitung hanya metrik yang didukung kolom. Contoh:
   - CTR = clicks / impressions × 100%
   - CPC = spend / clicks
   - CPM = spend / impressions × 1.000
   - Engagement rate = engagements / reach × 100% (gunakan definisi ini hanya jika sesuai definisi tim)
   - Conversion rate = conversions / clicks × 100% (jika definisi tim menggunakan clicks sebagai denominator)
4. Sebutkan rumus dan denominator yang digunakan.
5. Bandingkan dengan target atau periode sebelumnya hanya jika data pembanding tersedia.
6. Pisahkan:
   - Fakta (angka dari data)
   - Interpretasi (kemungkinan penjelasan)
   - Rekomendasi awal (perlu validasi manusia)
7. Jangan menyatakan sebab-akibat hanya dari korelasi sederhana.
8. Jangan menyarankan perubahan anggaran otomatis.

## Format output
### Ringkasan eksekutif
### Tabel KPI
### Perubahan penting
### Interpretasi
### Keterbatasan data
### Rekomendasi awal
### Pertanyaan untuk tim

## Quality check
Periksa pembagian nol, satuan mata uang, periode, definisi KPI, dan konsistensi angka sebelum menyimpulkan.
