# Pengembangan Game Edukasi 2D Berbasis Roblox Studio sebagai Media Pembelajaran Tokoh Alkitab Simon Petrus untuk Anak Sekolah Minggu

README ini memuat dan merangkum UTS Riset Informatika: rancangan game, penelitian terdahulu, research gap, pertanyaan riset, rencana evaluation metric, dan rencana dataset.

## 1. Ringkasan

Penelitian ini mengembangkan game edukasi 2D single player di Roblox Studio untuk membantu anak sekolah minggu mempelajari tokoh Simon Petrus. Game memiliki satu level utama untuk semua pemain dan satu level tambahan yang berbeda untuk dua kelompok usia (Pratama 7-10 tahun dan Remaja 12 tahun ke atas), dengan perbedaan bahasa narasi, jumlah kata, dan durasi bermain. Pengembangan memakai metode Game Development Life Cycle (GDLC). Evaluasi mencakup fungsionalitas (black box), kelayakan isi (validasi pendeta/pembimbing sekolah minggu), usability (SUS atau UEQ), dan peningkatan pemahaman anak (pre-test, post-test, N-Gain).

## 2. Rancangan Game

### 2.1 Spesifikasi

| Aspek | Keterangan |
|-------|------------|
| Platform | Roblox Studio (bahasa Lua) |
| Tampilan | 2D (antarmuka/UI dan top-down POV) |
| Mode | Single player |
| Sasaran | Anak sekolah minggu, kelompok Pratama (7-10 tahun) dan Remaja (12 tahun ke atas) |
| Metode pengembangan | GDLC (initiation, pre-production, production, testing, beta, release) |
| Validasi isi | Pendeta dan/atau pembimbing sekolah minggu |

### 2.2 Struktur level

| Level | Kelompok | Kisah | Rujukan Alkitab |
|-------|----------|-------|-----------------|
| **Level utama** | Semua | Petrus membantu membagikan roti dan ikan saat Yesus memberi makan lima ribu orang | Mat. 14:13-21; Mrk. 6:30-44; Luk. 9:10-17; Yoh. 6:1-14 |
| **Level tambahan 1** | Pratama (7-9 tahun) | Petrus dipanggil berjalan di atas air, kelanjutan langsung dari level utama | Mat. 14:22-33 |
| **Level tambahan 2** | Remaja (12 tahun ke atas) | Petrus menyangkal Yesus tiga kali pada malam penangkapan Yesus, sebelum penyaliban | Mat. 26:69-75; Mrk. 14:66-72; Luk. 22:54-62; Yoh. 18:15-27 |

Catatan isi: keempat Injil menyebut murid-murid secara bersama-sama membagikan roti dan ikan. Dalam game, Petrus dihadirkan sebagai salah satu dari murid-murid tersebut. Penggambaran peran dan nada narasi setiap level divalidasi oleh pendeta/pembimbing sekolah minggu.

### 2.3 Diferensiasi per kelompok usia

| Aspek | Pratama (7-9 tahun) | Remaja (12 tahun ke atas) |
|-------|---------------------|---------------------------|
| Bahasa narasi | Sederhana, kalimat pendek, kosakata konkret | Lebih kaya dan kompleks |
| Jumlah kata | Lebih sedikit | Lebih banyak |
| Durasi bermain (playtime) | Lebih singkat | Lebih panjang |
| Level tambahan | Mukjizat dan iman | Kegagalan dan penyesalan |

Target jumlah kata dan durasi ditetapkan pada tahap pre-production (GDLC). Keduanya dicatat sebagai variabel penelitian (lihat bagian 7).

Dasar diferensiasi: anak usia 7-11 tahun berada pada tahap operasional konkret dan usia 12 tahun ke atas pada tahap operasional formal (Bruckman dkk., 2002). Penelitian game edukasi menunjukkan bahwa usia memengaruhi perilaku pemain, dan prinsip desain bagi anak (misalnya koherensi lewat narasi) berbeda dari remaja (pilihan bermakna dan tantangan yang relevan).

## 3. Latar Belakang dan Urgensi

1. Pendidikan iman anak di sekolah minggu menghadapi kendala berulang: guru kesulitan menjaga minat anak dan kekurangan variasi media penyampai yang menarik.
2. Banyak penelitian game sekolah minggu berhenti pada rancang bangun dan uji kelayakan. Penelitian yang mengukur peningkatan pemahaman anak secara statistik masih sedikit dan berskala kecil.
3. Meta-analisis internasional menunjukkan game digital efektif untuk belajar, dan desain game (termasuk narasi) memengaruhi besar efeknya.
4. Roblox sudah dipakai untuk game edukasi anak pada mata pelajaran umum, tetapi penggunaannya untuk pembelajaran tokoh Alkitab belum ditemukan dalam literatur yang ditelaah.

## 4. Penelitian Terdahulu

### 4.1 Internasional (landasan teori)

| Penelitian | Jenis | Temuan inti yang relevan |
|-----------|-------|--------------------------|
| Wouters dkk. (2013), *Journal of Educational Psychology* 105(2) | Meta-analisis | Serious games lebih efektif daripada instruksi konvensional untuk belajar (d = 0,29; 77 studi, N = 5.547); efek lebih besar bila game dipadukan dengan metode pengajaran lain dan dimainkan dalam beberapa sesi |
| Clark dkk. (2016), *Review of Educational Research* 86(1) | Meta-analisis | Game digital meningkatkan pembelajaran dibanding kondisi nongame (efek 0,33; CI 95% 0,19-0,48; k = 57); efek bervariasi menurut mekanik game serta karakteristik visual dan naratif |
| Han, Liu, Gao (2023), *Education Sciences* 13(3):296 | Systematic review (PRISMA, 40 studi) | Roblox menarik banyak pengguna, memunculkan sikap positif, dan mendukung kemampuan kognitif dan nonkognitif; tantangannya mencakup perundungan siber, keamanan siber, dan kurangnya desain pembelajaran |
| Alotaibi (2024), *Frontiers in Psychology* 15 | Meta-analisis, anak usia dini | Game-based learning berefek sedang sampai besar pada hasil kognitif, sosial, emosional, motivasi, dan keterlibatan |
| Binhasyeesulaiman dkk. (2025), IEEE iSTEM-Ed | Eksperimen kecil, Roblox | Game persamaan linear di Roblox diuji pada 33 siswa dengan survei kepuasan terhadap konten, desain, karakteristik, dan performa |
| Aygül & Gürbüz (2021), *J. Qualitative Research in Education* 25 | Analisis semiotik | Game edukasi bertema agama berfungsi bagi sosialisasi religius anak, tetapi tanda dan isinya perlu dikendalikan secara pedagogis |
| Jejak Anbiya', *Quranica* (Universiti Malaya) | Quasi-eksperimen, board game | Pre-test/post-test pada 10 murid menunjukkan peningkatan ranah kognitif, afektif, dan psikomotor |
| Gabriel & Dangl (2020), *Österreichisches Religionspädagogisches Forum* 28(1) | Studi kualitatif | Mahasiswa calon guru menilai potensi pedagogis game digital untuk pendidikan agama relatif rendah, sehingga bukti efektivitas diperlukan |

### 4.2 Landasan diferensiasi usia dan desain naratif

| Penelitian | Relevansi |
|-----------|-----------|
| Bruckman, Bandlow, & Forte (2002), "HCI for Kids" (bab buku) | Tahap perkembangan: operasional konkret (7-11 tahun) dan formal (12 tahun ke atas) |
| O'Rourke dkk. (2013), "The Effects of Age on Player Behavior in Educational Games" | Usia memengaruhi perilaku pemain di game edukasi; disertai saran desain |
| "One Size Doesn't Fit All: Age-Aware Gamification Mechanics for Multimedia Learning Environments" (pracetak arXiv) | Anak memperoleh koherensi dari narasi, remaja membutuhkan pilihan bermakna dan tantangan yang relevan |
| "Designing Narrative-Focused Role-Playing Games" (pracetak arXiv) | Unsur naratif meningkatkan keterlibatan tanpa mengurangi pembelajaran, tetapi menggandakan waktu penyelesaian |
| Bible Games as Religious Educational Tools in Seventh-Day Adventist Church (*Gamevironments*, 2021) | Game Alkitab cenderung berpola tanya-jawab dan hafalan teks; game naratif berbeda dari pola tersebut |

### 4.3 SINTA 2 (metode pengembangan)

| Penelitian | Isi |
|-----------|-----|
| Prasetiyo, Widaningrum, Astuti (2020), *Jurnal RESTI* 4(1):37-49 | Game edukasi Android "Math & Trash" dengan Construct 2, UML, dan GDLC; uji unit, integrasi, dan sistem |
| Laksana, Wahyuni, Aditya (2023), *Jurnal RESTI* 7(3):688-696 | Game edukasi mobile pengenalan IoT dengan metode multimedia development; survei penerimaan 75,37% kategori sangat baik |

### 4.4 Game edukasi sekolah minggu dan Roblox di Indonesia

| Penelitian | Platform / metode | Evaluasi | Keterbatasan |
|-----------|-------------------|----------|--------------|
| Haliem, skripsi Univ. Kristen Petra, *Game Visual Novel Alkitab* | Visual novel + kuis/minigame | Uji-t satu arah vs metode konvensional (t = 1,732; p = 0,045) | Satu gereja, peserta terbatas |
| Tulung dkk. (2017), *Rancang Bangun Aplikasi Game Untuk Anak Sekolah Minggu* | Aplikasi game, prototyping | Tidak disebut di abstrak | Fokus rancang bangun |
| *Sunday Fun-Day* (UKSW) | Android | Tidak disebut di abstrak | Fokus membantu pengajar |
| *Aplikasi Game Alkitab Berbasis Android* (Unkriswina) | Android, waterfall | Uji coba ke anak | Studi kasus satu sekolah minggu |
| Hariyanto dkk., *Bible's Back in Time Challenge* | Board game fisik, R&D MANTAP Level 1 | Kelayakan 91,04% | Bukan digital |
| Implementasi FSM pada game edukasi 2D (JATI) | **Roblox Studio 2D**, waterfall | Pre/post-test 10 responden, kenaikan rata-rata 30,88% | Domain fasilitas umum, sampel kecil |
| *Geo Explorer* berbasis Roblox (JPPGSD, UNESA) | Roblox, kelas 4 SD Surabaya | Pre/post-test, rata-rata naik 50,12 menjadi 88 | Domain geografi |
| Game Imersif Telkom University Surabaya | Roblox Studio, GDLC | UEQ | Domain pengenalan kampus |
| *Pengembangan Game Edukasi Naratif* (UPN Veteran Jatim) | Game naratif | Kelayakan | Tema dakwah, preseden dari kampus |

## 5. Research Gap

1. **Gap domain dan platform.** Game edukasi sekolah minggu yang ada berupa aplikasi Android, visual novel, atau board game fisik. Roblox sudah dipakai untuk game edukasi anak pada mata pelajaran umum, tetapi penggunaannya untuk pembelajaran tokoh Alkitab belum ditemukan.
2. **Gap evaluasi.** Banyak penelitian game sekolah minggu berhenti pada rancang bangun dan uji kelayakan. Studi yang mengukur peningkatan pemahaman secara statistik masih sedikit dan berskala kecil.
3. **Gap desain per kelompok usia.** Game sekolah minggu yang ditemukan umumnya tidak membedakan narasi, jumlah kata, dan durasi bermain menurut tahap perkembangan, padahal literatur menunjukkan usia memengaruhi perilaku dan kebutuhan desain pemain.

Implikasi desain: game berfungsi sebagai pendamping pengajaran guru dan dapat dimainkan lebih dari satu sesi (Wouters dkk., 2013). Mode single player mengurangi risiko perundungan dan keamanan siber pada Roblox yang dicatat Han dkk. (2023). Validasi isi oleh pendeta/pembimbing sejalan dengan saran pengendalian pedagogis atas isi game religius (Aygül & Gürbüz, 2021).

## 6. Pertanyaan Riset dan Hipotesis

- **RQ1.** Bagaimana merancang dan membangun game edukasi 2D single player berbasis Roblox Studio untuk pembelajaran tokoh Simon Petrus, dengan level utama dan level tambahan yang dibedakan menurut kelompok usia?
- **RQ2.** Apakah game layak secara fungsional dan isi, serta memiliki usability yang baik?
- **RQ3.** Apakah terdapat peningkatan pemahaman anak setelah memakai game pada masing-masing kelompok usia?

Hipotesis RQ3, untuk setiap kelompok usia:
- H0: tidak ada perbedaan rata-rata skor pre-test dan post-test.
- H1: rata-rata skor post-test lebih tinggi daripada pre-test.

Perbandingan N-Gain antarkelompok bersifat eksploratif karena instrumen dan ukuran sampel setiap kelompok berbeda.

## 7. Rencana Evaluation Metric

| Dimensi | Metrik / instrumen | Responden | Dasar |
|---------|-------------------|-----------|-------|
| Fungsionalitas | Black box testing | Peneliti | Dipakai pada game Roblox lain |
| Kelayakan isi | Validasi ahli, skor persen, termasuk kesesuaian narasi dengan teks Injil | Pendeta/pembimbing sekolah minggu | Lazim dilaporkan sebagai persen |
| Usability | SUS atau UEQ untuk guru dan Remaja; skala wajah untuk Pratama | Guru dan anak | UEQ pada game Roblox Telkom; SUS lazim di game edukasi |
| Efektivitas belajar | Pre-test/post-test per kelompok usia, N-Gain, uji-t berpasangan (atau Wilcoxon bila data tidak normal), effect size | Anak sekolah minggu | Petra memakai uji-t; meta-analisis melaporkan effect size |
| Variabel pengiring | Jumlah kata narasi dan playtime per kelompok | Log game | Narasi tambahan memperpanjang waktu bermain tanpa mengurangi pembelajaran (lihat 4.2) |

Soal inti untuk level utama dibuat paralel pada kedua kelompok dengan narasi yang disesuaikan usia, ditambah soal lanjutan untuk level tambahan masing-masing kelompok.

Ukuran sampel kemungkinan kecil dan terbagi dua kelompok. Studi sejenis memakai sampel 10 anak (Jejak Anbiya'; game Roblox JATI), tetapi hasil per kelompok dianalisis dengan hati-hati dan dilaporkan sebagai keterbatasan.

## 8. Rencana Dataset

| Data | Format | Kolom minimal |
|------|--------|---------------|
| Skor pre-test | CSV | kode_peserta, kelompok_usia, usia, skor_pre |
| Skor post-test | CSV | kode_peserta, kelompok_usia, skor_post |
| Log game | CSV | kode_peserta, kelompok_usia, level, skor, playtime_menit |
| Kuesioner usability | CSV | kode_peserta/guru, kelompok_usia, butir 1..n |
| Validasi ahli | CSV | butir, skor, komentar |
| Black box | CSV | skenario, hasil, catatan |
| Profil narasi | CSV | kelompok_usia, level, jumlah_kata |

Perlindungan data anak: kode peserta (P01, P02, ...) tanpa nama, foto, atau kontak; pemetaan kode ke nama tidak diunggah; persetujuan orang tua/wali dan izin gereja diperoleh secara tertulis.

## 9. Keterbatasan

- Peserta berasal dari satu atau sedikit gereja dalam jumlah kecil, sehingga hasil tidak dapat digeneralisasi.
- Perbandingan antarkelompok usia bersifat eksploratif.
- Akses dan kebijakan akun Roblox bagi anak perlu disiapkan, termasuk rencana cadangan perangkat uji.

## 10. Research Mind Map

Tersedia di dalam folder main/UTS.

## 11. Referensi

Kuartil mengacu pada SCImago (SJR) dan perlu diverifikasi ulang sebelum sitasi final.

**A. Internasional**
- Wouters, P., van Nimwegen, C., van Oostendorp, H., & van der Spek, E. D. (2013). A meta-analysis of the cognitive and motivational effects of serious games. *Journal of Educational Psychology*, 105(2), 249-265. https://doi.org/10.1037/a0031311 (SJR Q1)
- Clark, D. B., Tanner-Smith, E. E., & Killingsworth, S. S. (2016). Digital games, design, and learning: A systematic review and meta-analysis. *Review of Educational Research*, 86(1), 79-122.
- Han, J., Liu, G., & Gao, Y. (2023). Learners in the Metaverse: A systematic review on the use of Roblox in learning. *Education Sciences*, 13(3), 296. https://doi.org/10.3390/educsci13030296 (Scopus; SJR Q1 kategori Education pada 2024-2025)
- Alotaibi, M. S. (2024). Game-based learning in early childhood education: a systematic review and meta-analysis. *Frontiers in Psychology*, 15. https://doi.org/10.3389/fpsyg.2024.1307881 (SJR Q2)
- Binhasyeesulaiman, N., dkk. (2025). Game-Based Learning of Linear Equations Using Roblox: Enhancing Pre-Semester Math Readiness. IEEE iSTEM-Ed. https://doi.org/10.1109/iSTEM-Ed65612.2025.11129279
- Aygül, H. H., & Gürbüz, G. (2021). A semiotic analysis of digital educational games with religious themes for children. *Journal of Qualitative Research in Education*, 25, 51-75. https://doi.org/10.14689/enad.25.3
- Gabriel, S., & Dangl, O. (2020). Religious Education with digital games? *Österreichisches Religionspädagogisches Forum*, 28(1), 59-77. https://doi.org/10.25364/10.28:2020.1.4
- The Development of the Educational Game "Jejak Anbiya'". *Quranica*, Universiti Malaya. https://doi.org/10.22452/quranica.vol17no1.17
- Bible Games as Religious Educational Tools in Seventh-Day Adventist Church. *Gamevironments*, 2021. https://doi.org/10.48783/gameviron.v15i15.143

**B. Landasan usia dan desain naratif**
- Bruckman, A., Bandlow, A., & Forte, A. (2002). HCI for kids. https://faculty.cc.gatech.edu/~asb/papers/chapters/hci-for-kids.pdf
- O'Rourke, E., dkk. (2013). The Effects of Age on Player Behavior in Educational Games. https://grail.cs.washington.edu/wp-content/uploads/2015/08/orourke2013teo.pdf
- One Size Doesn't Fit All: Age-Aware Gamification Mechanics for Multimedia Learning Environments (pracetak). https://arxiv.org/pdf/2512.15630
- Designing Narrative-Focused Role-Playing Games (pracetak). https://ar5iv.labs.arxiv.org/html/2008.13749

**C. SINTA 2 (Jurnal RESTI)**
- Prasetiyo, H., Widaningrum, I., & Astuti, I. P. (2020). Game Edukasi Math & Trash Berbasis Android dengan Menggunakan Scirra Construct 2 dan Adobe Phonegap. *Jurnal RESTI*, 4(1), 37-49. https://doi.org/10.29207/resti.v4i1.1385
- Laksana, I. P., Wahyuni, E. D., & Aditya, C. S. K. (2023). Game Design for Mobile App-Based IoT Introduction Education in STEM Learning. *Jurnal RESTI*, 7(3), 688-696. https://doi.org/10.29207/resti.v7i3.5007

**D. Game edukasi sekolah minggu dan Roblox di Indonesia**
- Haliem, H. K. *Pengembangan Game Visual Novel Alkitab untuk Membantu Pendidikan Anak di Minggu Gereja.* Skripsi, Universitas Kristen Petra. https://dewey.petra.ac.id/catalog/digital/get-file/468928 (jika tautan tidak terbuka, cari lewat katalog perpustakaan Petra)
- Tulung, R. A. M., dkk. (2017). Rancang Bangun Aplikasi Game Untuk Anak Sekolah Minggu. https://ejournal.unsrat.ac.id/v3/index.php/informatika/article/view/17656
- Perancangan Aplikasi Game "Sunday Fun-Day". https://ejournal.uksw.edu/itexplore/article/view/9509
- Aplikasi Game Alkitab Berbasis Android pada Anak Sekolah Minggu. https://ojs.unkriswina.ac.id/index.php/semnas-FST/article/download/530/354/2920
- Hariyanto, E. C., dkk. Pengembangan Board Game Interaktif "Bible's Back in Time Challenge". https://ejournal.uki.ac.id/index.php/shan/article/view/7877
- Implementasi Finite State Machine pada Game Edukasi 2D untuk Pengenalan Fasilitas Umum Anak Usia Dini. JATI. https://ejournal.itn.ac.id/jati/article/view/15736
- Pengembangan Media Game Edukasi "Geo Explorer" Berbasis Roblox. JPPGSD, UNESA. https://ejournal.unesa.ac.id/index.php/jurnal-penelitian-pgsd/article/download/80414/56067/213565
- Game Imersif Telkom University Campus Surabaya Berbasis Roblox. https://openlibrarypublications.telkomuniversity.ac.id/index.php/engineering/article/download/28930/27326
- Pengembangan Game Edukasi Naratif (UPN Veteran Jatim). https://repository.upnjatim.ac.id/47655/9/19081010191-cover.pdf
