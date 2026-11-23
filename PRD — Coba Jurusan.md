# PRD — Coba Jurusan

Nov 23, 2026 · ide tambahan, disusun dari Guidebook Hackvidia 11.0

## Ringkasan

**Coba Jurusan** membiarkan siswa SMA/SMK **mencicipi seminggu kuliah dan kerja** di sebuah jurusan sebelum memilihnya. Siswa tidak hanya mengisi tes minat bakat tentang dirinya. Mereka benar-benar **mengerjakan** tugas-tugas khas jurusan itu dalam versi ringan, ngobrol dengan persona kakak tingkat dan alumni yang disusun dari wawancara nyata, lalu melihat **Cermin Minat**: tugas mana yang mereka nikmati, mana yang terasa menyiksa, dan mana yang ternyata mereka kuasai.

**One-liner:** *Jangan pilih jurusan dari namanya. Coba dulu kerjaannya.*

**Konsep inti:** Kebanyakan siswa memilih jurusan dari nama, gengsi, passing grade, atau saran orang lain, tanpa pernah tahu seperti apa sehari-hari kuliahnya. Coba Jurusan mengganti pertanyaan "kamu suka apa?" dengan pengalaman langsung. Satu minggu mencoba "jadi mahasiswa Teknik Sipil" lebih jujur daripada 100 soal tes kepribadian.

**Subtema Hackvidia:** utama *AI for Learning & Self-Growth* (mengenali potensi dan minat sesuai kebutuhan masing-masing). Pendukungnya *AI for Inclusive Access* (siswa di sekolah tanpa guru BK memadai, atau tanpa kenalan yang kuliah).

**Prinsip desain:** Coba Jurusan **tidak pernah memutuskan** jurusan untuk siswa dan tidak memberi vonis "kamu cocok jurusan X". Yang diberikan adalah cermin pengalaman dan bahan diskusi. Keputusan tetap milik siswa, bersama orang tua dan guru BK.

**Hubungan dengan PRD lain:** Coba Jurusan adalah tahap paling awal dalam perjalanan yang sama dengan ide-ide lain di repo ini. **Coba Jurusan** membantu memilih jurusan, **Bertahan Kuliah** membantu tetap kuliah, **Sidang Bayangan** membantu lulus, dan **CareerMirror** membantu masuk dunia kerja. Pola "mencicipi masa depan sebelum terjadi" juga sejalan dengan **Diri Masa Depan**.

## Masalah

- **Taruhannya besar dan pesertanya banyak.** Pada 2026, pendaftar SNBP mencapai 806.242 siswa ([Bisnis.com](https://kabar24.bisnis.com/read/20260404/79/1964232/lolos-snbp-2026-ini-tahapan-wajib-sebelum-masuk-kuliah)), dan pendaftar UTBK-SNBT mencapai 871.496 orang ([JawaPos](https://www.jawapos.com/pendidikan/2605250285/hanya-2942-persen-dari-total-pendaftar-256369-calon-mahasiswa-diterima-snbt-2026)). Pilihan jurusan di jalur ini tidak mudah diulang: peserta yang lulus SNBP tidak boleh mengikuti SNBT maupun jalur mandiri pada 2026 hingga 2028 ([Kemdiktisaintek](https://kemdiktisaintek.go.id/news/article/hasil-snbp-2026-resmi-diumumkan-kemdiktisaintek-perkuat-jaminan-kip-kuliah)).
- **Banyak yang merasa salah pilih.** Survei Indonesia Career Center Network (2017) yang sering dikutip menyebut sekitar 87% mahasiswa merasa jurusannya tidak sesuai minat ([GNFI](https://www.goodnewsfromindonesia.id/2022/04/01/penyebab-fenomena-salah-jurusan)). *Catatan: survei ini sudah lama dan metodologinya tidak terlalu jelas, jadi dipakai sebagai indikasi. Tim perlu melengkapinya dengan survei sendiri.*
- **Penyebabnya adalah informasi, bukan kemampuan.** Penelitian menyebut tekanan orang tua, pengaruh lingkungan, dan kurangnya informasi sebagai penyebab utama salah memilih jurusan ([Jurnal UNMA](https://ejournal.unma.ac.id/index.php/dm/article/download/12231/6365/58589)).
- **Pendampingnya kurang.** Idealnya satu guru BK menangani maksimal 150 siswa, tapi di banyak sekolah rasionya jauh dari itu ([Jurnal UM](https://journal2.um.ac.id/index.php/jamp/article/download/62157/15683)). Di Kalimantan Timur misalnya, sekitar 30% guru BK bukan lulusan pendidikan BK ([Antara](https://kaltim.antaranews.com/berita/216093/disdikbud-kaltim-beri-penguatan-kapasitas-guru-bk-jenjang-sma)). Kemendikdasmen sekarang mendorong semua guru ikut berperan sebagai guru BK ([RRI](https://rri.co.id/samarinda/regional/2510838/disdikbud-kaltim-respons-kekurangan-guru-bk-dan-agama-di-sekolah-rakyat)), jadi guru mata pelajaran pun butuh alat bantu.
- **Dampaknya terasa saat kuliah.** Mahasiswa yang merasa salah jurusan umumnya kehilangan motivasi belajar, dan kondisi ini bisa memengaruhi prestasi akademik serta kesehatan mental mereka ([Binus](https://binus.ac.id/character-building/?p=7425)).

Intinya, siswa harus mengambil keputusan besar tanpa pernah "melihat ke dalam" jurusan yang mereka pilih.

## Target pengguna

| Persona | Situasi | Yang ia butuhkan |
| --- | --- | --- |
| **Nayla, 17, kelas 12 IPA di kota kabupaten** | Disuruh orang tua masuk Kedokteran, tapi diam-diam suka menggambar. Tidak punya kenalan yang kuliah Arsitektur atau DKV. | Pengalaman nyata dua-tiganya, supaya bisa membandingkan dan berbicara dengan orang tua pakai bukti, bukan perasaan. |
| **Raka, 17, kelas 12 SMK TKJ** | Bingung antara langsung kerja, D3, atau S1 Informatika. Tidak tahu bedanya. | Gambaran jujur tentang tugas sehari-hari di tiap jalur, termasuk yang membosankan. |
| **Bu Wati, 45, orang tua** | Ingin anaknya "jurusan yang pasti kerja", tapi tidak tahu banyak jurusan baru. | Ringkasan yang mudah dipahami tentang apa yang dinikmati dan dikuasai anaknya. |
| **Pak Hendra, 38, guru BK untuk 400 siswa** | Hanya bisa konseling singkat dengan tiap siswa kelas 12. | Ringkasan Cermin Minat setiap siswa sebelum sesi konseling, supaya waktu yang sedikit itu lebih bermakna. |

## Produk serupa dan pembeda

| Yang sudah ada | Apa yang dilakukan | Yang belum ada |
| --- | --- | --- |
| Rencanamu, Aku Pintar, Quipper (tes minat bakat) | Tes minat bakat, eksplorasi jurusan dan karier. Rencanamu bahkan bekerja sama dengan Direktorat SMA ([Industry.co.id](https://www.industry.co.id/read/75581/rencanamu-hadirkan-layanan-persiapan-kuliah-gratis)) | Berbasis **jawaban tentang diri sendiri** (self-report). Siswa yang belum tahu dirinya akan menjawab sesuai bayangan, bukan pengalaman |
| Artikel dan video "kuliah jurusan X itu seperti apa" | Informasi umum dari kampus atau kreator | Pasif; siswa menonton, tidak mencoba |
| Open house kampus dan *campus expo* | Pengalaman langsung yang bagus | Hanya di kota tertentu, setahun sekali, sulit dijangkau siswa daerah |
| Tanya kakak kelas atau saudara | Paling jujur | Hanya untuk yang punya kenalan; jurusannya terbatas |

**Lima pembeda Coba Jurusan:**

1. **Mengerjakan, bukan menjawab.** Siswa mengerjakan tugas khas jurusan: menghitung beban balok sederhana (Teknik Sipil), menganalisis kasus pasien fiktif (Keperawatan), membuat jurnal umum (Akuntansi), merancang poster (DKV). Sinyal minat datang dari perilaku dan perasaan saat mengerjakan, bukan dari pengakuan.
2. **Termasuk bagian yang membosankan.** Setiap simulasi memuat bagian "tidak glamor" yang nyata, misalnya laporan praktikum berulang atau hafalan anatomi. Yang dicari adalah jurusan yang bagian membosankannya masih bisa siswa jalani.
3. **Persona dari cerita nyata.** Kakak tingkat dan alumni AI disusun dari wawancara asli dengan mahasiswa dan lulusan (dengan izin), bukan karangan AI. Setiap jawaban persona bisa menunjukkan sumber ceritanya.
4. **Cermin, bukan vonis.** Hasilnya berupa peta pengalaman: apa yang dinikmati, apa yang dikuasai, apa yang menguras energi. Tidak ada label "kamu cocok jurusan X".
5. **Dibawa ke percakapan nyata.** Ada ringkasan khusus untuk orang tua dan guru BK, supaya diskusi keluarga berangkat dari pengalaman anak, bukan asumsi.

## Kapan AI dipakai, dan kapan tidak

Guidebook menilai kemampuan tim menentukan "kapan, bagaimana, dan sejauh mana AI perlu digunakan". Pembagiannya:

| Tugas | Dikerjakan oleh | Alasan |
| --- | --- | --- |
| Menyusun bank tugas per jurusan (kurikulum ringan, SOP, studi kasus) | Manusia (tim + dosen/mahasiswa relawan), dibantu AI untuk variasi | Isi harus akurat dan mewakili jurusan sebenarnya; AI hanya membuat variasi soal dari contoh yang sudah dicek |
| Memberi umpan balik atas jawaban siswa (misalnya analisis kasus, esai singkat) | AI (LLM) dengan rubrik dari dosen | Jawaban terbuka tidak bisa dinilai dengan kunci jawaban biasa |
| Menilai jawaban yang punya kunci (hitungan, jurnal akuntansi) | Kode | Pasti dan konsisten |
| Menjadi persona kakak tingkat dan alumni | AI (LLM) dengan RAG atas transkrip wawancara nyata | Percakapan natural, tapi isinya bersandar pada cerita asli |
| Membaca refleksi siswa ("aku capek banget ngerjain ini, tapi seru") | AI (LLM) | Siswa menulis atau bicara bebas; perasaan perlu dipahami dari bahasa sehari-hari |
| Menghitung Cermin Minat (nikmat, kuasai, menguras energi) | Kode, dari skor yang sudah terstruktur | Harus bisa dijelaskan ke siswa dan guru BK: "skor tinggi karena kamu menyelesaikan 4 dari 4 tugas dan menilainya seru" |
| Merekomendasikan satu jurusan | **Tidak dikerjakan siapa pun** | Bukan peran produk ini. Keputusan ada di siswa |

## Konsep inti dan cara kerja

Alurnya: **pilih, coba, ngobrol, refleksi, cermin**.

1. **Pilih.** Siswa memilih 2–3 jurusan yang sedang dipertimbangkan, termasuk jurusan "pilihan orang tua" kalau ada.
2. **Coba.** Untuk setiap jurusan, ada "Minggu Mencoba" berisi 4–5 misi pendek (15–20 menit per misi), dari yang seru sampai yang membosankan. Misi bisa berupa hitungan, studi kasus, tugas desain, membaca potongan teks kuliah, atau simulasi situasi kerja.
3. **Ngobrol.** Setelah tiap misi, siswa bisa bertanya ke persona kakak tingkat atau alumni: "Kak, semester 3 beneran seberat ini?", "Kerja di konsultan itu sehari-hari ngapain?".
4. **Refleksi.** Setelah setiap misi, siswa menjawab tiga pertanyaan singkat (lewat ketukan atau voice note): seberapa menikmati, seberapa yakin bisa, dan seberapa capek.
5. **Cermin.** Setelah semua jurusan dicoba, Cermin Minat menampilkan perbandingan pengalaman siswa di tiap jurusan, plus ringkasan untuk orang tua dan guru BK.

**Contoh Minggu Mencoba: Teknik Sipil**

| Misi | Isi | Sifat |
| --- | --- | --- |
| 1. Jembatan Kertas | Menghitung beban sederhana pada balok, lalu melihat simulasi apakah balok patah | Seru, hitungan |
| 2. Baca Gambar Kerja | Membaca potongan denah dan menemukan 3 kesalahan ukuran | Teliti |
| 3. Laporan Praktikum | Menulis ulang data uji tekan beton ke format laporan standar | **Membosankan tapi nyata** |
| 4. Rapat di Lapangan | Simulasi menjelaskan keterlambatan proyek ke mandor dan pemilik | Komunikasi |
| 5. Ngobrol Alumni | Tanya jawab dengan persona alumni yang bekerja di kontraktor dan di dinas PU | Gambaran karier |

**Contoh tampilan Cermin Minat untuk Nayla:**

| Jurusan | Menikmati | Merasa bisa | Menguras energi | Catatan dari refleksi |
| --- | --- | --- | --- | --- |
| Kedokteran | Sedang | Tinggi | Tinggi | "Kasusnya menarik, tapi hafalan anatominya bikin capek banget." |
| DKV | Tinggi | Sedang | Rendah | "Nggak kerasa waktu habis pas bikin poster." |
| Arsitektur | Tinggi | Sedang | Sedang | "Suka desainnya, kaget ternyata banyak hitungan struktur." |

Cermin tidak menyimpulkan. Ia memberi pertanyaan untuk direnungkan: "Kamu menilai dirimu mampu di Kedokteran, tapi juga paling lelah di sana. Apa yang membuatmu lelah, dan apakah itu bisa berubah?"

## Fitur

### Inti (MVP)

| Fitur | Apa yang dilakukan | Prioritas |
| --- | --- | --- |
| **Minggu Mencoba** | 4–5 misi per jurusan, dari yang seru sampai yang membosankan. Untuk demo cukup 3 jurusan. | MVP |
| **Umpan Balik Misi** | AI memberi umpan balik atas jawaban terbuka berdasarkan rubrik; kode menilai jawaban berkunci. | MVP |
| **Ngobrol Kakak Tingkat** | Persona kakak tingkat dan alumni yang menjawab berdasarkan transkrip wawancara nyata, lengkap dengan rujukan ceritanya. | MVP (momen wow demo) |
| **Refleksi Singkat** | Tiga pertanyaan setelah tiap misi, bisa lewat ketukan atau voice note. | MVP |
| **Cermin Minat** | Perbandingan pengalaman antar jurusan, plus pertanyaan reflektif (bukan rekomendasi). | MVP |

### Unggulan

| Fitur | Apa yang dilakukan | Kenapa keren | Prioritas |
| --- | --- | --- | --- |
| **Ringkasan untuk Orang Tua** | Satu halaman dalam bahasa sederhana: apa yang anak coba, nikmati, dan kuasai, plus pertanyaan untuk diskusi keluarga. | Diskusi keluarga berangkat dari pengalaman anak, bukan asumsi. | MVP |
| **Mode Guru BK** | Ringkasan Cermin Minat setiap siswa (dengan izin siswa) sebelum sesi konseling. | Waktu konseling yang sedikit jadi lebih bermakna. | Kalau sempat |
| **Jalur Lain** | Untuk setiap jurusan, tampilkan juga jalur alternatif: D3/D4 vokasi, kursus, atau kerja langsung. | Kuliah S1 bukan satu-satunya jalan, terutama untuk siswa SMK. | Kalau sempat |
| **Coba Bareng** | Dua sahabat mencoba misi yang sama, lalu membandingkan Cermin masing-masing. | Mengurangi "ikut-ikutan teman", karena terlihat bahwa pengalaman mereka ternyata berbeda. | Setelah MVP |

### Lanjutan (setelah hackathon)

| Fitur | Apa yang dilakukan | Prioritas |
| --- | --- | --- |
| **Perpustakaan Jurusan Komunitas** | Mahasiswa dari berbagai kampus menyumbang misi dan cerita untuk jurusannya, dikurasi dosen. | Jangka panjang |
| **Kunjungan Virtual** | Rekaman 360° laboratorium, studio, dan lokasi kerja. | Jangka panjang |
| **Pelacakan Lanjutan** | Dengan izin, menanyakan kembali setelah satu tahun kuliah: apakah pengalaman di Coba Jurusan sesuai kenyataan? Data ini memperbaiki misi. | Jangka panjang |

## Alur pengguna

**Siswa:** pilih 2–3 jurusan → kerjakan misi di tiap jurusan (bisa dicicil seminggu) → ngobrol dengan persona kakak tingkat → isi refleksi singkat → lihat Cermin Minat → bagikan ringkasan ke orang tua atau guru BK.

**Orang tua:** terima tautan ringkasan dari anak → baca apa yang dicoba dan dirasakan anak → diskusi dengan anak memakai pertanyaan yang disarankan.

**Guru BK:** buka daftar siswa yang memberi izin → baca Cermin Minat sebelum sesi → gunakan untuk konseling.

## Rencana teknologi

| Lapis | Pilihan utama | Alternatif | Fungsi |
| --- | --- | --- | --- |
| Frontend | Next.js + Tailwind, PWA | Flutter | Misi interaktif, chat, Cermin Minat |
| Bank misi | JSON terstruktur per jurusan (misi, rubrik, kunci jawaban), disusun manual dan dicek | CMS ringan (Supabase table) | Konten yang akurat dan bisa diaudit |
| Penilaian | Kode untuk jawaban berkunci; LLM dengan rubrik untuk jawaban terbuka | — | Umpan balik misi |
| Persona kakak tingkat | LLM dengan RAG atas transkrip wawancara (dengan izin), menampilkan rujukan cerita | Daftar FAQ statis | Percakapan yang bersandar pada pengalaman nyata |
| Refleksi | Skala ketuk + STT Whisper untuk voice note + LLM untuk menyarikan perasaan | Formulir teks | Data refleksi terstruktur |
| Cermin Minat | Fungsi Python yang menggabungkan skor misi dan refleksi | — | Perbandingan yang bisa dijelaskan |
| Simulasi kecil (misalnya jembatan kertas) | Canvas/JS sederhana | Video pendek | Momen "seru" dalam misi |
| Database | Supabase | Firebase | Profil, progres, izin berbagi |
| Deploy | Vercel | — | Link demo untuk juri |

**Data untuk demo:** siapkan 3 jurusan dengan 4–5 misi masing-masing (misalnya Teknik Sipil, DKV, dan Kedokteran atau Akuntansi). Wawancarai 2–3 mahasiswa dan 1 alumni per jurusan (15 menit cukup) sebagai sumber persona. Minta satu dosen atau mahasiswa tingkat akhir dari tiap jurusan mengecek misinya.

**Akurasi konten:** misi dan rubrik dicek manusia sebelum dipakai. Persona tidak boleh mengarang fakta di luar transkrip. Kalau ditanya hal yang tidak ada di sumber, persona menjawab "Aku nggak punya ceritanya, coba tanya ke kampus langsung".

## Prinsip human-centered, etika, dan keamanan

- **Bukan vonis.** Tidak ada label "kamu cocok jurusan X" atau "kamu tidak berbakat di Y". Yang ditampilkan adalah pengalaman siswa sendiri, dengan pertanyaan reflektif.
- **Melawan stereotip.** Misi dan persona tidak boleh mengaitkan jurusan dengan gender, asal daerah, atau latar ekonomi. Persona dipilih beragam (perempuan di Teknik, laki-laki di Keperawatan, alumni dari daerah).
- **Jujur tentang sisi membosankan.** Setiap jurusan wajib memuat misi "tidak glamor", supaya siswa tidak memilih berdasarkan citra yang dilebih-lebihkan.
- **Siswa memegang datanya.** Ringkasan hanya dibagikan ke orang tua atau guru BK kalau siswa memilih membagikannya. Refleksi pribadi tetap privat.
- **Tidak menambah tekanan.** Bahasanya menenangkan: "Bingung itu wajar. Tujuan di sini bukan langsung yakin, tapi lebih kenal dirimu."
- **Bukan pengganti guru BK.** Coba Jurusan menyiapkan bahan, guru BK yang mendampingi.

## Metrik keberhasilan

**Saat hackathon:**

- **Akurasi konten:** satu dosen atau mahasiswa tingkat akhir per jurusan menilai apakah misi mewakili kuliah sebenarnya (target ≥ 4 dari 5).
- **Uji pengguna:** 10–15 siswa kelas 12 mencoba minimal 2 jurusan. Ukur apakah mereka menemukan hal yang mengejutkan (target ≥ 70% menyebut minimal satu hal yang tidak mereka duga).
- **Perubahan keyakinan:** bandingkan keyakinan siswa sebelum dan sesudah mencoba (naik, turun, atau berubah pilihan). Yang dicari bukan "semua yakin", tapi "keyakinan berbasis pengalaman".
- **Kegunaan ringkasan:** 3–5 orang tua atau guru BK menilai apakah ringkasan membantu diskusi.

**Setelah peluncuran:**

- Jumlah siswa yang mencoba minimal 2 jurusan
- Persentase siswa yang membagikan ringkasan ke orang tua atau guru BK
- Survei satu tahun kemudian: seberapa sesuai pengalaman di Coba Jurusan dengan kuliah sebenarnya
- Jumlah misi dan cerita yang disumbangkan mahasiswa dan dosen

## Scope hackathon dan skenario demo

Final Hackvidia berlangsung 24 jam, dengan pitch dan demo 5 menit. Yang wajib jadi: 3 jurusan dengan misi lengkap, persona kakak tingkat, refleksi, dan Cermin Minat.

- **Wajib:** Minggu Mencoba (3 jurusan × 4–5 misi), Umpan Balik Misi, Ngobrol Kakak Tingkat, Refleksi Singkat, Cermin Minat, Ringkasan untuk Orang Tua.
- **Kalau sempat:** Mode Guru BK, Jalur Lain.
- **Tidak dikerjakan:** Coba Bareng, Perpustakaan Jurusan Komunitas, Kunjungan Virtual.

**Pembagian tim (contoh 4 orang):** frontend dan misi interaktif; penilaian, rubrik, dan Cermin Minat; persona RAG dan wawancara mahasiswa; riset konten jurusan, validasi dosen, dan pitch.

**Skenario demo 5 menit:**

1. **Hook (30 detik):** "Tahun ini, lebih dari 800 ribu siswa mendaftar SNBT. Berapa dari mereka yang pernah benar-benar mencoba jurusan yang mereka pilih?"
2. **Kenalan dengan Nayla (30 detik):** disuruh masuk Kedokteran, diam-diam suka menggambar.
3. **Misi live (75 detik):** juri mencoba satu misi singkat, misalnya Jembatan Kertas, lalu satu misi "membosankan" dari jurusan lain. Umpan balik muncul.
4. **Ngobrol Kakak Tingkat (45 detik):** tanya "Kak, semester 3 Kedokteran beneran seberat itu?". Persona menjawab dengan rujukan cerita asli.
5. **Cermin Minat (45 detik):** tampilkan perbandingan tiga jurusan Nayla dan pertanyaan reflektifnya, lalu ringkasan untuk orang tua.
6. **Dampak dan bisnis (75 detik):** hasil uji dengan siswa (berapa yang menemukan hal mengejutkan), kutipan siswa dan guru BK, dan model kerja sama dengan sekolah dan kampus.

**Cadangan:** rekam video demo lengkap, dan siapkan akun demo yang sudah menyelesaikan semua misi.

## Lean Canvas ringkas

| Komponen | Isi |
| --- | --- |
| Problem | Siswa memilih jurusan tanpa pernah mencoba isinya; tes minat bakat berbasis jawaban tentang diri sendiri; guru BK terlalu sedikit; diskusi keluarga berbasis asumsi |
| Customer Segments | Siswa kelas 11–12 SMA/SMK/MA (pengguna); sekolah dan guru BK; orang tua; kampus (untuk promosi jurusan yang jujur) |
| Unique Value Proposition | Coba dulu kerjaannya sebelum memilih jurusan, lalu bawa hasilnya ke diskusi dengan orang tua |
| Solution | Minggu Mencoba, Ngobrol Kakak Tingkat, Refleksi Singkat, Cermin Minat, Ringkasan untuk Orang Tua |
| Channels | Guru BK dan sekolah, komunitas persiapan SNBT, OSIS, kampus (*open house* virtual), media sosial siswa |
| Revenue Streams | Gratis untuk siswa; lisensi sekolah (Mode Guru BK); kemitraan kampus untuk "jurusan unggulan" dengan konten yang tetap jujur; kemitraan bimbel |
| Cost Structure | LLM per sesi, penyusunan dan validasi konten jurusan, wawancara mahasiswa, hosting |
| Key Metrics | Siswa yang mencoba ≥ 2 jurusan, ringkasan yang dibagikan, kesesuaian dengan pengalaman kuliah setelah satu tahun |
| Unfair Advantage | Bank misi dan cerita jurusan yang dikurasi dosen dan mahasiswa, yang makin kaya seiring sumbangan komunitas |

## Pertanyaan terbuka untuk diskusi

- [ ] **Nama produk:** "Coba Jurusan", "Jurusan Bayangan", atau "Seminggu Jadi Mahasiswa"?
- [ ] **Jurusan untuk demo:** pilih 3 jurusan yang kontras dan mudah divalidasi oleh tim (misalnya Teknik Sipil, DKV, Akuntansi). Apakah perlu satu jurusan yang sering jadi "pilihan orang tua", seperti Kedokteran?
- [ ] **Sumber persona:** siapa saja mahasiswa dan alumni yang bisa diwawancarai sebelum 6 Desember?
- [ ] **Siapa pembayar:** sekolah (lisensi guru BK) atau kampus (promosi)? Kalau kampus, bagaimana menjaga supaya kontennya tetap jujur?
- [ ] **Siswa SMK:** apakah fokus juga ke jalur kerja dan vokasi, atau hanya jurusan kuliah?

## Sumber

- [Lolos SNBP 2026, Ini Tahapan Wajib Sebelum Masuk Kuliah](https://kabar24.bisnis.com/read/20260404/79/1964232/lolos-snbp-2026-ini-tahapan-wajib-sebelum-masuk-kuliah) — Bisnis.com
- [Hanya 29,42 Persen dari Total Pendaftar, 256.369 Calon Mahasiswa Diterima SNBT 2026](https://www.jawapos.com/pendidikan/2605250285/hanya-2942-persen-dari-total-pendaftar-256369-calon-mahasiswa-diterima-snbt-2026) — JawaPos
- [Hasil SNBP 2026 Resmi Diumumkan, Kemdiktisaintek Perkuat Jaminan KIP Kuliah](https://kemdiktisaintek.go.id/news/article/hasil-snbp-2026-resmi-diumumkan-kemdiktisaintek-perkuat-jaminan-kip-kuliah) — Kemdiktisaintek
- [Penyebab Fenomena Salah Jurusan](https://www.goodnewsfromindonesia.id/2022/04/01/penyebab-fenomena-salah-jurusan) — Good News From Indonesia
- [Fenomena Salah Jurusan terhadap Studi Mahasiswa](https://ejournal.unma.ac.id/index.php/dm/article/download/12231/6365/58589) — Jurnal UNMA
- [Implementasi Layanan Bimbingan dan Konseling](https://journal2.um.ac.id/index.php/jamp/article/download/62157/15683) — Jurnal Universitas Negeri Malang
- [Disdikbud Kaltim Beri Penguatan Kapasitas Guru BK Jenjang SMA](https://kaltim.antaranews.com/berita/216093/disdikbud-kaltim-beri-penguatan-kapasitas-guru-bk-jenjang-sma) — Antara Kaltim
- [Disdikbud Kaltim Respons Kekurangan Guru BK](https://rri.co.id/samarinda/regional/2510838/disdikbud-kaltim-respons-kekurangan-guru-bk-dan-agama-di-sekolah-rakyat) — RRI
- [Persoalan Salah Jurusan Mahasiswa](https://binus.ac.id/character-building/?p=7425) — Binus
- [Rencanamu Hadirkan Layanan Persiapan Kuliah Gratis](https://www.industry.co.id/read/75581/rencanamu-hadirkan-layanan-persiapan-kuliah-gratis) — Industry.co.id
