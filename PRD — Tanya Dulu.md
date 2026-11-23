# PRD — Tanya Dulu

Nov 23, 2026 · ide tambahan, disusun dari Guidebook Hackvidia 11.0

## Ringkasan

**Tanya Dulu** adalah "teman cek" untuk lansia dan orang tua yang kurang akrab dengan dunia digital. Setiap kali menerima pesan, telepon, tautan, atau file yang mencurigakan, mereka cukup meneruskannya ke Tanya Dulu lewat WhatsApp, atau mengirim voice note seperti "Ini beneran dari bank nggak?". AI menjelaskan dalam bahasa sederhana, bahkan bahasa daerah, apakah ini aman, perlu hati-hati, atau hampir pasti penipuan. AI juga menjelaskan apa yang sebaiknya dilakukan. Kalau risikonya tinggi, anggota keluarga yang ditunjuk ikut diberi tahu.

**One-liner:** *Sebelum transfer, sebelum klik, sebelum kasih kode: tanya dulu.*

**Konsep inti:** Penipuan digital berhasil karena satu hal: korban dibuat panik dan terburu-buru. Tanya Dulu tidak mencoba menjadi filter yang sempurna. Tugasnya memberi **jeda** dan **orang kedua** yang tenang, persis seperti anak atau cucu yang ditanya "ini beneran nggak, Nak?", tapi tersedia 24 jam.

**Subtema Hackvidia:** utama *AI for Inclusive Access* (lansia dan warga dengan literasi digital terbatas). Pendukungnya *AI for Daily Living* (keamanan keuangan sehari-hari) dan *AI for Community Impact* (laporan yang membantu pemblokiran rekening dan nomor penipu).

**Prinsip desain:** Tanya Dulu tidak pernah menyuruh pengguna mentransfer, mengklik, atau memberikan data. Saat ragu, jawabannya selalu condong ke "jangan dulu, cek lewat jalur resmi".

## Masalah

- **Kerugiannya sangat besar dan terus bertambah.** Indonesia Anti-Scam Centre (IASC) mencatat kerugian masyarakat akibat penipuan mencapai Rp9,1 triliun dari 432.637 laporan, dihitung sejak IASC beroperasi hingga 14 Januari 2026 ([Kontan](https://keuangan.kontan.co.id/news/hingga-14-januari-2026-kerugian-masyarakat-akibat-penipuan-scam-rp-91-triliun)). Per akhir Agustus 2026, laporannya sudah mencapai 668.441 ([Katadata](https://katadata.co.id/indepth/telaah/6aa10f4783de1/data-bocor-telepon-spam-melonjak-indonesia-peringkat-dua-dunia-rentan-penipuan)).
- **Percobaan penipuan terjadi setiap minggu.** Komdigi menyebut 65% masyarakat Indonesia menerima percobaan penipuan digital setidaknya sekali seminggu, lewat SMS, email, WhatsApp, dan media sosial ([Bisnis.com](https://teknologi.bisnis.com/read/20260506/84/1971823/komdigi-ungkap-65-orang-indonesia-terima-percobaan-scam-lewat-sms-hingga-dm)).
- **Lansia jadi sasaran utama.** Meta menyebut lansia sebagai salah satu sasaran utama penipu, sampai merilis fitur peringatan khusus di WhatsApp saat berbagi layar dengan nomor asing ([Kompas TV](https://www.kompas.tv/info-publik/683021/fitur-whatsapp-ini-bisa-cegah-orang-tua-jadi-korban-penipuan-share-screen-begini-cara-kerjanya)). Modusnya makin canggih, termasuk memakai AI, *voice cloning*, dan *deepfake* ([Tirto, mengutip Mafindo](https://tirto.id/mafindo-kerugian-masyarakat-akibat-scam-capai-rp91-triliun-hrwa)).
- **Uang yang sudah hilang sulit kembali.** Dari kerugian triliunan rupiah itu, dana yang berhasil diblokir hanya ratusan miliar ([Katadata](https://katadata.co.id/indepth/telaah/6aa10f4783de1/data-bocor-telepon-spam-melonjak-indonesia-peringkat-dua-dunia-rentan-penipuan)). Mencegah jauh lebih efektif daripada memulihkan.

Kanal resmi sudah ada, seperti cekrekening.id, aduannomor.id, dan laporan ke IASC. Masalahnya, kanal-kanal ini dipakai *setelah* curiga atau *setelah* tertipu, dan menuntut pengguna tahu harus mengetik apa dan ke mana. Lansia butuh sesuatu yang lebih sederhana: satu tempat untuk bertanya, dengan cara yang sudah mereka kenal, yaitu meneruskan pesan WhatsApp.

## Target pengguna

| Persona | Situasi | Yang ia butuhkan |
| --- | --- | --- |
| **Bu Har, 64, pensiunan guru** | Sering menerima pesan "paket Anda tertahan" dan "undangan pernikahan" berupa file. Pernah hampir mengirim kode OTP ke orang yang mengaku petugas bank. | Satu tempat untuk bertanya, dengan jawaban jelas dalam bahasa Jawa: "Jangan dibuka, Bu." |
| **Pak Made, 58, pedagang** | Pakai m-banking untuk usaha. Ditelepon "petugas pajak" yang mendesak harus bayar hari ini. | Cara cepat memastikan apakah instansi itu benar-benar menghubungi lewat telepon. |
| **Nisa, 27, anak perantau** | Tinggal jauh dari orang tuanya, dan khawatir mereka tertipu. Tidak bisa selalu mengangkat telepon. | Diberi tahu kalau orang tuanya menerima pesan berisiko tinggi, tanpa harus memantau semua chat mereka. |
| **Pak RT / kader lansia** | Sering ditanya warga lansia soal pesan aneh. | Materi edukasi sederhana dan rekap modus yang sedang marak di lingkungannya. |

## Produk serupa dan pembeda

| Yang sudah ada | Apa yang dilakukan | Yang belum ada |
| --- | --- | --- |
| cekrekening.id dan aduannomor.id (Komdigi), laporan IASC (OJK) | Mengecek atau melaporkan rekening dan nomor yang terindikasi penipuan ([Viva](https://www.viva.co.id/bisnis/1879957-kemkomdigi-ungkap-modus-baru-penipuan-digital)) | Pengguna harus tahu apa yang dicek; tidak menilai isi pesan atau modusnya |
| Fitur keamanan WhatsApp dan Truecaller | Peringatan nomor asing dan identifikasi penelepon spam | Tidak menjelaskan "kenapa ini penipuan" dalam bahasa yang dipahami lansia; tidak melibatkan keluarga |
| Scam checker di aplikasi keuangan (misalnya DANA) | Mengecek keaslian nomor atau akun yang mengatasnamakan aplikasi itu ([detikInet](https://inet.detik.com/security/d-8325514/marak-penipuan-online-ini-cara-praktis-cegah-risikonya-agar-tetap-aman)) | Hanya untuk merek itu sendiri |
| Bertanya ke anak atau cucu | Cara paling efektif sekarang | Tidak selalu tersedia, dan sering terlambat |

**Lima pembeda Tanya Dulu:**

1. **Cukup teruskan pesan.** Tidak perlu memasang aplikasi baru atau belajar menu. Pesan, screenshot, file, tautan, dan voice note bisa dikirim apa adanya.
2. **Menjelaskan, bukan hanya memberi label.** "Ini penipuan karena bank tidak pernah meminta kode OTP lewat WhatsApp" lebih mendidik daripada sekadar "berbahaya".
3. **Suara dan bahasa daerah.** Jawaban bisa berupa voice note dalam bahasa Indonesia, Jawa, atau Sunda.
4. **Keluarga Jaga.** Anggota keluarga yang ditunjuk diberi tahu hanya saat risikonya tinggi, bukan diberi akses ke semua chat.
5. **Latihan Kenali Modus.** Simulasi telepon dan chat penipuan yang aman, supaya lansia terlatih mengenali tekanan sebelum benar-benar mengalaminya.

## Kapan AI dipakai, dan kapan tidak

| Tugas | Dikerjakan oleh | Alasan |
| --- | --- | --- |
| Mendeteksi file berbahaya (misalnya .apk yang menyamar jadi "undangan.pdf") | Kode (cek ekstensi dan tipe file) | Aturan pasti, tidak butuh AI dan tidak boleh salah |
| Mengecek tautan terhadap daftar domain resmi dan daftar blokir | Kode | Pencocokan pasti |
| Mengenali pola rekayasa sosial: desakan waktu, ancaman, hadiah, meminta OTP | AI (LLM) | Kalimat penipu selalu berubah-ubah; aturan kata kunci mudah diakali |
| Membaca screenshot chat atau SMS | AI (vision/OCR) | Lansia lebih sering mengirim screenshot daripada meneruskan teks |
| Memahami voice note pertanyaan | AI (STT) | Banyak lansia lebih nyaman berbicara daripada mengetik |
| Menentukan tingkat risiko akhir | Kode menggabungkan sinyal aturan + skor AI | Keputusan "berisiko tinggi" yang memicu notifikasi keluarga harus bisa dijelaskan |
| Menjelaskan dalam bahasa sederhana dan bahasa daerah | AI (LLM + TTS) | Inti nilai produk: penjelasan yang dipahami |

## Konsep inti dan cara kerja

Alurnya: **terima, periksa, jelaskan, lindungi, laporkan**.

1. **Terima.** Pengguna meneruskan apa saja ke nomor WhatsApp Tanya Dulu: teks, screenshot, file, tautan, atau voice note berisi pertanyaan.
2. **Periksa.** Kode mengecek hal-hal pasti: tipe file, domain tautan, dan nomor rekening atau telepon yang disebut. AI membaca isi dan mencari pola rekayasa sosial.
3. **Jelaskan.** Jawaban selalu punya tiga bagian: **tingkat risiko** (Aman / Hati-hati / Hampir pasti penipuan), **alasan** dalam satu atau dua kalimat, dan **langkah berikutnya** (misalnya "Jangan dibalas. Kalau ragu, telepon bank lewat nomor di belakang kartu ATM").
4. **Lindungi.** Kalau risikonya tinggi, Tanya Dulu menyarankan jeda ("Tunggu 10 menit, jangan transfer dulu") dan, kalau sudah diaktifkan, mengirim notifikasi ke anggota Keluarga Jaga.
5. **Laporkan.** Satu tombol untuk menyusun laporan ke aduannomor.id, cekrekening.id, atau IASC. Kalau pengguna sudah terlanjur transfer, Tanya Dulu langsung memberi panduan darurat: hubungi bank dan lapor ke IASC secepatnya.

**Contoh percakapan:**

> **Bu Har (voice note, bahasa Jawa):** Iki ana pesen saka kurir, jarene paketku ketahan, kon mbukak file iki.
>
> **Tanya Dulu (voice note):** Bu, sing iki *hampir mesti penipuan*. File-e jenenge "Foto Paket" nanging sejatine aplikasi (.apk). Yen dibukak, HP-ne Ibu iso dikuasai wong liya. Ampun dibukak, langsung dibusak mawon nggih. Kurir asli ora tau ngirim aplikasi liwat WhatsApp.

## Fitur

### Inti (MVP)

| Fitur | Apa yang dilakukan | Prioritas |
| --- | --- | --- |
| **Teruskan & Tanya** | Menerima teks, screenshot, file, tautan, dan voice note lewat WhatsApp atau web. | MVP |
| **Cek Risiko** | Gabungan pengecekan aturan (file, domain) dan analisis AI (pola rekayasa sosial). Hasilnya tiga tingkat risiko dengan alasan. | MVP |
| **Jawaban Suara** | Jawaban dibacakan dalam bahasa Indonesia, Jawa, atau Sunda, dengan kalimat pendek dan tempo pelan. | MVP |
| **Langkah Aman** | Setiap jawaban diakhiri dengan satu langkah konkret, termasuk nomor resmi yang benar (bukan nomor dari pesan itu). | MVP |
| **Keluarga Jaga** | Atas izin pengguna, anggota keluarga diberi tahu ringkasan saat ada pesan berisiko tinggi. Isi chat lain tetap privat. | MVP (momen wow demo) |

### Unggulan

| Fitur | Apa yang dilakukan | Kenapa keren | Prioritas |
| --- | --- | --- | --- |
| **Latihan Kenali Modus** | Simulasi telepon dan chat penipuan dengan suara AI (paket tertahan, petugas bank, anak kecelakaan). Setelahnya ada penjelasan tanda-tanda yang seharusnya dikenali. | Melatih "otot curiga" dengan aman, seperti simulasi kebakaran. | Kalau sempat |
| **Panduan Darurat** | Kalau sudah terlanjur transfer atau memberi OTP: langkah per menit, nomor bank, dan draf laporan IASC. | Menit-menit pertama paling menentukan peluang dana diselamatkan. | MVP |
| **Draf Laporan** | Menyusun laporan ke aduannomor.id, cekrekening.id, atau IASC dari pesan yang diteruskan. | Membantu pemblokiran nomor dan rekening penipu untuk orang lain juga. | Kalau sempat |
| **Kabar Modus Pekan Ini** | Rangkuman modus yang paling sering ditanyakan, untuk dibagikan kader lansia atau grup keluarga. | Edukasi yang selalu relevan. | Setelah MVP |

### Lanjutan (setelah hackathon)

| Fitur | Apa yang dilakukan | Prioritas |
| --- | --- | --- |
| **Cek Suara Kloning** | Membantu mengenali tanda telepon yang memakai suara tiruan, dengan saran "pertanyaan rahasia keluarga". | Jangka panjang |
| **Kemitraan bank** | Bank mengarahkan nasabah lansia ke Tanya Dulu, dan menerima sinyal agregat modus baru. | Jangka panjang |
| **Dashboard Komunitas** | Rekap anonim modus per kecamatan untuk kader, puskesmas lansia, atau kepolisian. | Jangka panjang |

## Alur pengguna

**Lansia:** terima pesan aneh → teruskan ke Tanya Dulu (atau kirim voice note) → terima jawaban suara: tingkat risiko, alasan, dan langkah aman → kalau risikonya tinggi, keluarga diberi tahu → opsional: tekan "laporkan".

**Keluarga:** pasang Keluarga Jaga bersama orang tua (dengan persetujuan) → hanya menerima notifikasi untuk risiko tinggi → bisa langsung menelepon orang tua.

## Rencana teknologi

| Lapis | Pilihan utama | Alternatif | Fungsi |
| --- | --- | --- | --- |
| Kanal | WhatsApp Cloud API (nomor uji untuk demo) | Web PWA dengan tombol rekam suara | Menerima pesan yang diteruskan |
| Backend | FastAPI (Python) | Next.js API routes | Orkestrasi pengecekan dan respons |
| Pengecekan aturan | Fungsi Python: tipe file (magic bytes), ekstrak dan cek domain, daftar domain resmi bank dan instansi | — | Sinyal pasti dan bisa dijelaskan |
| Analisis isi | LLM dengan output JSON (sinyal: desakan, ancaman, minta OTP, hadiah, mengatasnamakan instansi) | Model klasifikasi teks open-source | Skor risiko rekayasa sosial |
| Screenshot | Model vision | OCR (PaddleOCR) + LLM | Membaca isi chat atau SMS dari gambar |
| Suara | STT: Whisper. TTS: Google Cloud TTS atau ElevenLabs (perlu diuji untuk Jawa dan Sunda) | Teks saja | Tanya dan jawab lewat voice note |
| Database | Supabase | Firebase | Pengguna, relasi Keluarga Jaga, riwayat ringkas |
| Deploy | Railway atau Render (backend) + Vercel (web) | — | Link demo untuk juri |

**Data untuk demo dan evaluasi:** kumpulkan 100–200 contoh pesan penipuan nyata dari materi edukasi OJK, Komdigi, dan berita, ditambah pesan asli yang aman (notifikasi bank resmi, pesan keluarga). Gunakan ini untuk mengukur akurasi dan *false positive*.

## Prinsip human-centered, etika, dan keamanan

- **Lebih baik terlalu hati-hati.** Kalau tidak yakin, jawabannya "Hati-hati, cek dulu lewat jalur resmi", bukan "Aman". Tanya Dulu tidak pernah menjamin sebuah pesan 100% aman.
- **Tidak mempermalukan.** Bahasa yang dipakai menghargai pengguna: "Wajar kalau bingung, penipunya memang pintar meniru." Lansia yang merasa bodoh cenderung berhenti bertanya.
- **Privasi dan otonomi lansia.** Keluarga Jaga hanya aktif atas persetujuan pengguna, hanya mengirim ringkasan risiko tinggi, dan bisa dimatikan kapan saja. Ini bukan alat untuk memata-matai orang tua.
- **Data minimal.** Pesan yang diteruskan dihapus setelah dianalisis. Yang disimpan hanya ringkasan modus untuk statistik anonim.
- **Tidak menggantikan kanal resmi.** Tanya Dulu selalu mengarahkan ke bank, IASC, Komdigi, atau polisi untuk tindakan resmi.
- **Waspada terhadap peniruan.** Tanya Dulu tidak pernah menelepon atau menghubungi pengguna duluan, dan ini dijelaskan sejak awal, supaya penipu tidak bisa menyamar sebagai Tanya Dulu.

## Metrik keberhasilan

**Saat hackathon:**

- **Deteksi:** persentase pesan penipuan dari dataset uji yang ditandai "Hati-hati" atau "Hampir pasti penipuan" (target ≥ 90%).
- **False positive:** persentase pesan asli yang salah ditandai berisiko tinggi (target ≤ 10%).
- **Uji pemahaman lansia:** 5–10 lansia atau orang tua anggota tim mencoba 5 pesan. Ukur apakah mereka bisa mengulang alasan dan langkah aman dengan kata-kata sendiri.
- **Latensi:** waktu dari pesan diteruskan sampai jawaban suara diterima (target < 15 detik).

**Setelah peluncuran:**

- Jumlah pertanyaan per pengguna per bulan (tanda kebiasaan "tanya dulu" terbentuk)
- Jumlah laporan yang diteruskan ke kanal resmi
- Survei: berapa pengguna yang batal transfer atau batal memberi kode setelah bertanya
- Retensi keluarga yang mengaktifkan Keluarga Jaga

## Scope hackathon dan skenario demo

Final Hackvidia berlangsung 24 jam, dengan pitch dan demo 5 menit. Yang wajib jadi: satu alur utuh dari pesan diteruskan sampai jawaban suara dan notifikasi keluarga.

- **Wajib:** Teruskan & Tanya, Cek Risiko, Jawaban Suara (minimal bahasa Indonesia dan Jawa), Langkah Aman, Keluarga Jaga, Panduan Darurat.
- **Kalau sempat:** Latihan Kenali Modus, Draf Laporan.
- **Tidak dikerjakan:** Cek Suara Kloning, kemitraan bank, Dashboard Komunitas.

**Pembagian tim (contoh 4 orang):** integrasi WhatsApp dan backend; pengecekan aturan, LLM, dan skor risiko; suara, bahasa daerah, dan Keluarga Jaga; dataset uji, riset lansia, dan pitch.

**Skenario demo 5 menit:**

1. **Hook (30 detik):** "Rp9 triliun lebih uang warga hilang karena penipuan. Siapa di sini yang orang tuanya pernah dapat pesan 'paket tertahan'?"
2. **Pesan .apk (60 detik):** teruskan "Undangan Pernikahan.apk" dari HP demo. Jawaban suara bahasa Jawa muncul, dan HP anggota tim lain (sebagai "anak") menerima notifikasi Keluarga Jaga.
3. **Screenshot "petugas bank" (45 detik):** kirim screenshot chat yang meminta OTP. Tunjukkan alasan dan langkah aman.
4. **Pesan asli (30 detik):** kirim notifikasi resmi yang aman untuk menunjukkan sistem tidak asal menandai semua pesan.
5. **Panduan Darurat (45 detik):** "Saya sudah terlanjur transfer." Muncul langkah per menit dan draf laporan IASC.
6. **Dampak dan bisnis (90 detik):** angka deteksi dan *false positive* dari dataset uji, kutipan lansia saat uji coba, dan model kerja sama dengan bank dan operator.

**Cadangan:** rekam video demo lengkap, karena WhatsApp API dan koneksi bisa bermasalah saat presentasi.

## Lean Canvas ringkas

| Komponen | Isi |
| --- | --- |
| Problem | Lansia sering menjadi sasaran penipuan digital; kanal resmi dipakai setelah terlambat; anak dan cucu tidak selalu bisa ditanya |
| Customer Segments | Lansia dan orang tua (pengguna), anak dewasa (pembayar dan penjaga), bank, operator seluler, program lansia pemerintah |
| Unique Value Proposition | Cukup teruskan pesannya, lalu dapat jawaban suara dalam bahasamu dan keluarga ikut menjaga |
| Solution | Teruskan & Tanya, Cek Risiko, Jawaban Suara, Keluarga Jaga, Panduan Darurat |
| Channels | Rekomendasi dari anak ke orang tua, kader lansia, posyandu lansia, kampanye bank dan OJK |
| Revenue Streams | Gratis untuk lansia; paket Keluarga Jaga berbayar; kemitraan B2B dengan bank dan operator (perlindungan nasabah lansia, data modus agregat anonim); hibah literasi digital |
| Cost Structure | Biaya pesan WhatsApp Business API, LLM, STT/TTS, hosting, pembaruan daftar modus |
| Key Metrics | Pertanyaan per pengguna, deteksi dan false positive, laporan ke kanal resmi, transaksi yang batal |
| Unfair Advantage | Data modus penipuan terbaru dari pertanyaan pengguna, dengan konteks Indonesia dan bahasa daerah |

## Pertanyaan terbuka untuk diskusi

- [ ] **Nama produk:** "Tanya Dulu", "Cek Dulu Nak", atau "Jangan Dulu"?
- [ ] **WhatsApp atau web?** WhatsApp lebih natural untuk lansia, tapi ada biaya per pesan dan risiko demo. Web lebih stabil untuk demo.
- [ ] **Bahasa daerah apa dulu?** Jawa dan Sunda paling banyak penuturnya, tapi kualitas TTS-nya perlu diuji.
- [ ] **Batas Keluarga Jaga:** apa yang boleh dilihat keluarga, dan bagaimana kalau lansia tidak ingin diawasi?
- [ ] **Dataset:** dari mana contoh pesan penipuan yang cukup banyak dan beragam, tanpa melanggar privasi korban?

## Sumber

- [Hingga 14 Januari 2026, Kerugian Masyarakat Akibat Penipuan (Scam) Rp 9,1 Triliun](https://keuangan.kontan.co.id/news/hingga-14-januari-2026-kerugian-masyarakat-akibat-penipuan-scam-rp-91-triliun) — Kontan
- [Data Bocor, Telepon Spam Melonjak: Indonesia Peringkat Dua Dunia Rentan Penipuan](https://katadata.co.id/indepth/telaah/6aa10f4783de1/data-bocor-telepon-spam-melonjak-indonesia-peringkat-dua-dunia-rentan-penipuan) — Katadata
- [Komdigi Ungkap 65% Orang Indonesia Terima Percobaan Scam Lewat SMS hingga DM](https://teknologi.bisnis.com/read/20260506/84/1971823/komdigi-ungkap-65-orang-indonesia-terima-percobaan-scam-lewat-sms-hingga-dm) — Bisnis.com
- [Fitur WhatsApp Ini Bisa Cegah Orang Tua Jadi Korban Penipuan Share Screen](https://www.kompas.tv/info-publik/683021/fitur-whatsapp-ini-bisa-cegah-orang-tua-jadi-korban-penipuan-share-screen-begini-cara-kerjanya) — Kompas TV
- [Mafindo: Kerugian Masyarakat Akibat Scam Capai Rp9,1 Triliun](https://tirto.id/mafindo-kerugian-masyarakat-akibat-scam-capai-rp91-triliun-hrwa) — Tirto
- [Kemkomdigi Ungkap Modus Baru Penipuan Digital](https://www.viva.co.id/bisnis/1879957-kemkomdigi-ungkap-modus-baru-penipuan-digital) — Viva
- [Marak Penipuan Online, Ini Cara Praktis Cegah Risikonya](https://inet.detik.com/security/d-8325514/marak-penipuan-online-ini-cara-praktis-cegah-risikonya-agar-tetap-aman) — detikInet
