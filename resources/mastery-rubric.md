# Mastery Rubric — Status, Scoring, & Spaced Review

Dibaca saat menentukan status penguasaan murid dan saat menjadwalkan review.

## Status penguasaan

Gunakan lima status ini untuk setiap grammar point. Jangan melompat ke status lebih tinggi hanya karena beberapa jawaban benar — status harus mencerminkan kemampuan nyata.

| Status | Kriteria |
|---|---|
| `NEW` | Baru diperkenalkan, belum melewati controlled practice |
| `LEARNING` | Sudah paham arti & pola dasar, tapi masih sering perlu bantuan/hint saat production |
| `UNSTABLE` | Bisa benar di controlled practice tapi masih sering salah saat konteksnya berubah atau dicampur dengan grammar mirip |
| `PRACTICED` | Konsisten benar di controlled + contextual + transformation, sudah cukup lancar, tapi belum diuji lewat bacaan/production bebas secara memadai |
| `MASTERED` | Memenuhi SEMUA kriteria mastery checklist di bawah |

### Checklist untuk status `MASTERED`

Grammar hanya boleh diberi status `MASTERED` jika murid terbukti mampu:

- [ ] Memahami arti inti dengan benar
- [ ] Mengenali konteks kapan pola ini tepat dipakai
- [ ] Memilih pola yang benar di antara pilihan yang membingungkan (bukan cuma recognition sederhana)
- [ ] Membentuk kalimat sendiri dengan pola ini secara gramatikal benar
- [ ] Mengubah/mentransformasi kalimat memakai pola ini
- [ ] Menggunakan pola ini dalam konteks yang belum pernah dilatih sebelumnya (bukan hafalan contoh)
- [ ] Memahami pola ini saat muncul dalam bacaan (dokkai)
- [ ] Membedakan pola ini dari grammar mirip dengan penjelasan yang benar, bukan tebakan
- [ ] Memakai pola ini dengan kealamian yang relatif wajar (bukan gramatikal tapi kaku/aneh)

Kalau satu poin saja belum terpenuhi dengan meyakinkan, status maksimal adalah `PRACTICED`, dan katakan secara eksplisit ke murid poin mana yang belum terpenuhi supaya mereka tahu progresnya nyata.

## Sistem nilai (scoring)

Jangan hanya melihat persentase akurasi mentah. Gunakan pedoman:

| Akurasi | Interpretasi awal |
|---|---|
| 90–100% | Kuat |
| 80–89% | Cukup stabil |
| 70–79% | Perlu review |
| < 70% | Perlu drilling ulang dari dasar |

**Tapi** persentase ini harus dikoreksi dengan kategori kesalahan (lihat `error-taxonomy.md`) — 8/10 benar karena betul-betul paham TIDAK SAMA dengan 8/10 benar karena menebak atau careless mistake berulang. Kalau kamu curiga murid menebak (mis. pola jawaban acak, ragu-ragu di free-text), tanyakan alasannya sebelum mencatat sebagai correct penuh.

## Spaced review

Kalau kamu punya cara menyimpan state antar sesi (lihat SKILL.md §9), gunakan jadwal berikut sebagai acuan (hari dihitung sejak grammar itu pertama kali diajarkan, bukan kalender pasti — sesuaikan ke sesi belajar aktual murid):

```
Sesi 1  : belajar pertama kali
Sesi +1 : review ringan (beberapa soal campuran)
Sesi +2 hingga +3 : review sedang
Sesi +4 hingga +5 : review lanjut
Sesi +tengah waktu : mastery check ulang
```

Prioritas review, dari yang paling mendesak:
1. Grammar berstatus `UNSTABLE` (paling butuh review karena rawan salah lagi)
2. Grammar berstatus `LEARNING`
3. Grammar berstatus `PRACTICED` (review lebih jarang, sekadar menjaga ingatan)
4. Grammar berstatus `MASTERED` (review paling jarang, biasanya lewat JLPT Simulation Mode saja)

Kalau tidak ada persistensi file: di akhir setiap sesi, tampilkan ringkasan singkat berisi status semua grammar yang dibahas hari itu + rekomendasi grammar apa yang perlu direview di sesi berikutnya, supaya murid bisa paste ulang ringkasan itu untuk melanjutkan.

## Format ringkasan status (dipakai di akhir Mastery Check maupun akhir sesi)

```
📊 Ringkasan Progres

Pola: ～XXXX
Status: [NEW/LEARNING/UNSTABLE/PRACTICED/MASTERED]
Kelemahan tercatat: [ambil dari error-taxonomy.md, atau "belum ada"]
Rekomendasi: [lanjut ke pola baru / review ringan sesi depan / drill ulang X]
```