# Error Taxonomy — Melacak & Memanfaatkan Kesalahan Murid

Ini fitur paling penting dari skill ini (lihat SKILL.md §8-9). Dibaca setiap kali murid menjawab salah, dan saat merancang soal susulan.

## Kategori kesalahan

Setiap kali murid salah, klasifikasikan (boleh di kepala, tidak perlu selalu ditulis eksplisit ke murid kecuali relevan) ke salah satu kategori berikut. Ini menentukan jenis drill susulan yang tepat — solusinya berbeda untuk tiap kategori:

| Kategori | Ciri | Drill susulan yang tepat |
|---|---|---|
| **Careless mistake** | Murid sebenarnya tahu, tapi salah baca/salah ketik/keliru sesaat | Soal serupa singkat untuk konfirmasi, tidak perlu penjelasan ulang panjang |
| **Conceptual mistake** | Salah paham inti makna/nuansa pola | Kembali ke Teaching singkat (bagian "arti inti"/"nuansa"), lalu soal recognition ulang |
| **Vocabulary mistake** | Grammar-nya benar tapi salah karena tidak tahu arti kata di soal | Klarifikasi kosakata itu, lanjutkan soal (jangan turunkan level grammar-nya) |
| **Particle mistake** | Salah partikel pendamping pola (は/が/に/で, dst.) | Drill partikel spesifik untuk pola ini beberapa soal berturut-turut |
| **Grammar confusion** | Tertukar dengan pola mirip (lihat `pedagogy.md` §Daftar pasangan) | WAJIB jalankan bagian pembedaan kontras, lalu drill soal berpasangan A vs B |
| **Reading mistake** | Salah pahami maksud dalam bacaan (dokkai), bukan grammar-nya sendiri | Beri bacaan pendek lain dengan pertanyaan sejenis, fokus ke jenis pertanyaan yang salah (rujukan/inferensi/dsb.) |
| **Production mistake** | Kalimat buatan sendiri gramatikal tapi tidak natural atau konteksnya kurang pas | Tunjukkan versi natural, minta murid membuat kalimat baru dengan feedback itu diterapkan |

## Mendeteksi weakness yang berulang

Kalau murid melakukan kesalahan kategori yang sama (atau tertukar pasangan grammar yang sama) **≥2 kali** dalam satu topik/sesi, catat sebagai **WEAKNESS** eksplisit, contoh:

```
⚠️ WEAKNESS terdeteksi: tertukar ～ように vs ～ために (tujuan yang diharapkan vs
tujuan yang bisa dikontrol penutur)
```

Setelah WEAKNESS tercatat:
- Soal-soal berikutnya (tidak harus langsung berurutan, tapi dalam beberapa soal ke depan) harus secara sengaja menyasar titik lemah itu.
- Jangan kembali ke soal generik acak sampai murid menunjukkan perbaikan konsisten (≈3 kali benar berturut dengan pemahaman yang jelas, bukan kebetulan).
- Bawa WEAKNESS ini ke sesi/mode berikutnya (mis. kalau murid pindah ke "gas drill", tetap selipkan soal yang menyasar WEAKNESS lama).

## Format feedback lengkap (rujukan detail dari SKILL.md §8)

```
### Jawaban
[Benar / Salah / Partial — partial = grammar benar tapi pemahaman/alasan salah]

### Jawaban yang benar
[...]

### Kenapa
[Penjelasan gramatikal singkat, bukan "karena itu memang polanya"]

### Kenapa pilihanmu kelihatan masuk akal (khusus pilihan ganda yang salah)
[Jelaskan logika di balik pilihan murid, lalu tunjukkan titik di mana logika itu
tidak berlaku untuk pola ini]

### Bandingkan
[Kalau relevan, sandingkan dengan grammar mirip yang jadi sumber kebingungan —
lihat pedagogy.md §Daftar pasangan]

### Drill berikutnya
[1 soal baru yang secara spesifik menyasar kesalahan/kategori di atas]
```

Kalau jawaban **Partial** (grammar/kata benar tapi alasan murid salah saat ditanya kenapa, atau grammar benar tapi dipakai untuk maksud yang keliru): jangan tandai sebagai correct penuh dalam catatan progres — perlakukan seperti conceptual mistake ringan.

## Menghubungkan ke scoring

Saat menghitung akurasi untuk `mastery-rubric.md`, kesalahan careless TIDAK sama bobotnya dengan conceptual/grammar confusion. Kalau sebagian besar kesalahan murid careless, akurasi mentah boleh dianggap cukup representatif. Kalau sebagian besar conceptual/grammar confusion, jangan naikkan status mastery meskipun angka akurasi terlihat tinggi (mis. karena banyak soal recognition mudah yang kebetulan benar) — utamakan bukti pemahaman nyata dari jenis kesalahan yang tersisa.