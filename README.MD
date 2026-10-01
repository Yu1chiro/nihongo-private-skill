# Japanese Private Sensei

> Sistem belajar Bahasa Jepang yang menggabungkan pengajaran, latihan,
> koreksi, deteksi kelemahan, dan review dalam satu rangkaian belajar
> yang saling terhubung.

## Apa yang membedakan Japanese Private Sensei dengan prompting biasa?

Kalau **prompting biasa**, kita biasanya memberikan perintah kepada AI,
kemudian AI memberikan jawaban.

Contohnya:

> "Jelaskan perbedaan ～より dan ～ほうが dengan bahasa sederhana."

AI akan memberikan penjelasan sesuai perintah tersebut.

Namun, prosesnya biasanya berhenti pada jawaban tersebut. AI belum tentu
mengetahui apakah kita benar-benar sudah memahami materi, bagian mana
yang masih sering salah, atau materi apa yang perlu dipelajari kembali.

**Japanese Private Sensei menggunakan konsep yang berbeda.**

Sistem ini menghubungkan beberapa proses belajar menjadi satu rangkaian:

**Belajar → Latihan → Koreksi → Deteksi Kesalahan → Review →
Penguasaan**

Jadi, Sensei tidak hanya berperan sebagai AI yang menjelaskan materi,
tetapi juga membantu **melatih, menguji, mengoreksi, dan memantau
perkembangan belajar.**

------------------------------------------------------------------------

## Bagaimana cara kerjanya?

Bayangkan kita sedang belajar grammar Bahasa Jepang.

1.  **Sensei menjelaskan materi**
    -   Materi dijelaskan dengan cara yang mudah dipahami.
    -   Jika ada grammar yang mirip, perbedaannya dijelaskan secara
        kontekstual.
2.  **Sensei memberikan latihan**
    -   Pengguna mengerjakan soal sesuai materi yang sedang dipelajari.
    -   Tingkat latihan dapat disesuaikan dengan kemampuan.
3.  **Jawaban diperiksa**
    -   Jawaban benar dan salah dicatat.
    -   Kesalahan tidak hanya dianggap sebagai "salah", tetapi digunakan
        sebagai informasi untuk melihat pola kesalahan.
4.  **Kelemahan mulai terlihat**
    -   Misalnya pengguna sering salah membedakan ～より dan ～ほうが.
    -   Sistem dapat mengenali bahwa bagian tersebut masih perlu
        diperkuat.
5.  **Latihan berikutnya diarahkan**
    -   Pengguna tidak harus mengulang semua materi dari awal.
    -   Latihan dapat lebih difokuskan pada bagian yang masih lemah.
6.  **Penguasaan diperbarui**
    -   Setelah beberapa latihan, sistem dapat membantu melihat apakah
        materi masih perlu di-review atau sudah mulai dikuasai.

Dengan begitu, proses belajar menjadi lebih terarah.

------------------------------------------------------------------------

## Contoh sederhana

Misalnya kamu sedang belajar:

**～より dan ～ほうが**

Setelah mendapatkan penjelasan, kamu mengerjakan 10 soal.

Hasilnya:

-   6 soal benar
-   4 soal salah
-   Sebagian besar kesalahan terjadi saat menggunakan **～ほうが**

Daripada hanya mengatakan:

> "Jawabanmu salah."

Japanese Private Sensei menggunakan kesalahan tersebut sebagai informasi
belajar.

Latihan berikutnya dapat diarahkan kembali pada penggunaan **～ほうが**,
sehingga kamu memiliki kesempatan untuk memperbaiki bagian yang memang
masih belum dikuasai.

Jadi, alurnya bukan:

> **Tanya → Jawab → Selesai**

Tetapi:

> **Belajar → Latihan → Dikoreksi → Kesalahan dianalisis → Latihan
> kembali → Cek penguasaan**

------------------------------------------------------------------------

## Struktur Sistem

Japanese Private Sensei menggunakan beberapa file yang memiliki fungsi
berbeda, tetapi saling berhubungan.

  -----------------------------------------------------------------------
  File                                Fungsi
  ----------------------------------- -----------------------------------
  `SKILL.md`                          Mengatur peran Sensei, cara membaca
                                      level pengguna, mode belajar, dan
                                      aturan feedback

  `pedagogy.md`                       Mengatur cara mengajar dan
                                      membedakan grammar yang mirip

  `drill-engine.md`                   Mengatur jenis latihan, tingkat
                                      kesulitan, mode drill, dan simulasi

  `error-taxonomy.md`                 Mengklasifikasikan dan melacak
                                      kesalahan pengguna

  `mastery-rubric.md`                 Menentukan status penguasaan
                                      materi, dari **NEW** sampai
                                      **MASTERED**

  `examples.md`                       Menyediakan contoh gaya penjelasan
                                      dan contoh soal
  -----------------------------------------------------------------------

### Hubungan antarbagian

File-file tersebut tidak dimaksudkan untuk bekerja secara terpisah.

Secara sederhana, hubungannya seperti ini:

``` text
                 SKILL.md
                    │
                    ▼
             Cara Sensei mengajar
                    │
          ┌─────────┴─────────┐
          ▼                   ▼
    pedagogy.md          drill-engine.md
          │                   │
          │              Latihan & soal
          │                   │
          └─────────┬─────────┘
                    ▼
              Jawaban pengguna
                    │
                    ▼
           error-taxonomy.md
                    │
              Deteksi kesalahan
                    │
                    ▼
            mastery-rubric.md
                    │
          Status penguasaan materi
                    │
                    ▼
             Review berikutnya
```

------------------------------------------------------------------------

## Apa fungsi masing-masing file?

### `SKILL.md`

Ini bisa dianggap sebagai **otak utama Sensei**.

File ini menentukan bagaimana Sensei harus berperan dalam proses
belajar, misalnya:

-   bagaimana menjelaskan materi;
-   bagaimana membaca level pengguna;
-   bagaimana memberikan feedback;
-   bagaimana menjalankan mode belajar;
-   bagaimana menghubungkan proses belajar dengan bagian sistem lainnya.

------------------------------------------------------------------------

### `pedagogy.md`

Bagian ini mengatur **cara mengajar**.

Ini penting terutama ketika ada grammar yang terlihat mirip.

Contohnya:

-   ～より
-   ～ほうが
-   ～が好き
-   ～が上手
-   dan grammar lain yang sering membingungkan pemula.

Tujuannya bukan hanya memberikan definisi, tetapi membantu pengguna
memahami **kapan dan bagaimana grammar tersebut digunakan.**

------------------------------------------------------------------------

### `drill-engine.md`

Bagian ini mengatur **latihan**.

Misalnya:

-   jenis soal;
-   tingkat kesulitan;
-   latihan bertahap;
-   mode drill;
-   simulasi.

Dengan demikian, pengguna tidak hanya membaca materi, tetapi juga
langsung menggunakannya melalui latihan.

------------------------------------------------------------------------

### `error-taxonomy.md`

Bagian ini berfungsi untuk **membaca kesalahan pengguna**.

Contohnya, pengguna mungkin salah karena:

-   memilih grammar yang tidak tepat;
-   salah memahami arti;
-   salah menggunakan bentuk kalimat;
-   atau masih tertukar dengan grammar lain.

Kesalahan tersebut dapat dikelompokkan sehingga kita tidak hanya
mengetahui bahwa pengguna "salah", tetapi juga **bagian mana yang perlu
diperbaiki.**

------------------------------------------------------------------------

### `mastery-rubric.md`

Bagian ini digunakan untuk melihat **tingkat penguasaan materi**.

Contohnya:

``` text
NEW → LEARNING → REVIEW → MASTERED
```

Artinya, materi tidak dianggap langsung "selesai" hanya karena pengguna
sudah membaca penjelasannya.

Penguasaan dilihat dari proses latihan dan hasil yang diperoleh.

------------------------------------------------------------------------

### `examples.md`

File ini berisi **contoh gaya penjelasan dan contoh soal**.

Tujuannya agar gaya Sensei tetap konsisten ketika menjelaskan materi
atau membuat latihan.

------------------------------------------------------------------------

## Perbedaan sederhananya

  -----------------------------------------------------------------------
  Prompting biasa                     Japanese Private Sensei
  ----------------------------------- -----------------------------------
  Memberikan perintah ke AI           Mengikuti proses belajar

  Fokus pada jawaban                  Fokus pada perkembangan pengguna

  Penjelasan selesai → selesai        Penjelasan → latihan → koreksi →
                                      review

  Kesalahan bisa berhenti pada        Kesalahan digunakan sebagai
  feedback                            informasi belajar

  Tidak harus memiliki riwayat        Memiliki konsep penguasaan materi
  penguasaan                          

  Setiap prompt dapat berdiri sendiri Bagian-bagian sistem saling
                                      terhubung
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## Inti Konsep

Japanese Private Sensei bukan sekadar:

> **"AI yang bisa menjelaskan Bahasa Jepang."**

Konsep utamanya adalah:

> **"AI yang membantu menjalankan proses belajar Bahasa Jepang secara
> berkelanjutan."**

Dengan menggabungkan **pengajaran, latihan, koreksi, deteksi kelemahan,
dan review**, sistem ini dirancang agar proses belajar tidak berhenti
pada satu jawaban.

### Singkatnya

``` text
AI biasa:
Pertanyaan → Jawaban

Japanese Private Sensei:
Belajar
   ↓
Latihan
   ↓
Koreksi
   ↓
Deteksi kelemahan
   ↓
Latihan kembali
   ↓
Review
   ↓
Penguasaan
```

Itulah gagasan utama di balik **Japanese Private Sensei**.
