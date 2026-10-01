# Japanese Private Sensei 🇯🇵

Skill AI untuk belajar bahasa Jepang secara serius. AI akan berperan sebagai **sensei pribadi** yang mengajar, mendrill, menguji, mengoreksi, dan melacak kelemahanmu — bukan sekadar menjelaskan grammar lalu selesai.

**Level yang didukung:** JLPT **N5 · N4 · N3 · N2 · N1** dan **Irodori** (A1–B1).
**Bahasa penjelasan:** Indonesia. **Kanji:** selalu disertai furigana.

---

## Isi paket

| File | Fungsi |
|---|---|
| `SKILL.md` | Otak utama: peran sensei, deteksi level, mode belajar, aturan feedback |
| `pedagogy.md` | Cara mengajar & membedakan grammar yang mirip |
| `drill-engine.md` | Jenis latihan, level kesulitan adaptif, mode drill & simulasi |
| `error-taxonomy.md` | Klasifikasi & pelacakan kesalahanmu (weakness detection) |
| `mastery-rubric.md` | Status penguasaan (NEW → MASTERED), scoring, jadwal review |
| `examples.md` | Contoh gaya penjelasan dan soal |

---

## Cara pakai

1. **Download semua file**: `SKILL.md`, `pedagogy.md`, `drill-engine.md`, `error-taxonomy.md`, `mastery-rubric.md`, dan `examples.md`.
2. **Buka AI favoritmu**, misalnya Claude, ChatGPT, atau Gemini.
3. **Upload semua file** yang sudah kamu download (enam file sekaligus).
4. **Paste prompt berikut:**

   ```
   Silakan baca dan pahami SKILL.md yang sudah saya upload. Pastikan role dan
   karakter kamu persis seperti di SKILL.md saya.
   ```

5. **Sensei otomatis menampilkan menu pembuka.** Pilih menu (pola kalimat atau kotoba), lalu jawab beberapa pertanyaan singkat: kosakata khusus, furigana, dan jumlah soal. Setelah itu sesi dimulai.

> Tips: sebutkan level di awal supaya materi pas. Contoh: `N4 ～てしまう`. Kalau tidak menyebut level, sensei akan menebak dari polanya dan memberi tahu asumsinya; kamu tinggal koreksi.

---

## Alur sesi: menu & pertanyaan awal

Sebelum mengajar, sensei menanyakan kebutuhanmu **satu pertanyaan per giliran**, seperti konsultasi dua arah. Setelah kamu mengirim prompt pembuka, kamu akan melihat menu seperti ini:

```
1. Pola kalimat apa yang ingin kamu dalami hari ini?
2. Apakah kamu ingin latihan kotoba hari ini? (ketik 2, lalu paste list kotoba kamu)
3. Tes level
4. Review kelemahan sesi sebelumnya
5. Mode khusus: gas drill / JLPT mode / mode Irodori
```

**Jalur 1: pola kalimat**

1. Kamu ketik polanya (boleh sebut level, mis. `N4 ～てしまう`).
2. Sensei bertanya: *"Apakah kamu memiliki list kosakata khusus yang bisa saya gunakan?"* Kalau kamu paste list, kata-kata itu dipakai di contoh dan soal. Kalau tidak, ketik `skip`.
3. Sensei bertanya: *"Apakah di setiap penjelasan dan latihan, kanji ditampilkan dengan furigana?"* Pilihannya: semua kanji, tidak, atau hanya kanji sulit.
4. Sensei bertanya: *"Berapa butir soal yang kamu inginkan di setiap sesi?"*
5. Sensei menampilkan ringkasan pilihanmu, lalu langsung mulai dengan diagnosis singkat dan pengajaran.

**Jalur 2: kotoba.** Ketik `2` dan paste list kotoba atau kanji. Sensei lalu menanyakan furigana dan jumlah soal, kemudian melatih kata-katamu dengan berbagai jenis soal.

**Jalur cepat.** Kamu bisa menjawab sekaligus, mis. `N4 ～てしまう, skip, furigana ya, 10 soal`, dan pertanyaan yang sudah terjawab dilewati. Ketik `langsung aja` untuk memakai pengaturan default (furigana semua kanji, 10 soal). Pilihan furigana dan jumlah soal berlaku sepanjang sesi dan bisa diubah kapan saja (mis. `matikan furigana`, `jadi 20 soal`).

---

## Contoh input

| Yang kamu ketik | Yang terjadi |
|---|---|
| `～ために` | Sensei menebak level, menanyakan kosakata, furigana, dan jumlah soal, lalu diagnosis, mengajar, dan mendrill |
| `N5 ～ています` | Belajar pola itu dengan kosakata dan kalimat level N5 |
| `N2 ～わけにはいかない` | Penjelasan nuansa tingkat lanjut + pembedaan dengan pola mirip |
| `N3 ～ことになっている` + `会社, ルール, 毎日, 禁止する` | Contoh dan soal wajib memakai 4 kosakata itu |
| `Irodori A2 ～てもいいですか` | Belajar lewat situasi nyata, dialog, dan role-play |
| `saya masih bingung ～たら dan ～なら` | Langsung ke pembedaan kontras + drill A vs B |

## Perintah sesi

| Perintah | Fungsi |
|---|---|
| `menu` | Tampilkan menu pembuka kapan saja |
| `tes level` | Tes penempatan singkat untuk menentukan levelmu |
| `gas drill` / `uji gue` / `habisin gue` / `full drill` | Mode drill intensif ("Sensei Galak"): langsung soal, campur grammar, berjalan sampai kelemahanmu kelihatan |
| `JLPT mode` | Simulasi ujian: tanpa hint, pembahasan setelah semua selesai |
| `mode Irodori` / `role-play` | Latihan komunikatif berbasis situasi dan dialog |
| `review grammar kemarin` | Review pola yang berstatus lemah |
| `ganti level ke N3` | Pindah level; data kelemahan lama tetap dibawa |
| `kasih latihan N4` | Latihan sesuai level |

---

## Cara kerja singkat

1. **Diagnosis**: beberapa soal untuk mengecek posisimu, tanpa kunci jawaban dulu.
2. **Teaching**: arti inti, nuansa, pola pembentukan, cara berpikir, dan contoh dengan furigana.
3. **Pembedaan grammar mirip**: dijelaskan lewat kalimat kontras, bukan sekadar "konteksnya beda".
4. **Latihan bertahap**: pilihan ganda, cloze, menyusun kalimat, transformasi, produksi bebas, bacaan atau dialog.
5. **Koreksi detail**: setiap jawaban salah dijelaskan kenapa salah dan kenapa pilihanmu terlihat masuk akal.
6. **Status penguasaan**: `NEW → LEARNING → UNSTABLE → PRACTICED → MASTERED`. Status MASTERED hanya diberikan kalau kamu terbukti bisa memakai pola itu secara nyata, bukan hanya karena beberapa jawaban benar.

---

## Menyimpan progres antar sesi

Kebanyakan AI chat **tidak mengingat** sesi sebelumnya. Sensei akan memberi **ringkasan progres** di akhir sesi (termasuk level, preferensi furigana, dan jumlah soal). Caranya:

1. **Copy ringkasan** itu di akhir sesi.
2. Di sesi baru, upload file skill lagi, paste prompt langkah 4, lalu **paste ringkasan tadi**.
3. Sensei melanjutkan dari status dan kelemahanmu sebelumnya.

Kalau kamu memakai tool yang bisa menyimpan file (mis. Claude Code), progres bisa disimpan otomatis di `progress-log.md`.

---

## Catatan

- **Hasil di ChatGPT dan Gemini bisa sedikit berbeda** dari Claude. Jika AI mulai "keluar karakter" (terlalu banyak basa-basi, tidak memberi drill), paste ulang prompt langkah 4.
- Sensei tidak akan mengarang aturan grammar. Kalau suatu pola ambigu atau pengelompokan levelnya berbeda antar buku, dia akan bilang terus terang. Untuk hal penting, cek ulang dengan kamus atau buku resmi.
- Semua soal, contoh, dan bacaan dibuat **original**; isi buku pelajaran tidak disalin.
- Pengelompokan level pola (N5–N1) bisa berbeda antar sumber. Anggap level dari sensei sebagai acuan praktis, bukan daftar resmi ujian.
- Beberapa file pendukung masih memakai N3 sebagai contoh gaya. `SKILL.md` sudah mengatur agar AI menyesuaikannya dengan levelmu.

Selamat belajar. がんばってください！