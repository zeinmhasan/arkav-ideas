# PRD — Bertahan Kuliah

Nov 23, 2026 · ide tambahan, disusun dari Guidebook Hackvidia 11.0

## Ringkasan

**Bertahan Kuliah** adalah pendamping untuk mahasiswa yang terancam berhenti kuliah karena biaya. Mahasiswa cukup bercerita tentang kondisinya, misalnya "Ayah baru kena PHK, UKT semester depan Rp6 juta, saya nggak tahu harus gimana". AI lalu memetakan **semua jalan yang masih terbuka**: banding UKT, cicilan atau penundaan, bantuan pemerintah, beasiswa kampus dan swasta, kerja paruh waktu di kampus, sampai cuti sebagai pilihan terakhir. Setiap jalan disertai syarat, tenggat, dan berkas yang perlu disiapkan. Untuk kampus, ada dasbor yang membantu bagian kemahasiswaan menemukan mahasiswa yang butuh bantuan *sebelum* mereka menghilang.

**One-liner:** *Jangan berhenti hanya karena tidak tahu masih ada jalan.*

**Konsep inti:** Banyak mahasiswa berhenti bukan karena benar-benar tidak ada jalan, tapi karena informasinya tersebar, tenggatnya terlewat, berkasnya membingungkan, dan mereka malu bertanya. Bertahan Kuliah mengubah "aku nggak sanggup bayar" menjadi daftar langkah konkret dengan tanggal.

**Subtema Hackvidia:** utama *AI for Inclusive Access* (akses pendidikan tinggi bagi mahasiswa dari keluarga rentan). Pendukungnya *AI for Daily Living* (perencanaan keuangan semester) dan *AI for Learning & Self-Growth* (menjaga mahasiswa tetap kuliah).

**Prinsip desain:** Bertahan Kuliah membantu mahasiswa menyampaikan kondisi **yang sebenarnya** dengan lebih jelas dan lengkap. Ia tidak pernah membantu memalsukan dokumen atau melebih-lebihkan kondisi. Keputusan banding UKT dan beasiswa tetap ada di kampus dan pemberi beasiswa.

**Hubungan dengan PRD lain:** Diri Masa Depan berfokus pada keuangan jangka panjang anak muda, dan CareerMirror pada kesiapan kerja. Bertahan Kuliah mengisi tahap sebelumnya: memastikan mahasiswa bisa lulus dulu.

## Masalah

- **Ratusan ribu mahasiswa berhenti setiap tahun.** Sepanjang 2025, ada 289.670 mahasiswa Indonesia yang putus kuliah, naik 2,62% dibanding 2024 ([Databoks Katadata](https://databoks.katadata.co.id/pendidikan/statistik/6a1e312edea6e/mahasiswa-putus-kuliah-di-ri-terbanyak-dari-ilmu-ekonomi-pada-2025)).
- **Biaya jadi faktor yang paling sering disebut.** Penyebab putus kuliah beragam (psikologis, akademik, pekerjaan), tapi masalah finansial disebut paling dominan ([MomsMoney/Kontan](https://momsmoney.kontan.co.id/news/peran-perguruan-tinggi-untuk-mengurangi-tingkat-mahasiswa-putus-kuliah)). JPPI juga menyoroti mahasiswa dari keluarga ekonomi menengah yang merasa sangat terbebani UKT, sehingga banyak yang putus kuliah di tengah jalan ([NU Online](https://www.nu.or.id/nasional/jppi-sesalkan-pembatalan-kenaikan-ukt-tak-dibarengi-pengembalian-status-ptnbh-ke-ptn-5yr7J)).
- **Masalahnya bahkan dimulai sebelum kuliah.** Sekitar 60 ribu calon mahasiswa baru yang lolos seleksi tidak melakukan registrasi ulang. Angka ini berasal dari evaluasi penerimaan 2025 ([Metro TV](https://www.metrotvnews.com/read/bD2Cwjpr-mendiktisaintek-informasi-60-ribu-mahasiswa-undur-diri-tidak-tepat)), dan DPR mempertanyakan apakah UKT yang tinggi menjadi penyebab utamanya ([DPR RI](https://emedia.dpr.go.id/news/2026/06/30/fenomena-60-ribu-mahasiswa-tak-registrasi-ulang-jadi-sorotan-komisi-x-dpr)).
- **Bantuannya ada, tapi jalannya rumit.** Mulai 2026, KIP Kuliah tidak lagi memakai kuota per kampus: calon mahasiswa yang lolos seleksi nasional dan masuk desil 1–4 dipastikan dapat ([GNFI](https://www.goodnewsfromindonesia.id/short/cek-aturan-baru-kip-kuliah-2026-tidak-ada-lagi-batasan-kuota)). PIP Dikti masih bisa diberikan kepada mahasiswa yang tidak masuk desil rentan, asalkan penghasilan orang tuanya tidak melebihi UMP ([Kontan](https://industri.kontan.co.id/news/salah-kaprah-bansos-dan-pip-pengamat-jelaskan-fungsi-dtsen-bps)). Banyak kampus juga membuka sanggah UKT ([Metro TV](https://www.metrotvnews.com/play/NgxClLzw-ketika-biaya-kuliah-menjadi-tantangan-mahasiswa)). Masalahnya, setiap jalur punya syarat, tenggat, dan berkas yang berbeda-beda.
- **Kampus belum punya data penyebabnya.** Saat DPR menanyakan berapa banyak calon mahasiswa yang batal kuliah karena miskin atau karena KIP Kuliah-nya ditolak, pemerintah belum punya jawaban berbasis data ([Mojok](https://mojok.co/tajuk/mengapa-calon-mahasiswa-ptn-banyak-yang-mengundurkan-diri/)).
- **Saat terdesak, mahasiswa bisa mengambil jalan yang berbahaya.** Mahasiswa ITB pernah dihebohkan dengan tawaran pembiayaan kuliah lewat pinjaman online ([Antara](https://megapolitan.antaranews.com/berita/280959/mencari-skema-pendanaan-pendidikan-tinggi)).

Intinya, bantuan tersedia di banyak tempat, tapi mahasiswa harus mencarinya sendiri, di saat paling tertekan, dan sering baru tahu setelah tenggatnya lewat.

## Target pengguna

| Persona | Situasi | Yang ia butuhkan |
| --- | --- | --- |
| **Raka, 20, semester 3, PTN** | Ayahnya baru kena PHK. UKT-nya golongan 5 karena ditetapkan saat kondisi keluarga masih baik. Tidak tahu bahwa UKT bisa dibanding di tengah masa studi. | Tahu bahwa ada jalan, apa syaratnya, dan kapan batasnya. |
| **Sari, 19, mahasiswa baru, rantau** | Lolos jalur mandiri, UKT dan IPI-nya besar. Keluarganya pedagang tanpa slip gaji, sehingga sulit membuktikan penghasilan. | Bantuan menyusun bukti kondisi ekonomi yang jujur dan meyakinkan tanpa slip gaji. |
| **Dimas, 22, semester 7** | Kuliah sambil kerja di kafe. Nilainya turun, beasiswanya terancam dicabut karena IPK di bawah syarat. | Peringatan dini sebelum beasiswa dicabut, dan rencana keuangan cadangan. |
| **Bu Ratih, 45, staf kemahasiswaan** | Baru tahu mahasiswa bermasalah saat namanya muncul di daftar "belum bayar" atau "tidak aktif". | Daftar mahasiswa yang butuh bantuan lebih awal, dan cara cepat mengarahkannya ke jalur bantuan yang tepat. |

## Produk serupa dan pembeda

| Yang sudah ada | Apa yang dilakukan | Yang belum ada |
| --- | --- | --- |
| Situs dan kanal info beasiswa (INDBeasiswa, grup Telegram, dsb.) | Mengumpulkan pengumuman beasiswa dari berbagai sumber ([INDBeasiswa](https://indbeasiswa.com/?paged=17)) | Tidak dipersonalisasi; tidak mencakup banding UKT, cicilan, atau bantuan pemerintah; tidak membantu menyiapkan berkas |
| Portal KIP Kuliah dan aplikasi Cek Bansos | Pendaftaran dan cek status bantuan pemerintah | Satu jalur per portal; tidak memberi gambaran semua pilihan |
| Bagian kemahasiswaan kampus | Menangani sanggah UKT dan beasiswa kampus | Reaktif; mahasiswa harus datang sendiri, dan banyak yang malu |
| Aplikasi mahasiswa (SejutaCita, dsb.) | Info karier, beasiswa, dan komunitas | Tidak fokus pada mahasiswa yang sedang terancam berhenti |

**Lima pembeda Bertahan Kuliah:**

1. **Semua jalan dalam satu peta.** Banding UKT, cicilan, KIP Kuliah, PIP Dikti, beasiswa kampus dan swasta, kerja kampus, dan cuti, diurutkan sesuai kondisi dan tenggat masing-masing mahasiswa.
2. **Aturan kampus yang dibaca AI.** Peraturan rektor dan panduan UKT setiap kampus (PDF panjang dan membingungkan) diubah menjadi aturan yang bisa dicek: apakah boleh banding di tengah masa studi, dokumen apa saja, sampai kapan.
3. **Berkas yang jujur dan lengkap.** AI membantu mengecek kelengkapan dan konsistensi berkas, serta menyusun penjelasan kondisi ekonomi, termasuk untuk keluarga tanpa slip gaji.
4. **Peringatan dini dua arah.** Mahasiswa diingatkan sebelum tenggat lewat atau syarat beasiswa terancam. Kampus melihat sinyal risiko dari mahasiswa yang sudah memberi izin.
5. **Menangkal jalan pintas berbahaya.** Saat mahasiswa menyebut pinjol, Bertahan Kuliah menjelaskan risikonya dan menunjukkan pilihan lain yang masih terbuka.

## Kapan AI dipakai, dan kapan tidak

| Tugas | Dikerjakan oleh | Alasan |
| --- | --- | --- |
| Memahami cerita kondisi mahasiswa (teks atau voice note) | AI (LLM + STT) | Mahasiswa bercerita dengan bahasanya sendiri, tidak dalam format formulir |
| Membaca peraturan UKT dan pengumuman beasiswa (PDF, poster) | AI (LLM + OCR) | Setiap kampus dan pemberi beasiswa punya format berbeda |
| Menentukan apakah mahasiswa memenuhi syarat suatu jalur | Kode (aturan terstruktur hasil ekstraksi, dicek manusia) | Keputusan kelayakan harus konsisten dan bisa dijelaskan |
| Menghitung kekurangan dana sampai UKT berikutnya | Kode | Aritmetika biasa |
| Membaca dokumen pendukung (slip gaji, tagihan listrik, KK, surat PHK) | AI (OCR + ekstraksi) | Dokumen berupa foto dengan kualitas beragam |
| Mengecek konsistensi antar dokumen | Kode + AI | Kode membandingkan angka; AI menjelaskan ketidaksesuaian dalam bahasa sederhana |
| Menyusun draf surat permohonan dan penjelasan kondisi | AI (LLM) | Mahasiswa sering kesulitan menulis surat formal yang jelas |
| Skor risiko di dasbor kampus | Aturan berbobot sederhana | Harus bisa dijelaskan ke staf kampus: "berisiko karena belum bayar dan beasiswanya akan berakhir" |

## Konsep inti dan cara kerja

Alurnya: **cerita, peta jalan, siapkan, ingatkan, sambungkan**.

1. **Cerita.** Mahasiswa menjelaskan situasinya lewat chat atau voice note. AI mengubahnya menjadi profil terstruktur: kampus, semester, golongan UKT, kondisi ekonomi keluarga, perubahan terbaru (misalnya PHK), IPK, dan beasiswa yang sedang diterima.
2. **Peta jalan.** Sistem mencocokkan profil dengan basis aturan (kampus, pemerintah, pemberi beasiswa), lalu menampilkan **Rute Bertahan**: jalur yang mungkin, diurutkan berdasarkan peluang dan tenggat terdekat.
3. **Siapkan.** Untuk jalur yang dipilih, Bertahan Kuliah membuat daftar berkas, mengecek foto dokumen yang diunggah, dan membantu menyusun surat permohonan.
4. **Ingatkan.** Tenggat, jadwal pembayaran, dan syarat beasiswa (misalnya IPK minimal) dipantau. Mahasiswa diingatkan sebelum terlambat.
5. **Sambungkan.** Kalau mahasiswa memberi izin, kasusnya diteruskan ke bagian kemahasiswaan lengkap dengan ringkasan dan berkas, sehingga mahasiswa tidak perlu mengulang cerita dari awal.

**Contoh Rute Bertahan untuk Raka:**

| Urutan | Jalur | Kenapa cocok | Tenggat | Status |
| --- | --- | --- | --- | --- |
| 1 | Banding penurunan UKT | Kondisi ekonomi berubah (ayah kena PHK); peraturan kampusnya membolehkan banding di tengah masa studi | 14 hari sebelum masa pembayaran | Berkas 3 dari 5 lengkap |
| 2 | Cicilan UKT | Bisa diajukan bersamaan dengan banding, untuk berjaga-jaga | Sebelum tagihan terbit | Belum diajukan |
| 3 | Beasiswa kampus untuk keluarga terdampak PHK | Syarat cocok, IPK memenuhi | 30 Des 2026 | Perlu esai |
| 4 | PIP Dikti | Perlu dicek apakah penghasilan orang tua saat ini di bawah UMP | Mengikuti jadwal kampus | Perlu konfirmasi |
| 5 | Kerja paruh waktu di kampus | Asisten lab di prodinya sedang buka | Rolling | Opsional |

## Fitur

### Inti (MVP)

| Fitur | Apa yang dilakukan | Prioritas |
| --- | --- | --- |
| **Cerita Dulu** | Wawancara singkat lewat chat atau voice note, lalu diubah menjadi profil terstruktur. | MVP |
| **Rute Bertahan** | Peta semua jalur yang mungkin, diurutkan berdasarkan peluang dan tenggat, dengan alasan kenapa cocok. | MVP (momen wow demo) |
| **Pembaca Aturan** | Unggah peraturan UKT atau pengumuman beasiswa (PDF atau poster), lalu AI mengekstrak syarat, dokumen, dan tenggat menjadi aturan terstruktur. | MVP |
| **Cek Berkas** | Foto dokumen pendukung dicek kelengkapan dan konsistensinya, lalu ditampilkan daftar yang masih kurang. | MVP |
| **Draf Surat** | Menyusun surat permohonan banding atau cicilan UKT dan penjelasan kondisi ekonomi berdasarkan data yang sudah diverifikasi mahasiswa. | MVP |

### Unggulan

| Fitur | Apa yang dilakukan | Kenapa keren | Prioritas |
| --- | --- | --- | --- |
| **Rencana Semester** | Proyeksi pemasukan dan pengeluaran sampai tagihan UKT berikutnya, dengan peringatan kalau akan kekurangan. | Masalah terlihat berbulan-bulan sebelumnya, bukan seminggu sebelum bayar. | MVP |
| **Penjaga Beasiswa** | Memantau syarat beasiswa yang sedang diterima (IPK, SKS, laporan) dan memberi peringatan sebelum terancam dicabut. | Mencegah kehilangan beasiswa karena hal yang sebenarnya bisa dicegah. | Kalau sempat |
| **Bukti Tanpa Slip Gaji** | Panduan menyusun bukti penghasilan untuk keluarga pekerja informal: catatan usaha, surat keterangan, foto tempat usaha, sesuai yang diterima kampus. | Menjawab masalah yang paling sering membuat pekerja informal kesulitan. | Kalau sempat |
| **Dasbor Kampus** | Daftar mahasiswa yang memberi izin dan sedang berisiko, beserta alasannya dan jalur bantuan yang disarankan. | Kampus bisa menjemput bola. Ini juga kunci model bisnis. | MVP (versi sederhana) |

### Lanjutan (setelah hackathon)

| Fitur | Apa yang dilakukan | Prioritas |
| --- | --- | --- |
| **Mode Calon Mahasiswa** | Membantu siswa SMA memperkirakan biaya dan menyiapkan berkas sebelum pengumuman, supaya tidak mundur saat registrasi ulang. | Setelah MVP |
| **Basis Aturan Bersama** | Kumpulan aturan UKT dan beasiswa dari banyak kampus yang diperbarui bersama oleh komunitas mahasiswa. | Jangka panjang |
| **Laporan Kebijakan** | Data agregat anonim tentang penyebab mahasiswa terancam berhenti, untuk kampus dan pembuat kebijakan. | Jangka panjang |

## Alur pengguna

**Mahasiswa:** buka aplikasi atau WhatsApp → ceritakan kondisi → lihat Rute Bertahan → pilih jalur → unggah berkas dan dapatkan draf surat → terima pengingat tenggat → (opsional) teruskan kasus ke kemahasiswaan.

**Staf kemahasiswaan:** buka dasbor → lihat daftar mahasiswa berisiko yang sudah memberi izin → baca ringkasan kasus → hubungi mahasiswa atau arahkan ke bantuan yang tepat.

## Rencana teknologi

| Lapis | Pilihan utama | Alternatif | Fungsi |
| --- | --- | --- | --- |
| Frontend | Next.js + Tailwind, PWA | Flutter | Chat, Rute Bertahan, unggah berkas, dasbor kampus |
| Wawancara | LLM dengan output JSON (profil terstruktur) + STT Whisper | Formulir bertahap | Mengubah cerita menjadi data |
| Pembaca aturan | LLM + OCR untuk PDF dan poster, output berupa skema aturan (syarat, dokumen, tenggat) | Input manual untuk 2–3 kampus demo | Basis aturan yang bisa dicek kode |
| Mesin kelayakan | Fungsi Python yang mencocokkan profil dengan aturan | — | Rute Bertahan yang konsisten dan bisa dijelaskan |
| Cek berkas | OCR (model vision) + aturan konsistensi | — | Daftar kekurangan dan ketidaksesuaian |
| Database | Supabase (Postgres + storage terenkripsi) | Firebase | Profil, berkas, pengingat |
| Pengingat | Cron job + notifikasi WhatsApp atau email | Notifikasi web | Tenggat dan peringatan |
| Deploy | Vercel + Railway | — | Link demo untuk juri |

**Data untuk demo:** kumpulkan peraturan UKT dan panduan beasiswa resmi dari 2–3 kampus (biasanya tersedia publik), pengumuman 10–20 beasiswa nyata, dan buat 3–5 profil mahasiswa simulasi berdasarkan wawancara dengan teman. Gunakan dokumen contoh, bukan dokumen asli orang lain.

**Akurasi aturan:** setiap aturan hasil ekstraksi AI menyimpan kutipan dan nomor halaman sumbernya. Untuk demo, aturan kampus dicek manual oleh tim. Di produk nyata, aturan dicek oleh staf kampus atau relawan mahasiswa sebelum dipakai.

## Prinsip human-centered, etika, dan keamanan

- **Jujur, bukan akal-akalan.** Bertahan Kuliah tidak pernah membuat dokumen palsu, tidak menyarankan melebih-lebihkan kondisi, dan menjelaskan konsekuensi memberikan data tidak benar. Tujuannya membantu kondisi yang sebenarnya tersampaikan dengan jelas.
- **Tidak menjanjikan hasil.** Setiap jalur ditampilkan sebagai "peluang", bukan jaminan. Keputusan tetap di kampus dan pemberi beasiswa.
- **Mengurangi rasa malu.** Bahasanya hangat dan tidak menghakimi: "Banyak mahasiswa mengalami ini, dan ada jalannya." Mahasiswa bisa mengeksplorasi pilihan tanpa ada yang tahu.
- **Data sangat sensitif.** Dokumen keluarga disimpan terenkripsi dan bisa dihapus kapan saja. Dasbor kampus hanya menampilkan mahasiswa yang secara eksplisit memberi izin, dan izin bisa dicabut.
- **Bukan alat penghakiman kampus.** Skor risiko hanya dipakai untuk menawarkan bantuan, tidak boleh dipakai untuk sanksi akademik atau penilaian.
- **Waspada jalan pintas berbahaya.** Saat mahasiswa menyebut pinjol atau pinjaman tidak resmi, AI menjelaskan risikonya dan menunjukkan pilihan lain yang masih terbuka.

## Metrik keberhasilan

**Saat hackathon:**

- **Akurasi ekstraksi aturan:** dari peraturan UKT dan 10–20 pengumuman beasiswa, persentase syarat, dokumen, dan tenggat yang diekstrak benar (target ≥ 90%).
- **Akurasi Rute Bertahan:** untuk 5 profil simulasi, bandingkan rute yang dihasilkan dengan penilaian staf kemahasiswaan atau mahasiswa senior yang paham aturan.
- **Uji kegunaan:** 5–10 mahasiswa mencoba alur dari cerita sampai draf surat. Ukur waktu (target < 15 menit) dan apakah mereka menemukan jalur yang sebelumnya tidak mereka ketahui.
- **Validasi kampus:** satu staf kemahasiswaan menilai apakah dasbor dan ringkasan kasus berguna.

**Setelah peluncuran:**

- Persentase pengguna yang mengajukan setidaknya satu jalur sebelum tenggat
- Persentase pengajuan yang berhasil (banding UKT, beasiswa, cicilan)
- Persentase pengguna yang tetap terdaftar aktif di semester berikutnya
- Waktu dari mahasiswa pertama kali bercerita sampai dihubungi kampus (untuk yang memberi izin)

## Scope hackathon dan skenario demo

Final Hackvidia berlangsung 24 jam, dengan pitch dan demo 5 menit. Yang wajib jadi: satu alur utuh dari cerita sampai Rute Bertahan, berkas, dan draf surat, plus dasbor kampus versi sederhana.

- **Wajib:** Cerita Dulu, Rute Bertahan, Pembaca Aturan (untuk 2–3 kampus demo), Cek Berkas, Draf Surat, Rencana Semester, Dasbor Kampus sederhana.
- **Kalau sempat:** Penjaga Beasiswa, Bukti Tanpa Slip Gaji, pengingat lewat WhatsApp.
- **Tidak dikerjakan:** Mode Calon Mahasiswa, Basis Aturan Bersama, Laporan Kebijakan.

**Pembagian tim (contoh 4 orang):** frontend dan alur chat; Pembaca Aturan dan mesin kelayakan; Cek Berkas, Draf Surat, dan Rencana Semester; riset aturan kampus, wawancara mahasiswa, dan pitch.

**Skenario demo 5 menit:**

1. **Hook (30 detik):** "Tahun lalu, hampir 290 ribu mahasiswa berhenti kuliah. Berapa di antaranya yang sebenarnya masih punya jalan, tapi tidak tahu?"
2. **Cerita (45 detik):** voice note dari persona Raka. Profil terstruktur muncul.
3. **Rute Bertahan (75 detik):** lima jalur muncul, diurutkan dengan alasan dan tenggat. Tunjukkan satu aturan dan kutipan sumbernya dari PDF peraturan kampus.
4. **Pembaca Aturan live (45 detik):** unggah poster beasiswa baru di depan juri. Syarat dan tenggatnya terekstrak, dan Rute Bertahan Raka langsung diperbarui.
5. **Berkas dan surat (45 detik):** unggah foto surat PHK dan KK. Muncul daftar yang masih kurang dan draf surat banding UKT.
6. **Dasbor kampus dan bisnis (60 detik):** tampilan staf kemahasiswaan, hasil uji akurasi, kutipan dari mahasiswa saat uji coba, dan model kerja sama dengan kampus.

**Cadangan:** rekam video demo lengkap, dan simpan hasil ekstraksi aturan kalau API lambat.

## Lean Canvas ringkas

| Komponen | Isi |
| --- | --- |
| Problem | Mahasiswa berhenti kuliah karena biaya, padahal masih ada jalur bantuan yang tidak mereka ketahui; informasi tersebar dan tenggat terlewat; kampus baru tahu setelah terlambat |
| Customer Segments | Mahasiswa dari keluarga rentan dan menengah yang terancam berhenti (pengguna); bagian kemahasiswaan kampus (pembayar); yayasan dan pemberi beasiswa |
| Unique Value Proposition | Semua jalan untuk tetap kuliah dalam satu peta pribadi, lengkap dengan berkas dan tenggat |
| Solution | Cerita Dulu, Rute Bertahan, Pembaca Aturan, Cek Berkas, Draf Surat, Dasbor Kampus |
| Channels | BEM dan himpunan mahasiswa, bagian kemahasiswaan, komunitas penerima beasiswa, guru BK SMA (untuk calon mahasiswa) |
| Revenue Streams | Gratis untuk mahasiswa; lisensi Dasbor Kampus per perguruan tinggi; kemitraan dengan yayasan beasiswa (penyaringan pelamar yang lebih tepat sasaran); hibah program pendidikan |
| Cost Structure | LLM dan OCR per pengguna, hosting dan penyimpanan terenkripsi, pemeliharaan basis aturan, onboarding kampus |
| Key Metrics | Pengajuan sebelum tenggat, tingkat keberhasilan pengajuan, retensi mahasiswa semester berikutnya |
| Unfair Advantage | Basis aturan UKT dan beasiswa terstruktur dari banyak kampus, yang makin lengkap seiring pemakaian |

## Pertanyaan terbuka untuk diskusi

- [ ] **Nama produk:** "Bertahan Kuliah", "Jalan Lain", atau "Tetap Kuliah"?
- [ ] **Kampus demo:** kampus mana yang peraturan UKT dan beasiswanya tersedia publik dan cukup lengkap? Idealnya kampus tim sendiri, supaya bisa divalidasi staf kemahasiswaan.
- [ ] **Siapa pembayar utama?** Kampus (B2B) lebih realistis, tapi apakah kampus mau melihat data mahasiswa yang berisiko berhenti?
- [ ] **Batas privasi dasbor kampus:** data apa yang boleh dilihat kampus, dan bagaimana memastikan mahasiswa benar-benar paham saat memberi izin?
- [ ] **Cakupan jalur:** apakah termasuk kerja paruh waktu dan cuti, atau fokus ke bantuan biaya saja supaya lebih tajam?

## Sumber

- [Mahasiswa Putus Kuliah di RI Terbanyak dari Ilmu Ekonomi pada 2025](https://databoks.katadata.co.id/pendidikan/statistik/6a1e312edea6e/mahasiswa-putus-kuliah-di-ri-terbanyak-dari-ilmu-ekonomi-pada-2025) — Databoks Katadata
- [Peran Perguruan Tinggi untuk Mengurangi Tingkat Mahasiswa Putus Kuliah](https://momsmoney.kontan.co.id/news/peran-perguruan-tinggi-untuk-mengurangi-tingkat-mahasiswa-putus-kuliah) — MomsMoney/Kontan
- [JPPI Sesalkan Pembatalan Kenaikan UKT Tak Dibarengi Pengembalian Status PTNBH ke PTN](https://www.nu.or.id/nasional/jppi-sesalkan-pembatalan-kenaikan-ukt-tak-dibarengi-pengembalian-status-ptnbh-ke-ptn-5yr7J) — NU Online
- [Mendiktisaintek: Informasi 60 Ribu Mahasiswa Undur Diri Tidak Tepat](https://www.metrotvnews.com/read/bD2Cwjpr-mendiktisaintek-informasi-60-ribu-mahasiswa-undur-diri-tidak-tepat) — Metro TV
- [Fenomena 60 Ribu Mahasiswa Tak Registrasi Ulang Jadi Sorotan Komisi X DPR](https://emedia.dpr.go.id/news/2026/06/30/fenomena-60-ribu-mahasiswa-tak-registrasi-ulang-jadi-sorotan-komisi-x-dpr) — DPR RI
- [Cek Aturan Baru KIP Kuliah 2026, Tidak Ada Lagi Batasan Kuota](https://www.goodnewsfromindonesia.id/short/cek-aturan-baru-kip-kuliah-2026-tidak-ada-lagi-batasan-kuota) — Good News From Indonesia
- [Salah Kaprah Bansos dan PIP, Pengamat Jelaskan Fungsi DTSEN BPS](https://industri.kontan.co.id/news/salah-kaprah-bansos-dan-pip-pengamat-jelaskan-fungsi-dtsen-bps) — Kontan
- [Ketika Biaya Kuliah Menjadi Tantangan Mahasiswa](https://www.metrotvnews.com/play/NgxClLzw-ketika-biaya-kuliah-menjadi-tantangan-mahasiswa) — Metro TV
- [Mengapa Calon Mahasiswa PTN Banyak yang Mengundurkan Diri](https://mojok.co/tajuk/mengapa-calon-mahasiswa-ptn-banyak-yang-mengundurkan-diri/) — Mojok
- [Mencari Skema Pendanaan Pendidikan Tinggi](https://megapolitan.antaranews.com/berita/280959/mencari-skema-pendanaan-pendidikan-tinggi) — Antara
- [INDBeasiswa](https://indbeasiswa.com/?paged=17) — contoh platform info beasiswa
