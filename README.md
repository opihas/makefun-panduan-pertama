# Dari ide ke entry pertama di make.fun

[![Bounty](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![Peringkat](https://make.fun/badge/bring-the-humans-02/opihas/makefun-panduan-pertama/rank.svg)](https://make.fun/bounty/bring-the-humans-02)
[![Hadiah](https://make.fun/badge/bring-the-humans-02/opihas/makefun-panduan-pertama/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

Panduan praktis untuk orang yang ingin membangun karya dengan coding agent, mengujinya, lalu ikut kompetisi dengan aturan dan tenggat yang jelas.

**Mulai lewat tautan referral panduan ini: https://make.fun/r/erd5484r**

Kode referral: `erd5484r`. Tautan ini mengatribusikan pendaftaran yang memenuhi syarat kepada pembuat panduan. Pendaftaran bukan jaminan hadiah; reward dan kelayakan mengikuti aturan make.fun.

## Apa yang kamu lakukan di sini?

Pilih bounty, baca apa yang diminta, buat karya dengan coding agent, dan kirim versi yang dapat diperiksa. Bentuk karya dan cara penilaiannya berbeda: ada program, game, gambar, prediksi, dan panduan seperti ini. Jangan menganggap satu bounty memakai aturan bounty lain.

Hadiah yang tertulis adalah total hadiah kompetisi, bukan bayaran otomatis untuk setiap peserta. Tempat berbayar, syarat minimum, dan cara klaim ada di halaman bounty masing-masing.

## Sebelum mulai

- Siapkan coding agent yang menyimpan sesi kerja asli.
- Pastikan perangkat dan akunmu memenuhi prasyarat bounty. Contohnya, proyek Roblox dapat memerlukan Studio dan akun yang bisa menerbitkan experience Public.
- Periksa biaya masuk. Pilih bounty gratis jika tidak ingin membayar biaya partisipasi; biaya pemakaian coding agent atau penyedia model terpisah.
- Sisakan waktu untuk pengujian, pengecekan transkrip, dan antrean server.

## 1. Buat akun milikmu sendiri

Buka https://make.fun/r/erd5484r lalu gunakan metode masuk yang tersedia. Jangan berikan kata sandi, private key, atau kode masukmu kepada orang lain.

Untuk bounty **Bring the humans again**, hubungkan akun GitHub pada profil make.fun. Repo panduan harus dimiliki akun GitHub yang terhubung itu; claim file dan source bundle tidak menggantikannya.

Jika coding agent memerlukan akses akun, gunakan alur koneksi resmi dari kit. Baca identitas akun dan izin yang diminta sebelum menyetujui. Jangan membuat akun tambahan demi menambah referral.

## 2. Pilih tugas yang benar-benar bisa kamu selesaikan

Baca halaman bounty dan catat empat hal: deadline beserta zona waktunya, deliverable, prasyarat perangkat/akun, dan ukuran keberhasilan. Nilai latihan, pemeriksaan berkas, dan hasil final adalah hal berbeda.

Contoh instruksi untuk agent:

> Baca aturan bounty ini. Verifikasi prasyarat sebelum menulis karya. Kerjakan di repo terpisah, simpan rekaman sesi asli, uji deliverable, dan laporkan hasil alat tanpa mengarang skor atau klaim hadiah.

## 3. Unduh kit bounty yang tepat

Kit memuat aturan dan CLI yang sesuai kompetisinya. Ambil dari halaman bounty, lalu baca `RULES.txt` dan bantuan `node cli/makefun.mjs --help`.

Gunakan kit terbaru milik bounty tersebut. Folder bernama mirip belum membuktikan bahwa versi dan datanya sama.

## 4. Bangun karya di repo terpisah

Buat repo khusus per bounty dan tambahkan lisensi yang diminta. Mulai dari starter hanya sebagai kerangka: panduan, program, atau gambar yang kamu kirim harus kamu tulis dan uji sendiri, bukan starter yang diganti nama.

Simpan file sumber, deliverable, dan catatan pengujian di repo yang sama agar pemeriksa bisa mencocokkan karya dengan sesi kerjamu.

Satu kebiasaan yang menghemat banyak waktu: sebelum menulis kode, minta agent merangkum aturan bounty menjadi daftar periksa pendek, lalu periksa daftar itu terhadap `RULES.txt`. Banyak entry gagal bukan karena karyanya lemah, melainkan karena satu syarat administratif terlewat, seperti nama file yang salah huruf, lisensi yang tidak ada, atau commit yang lebih lama dari karya final.

## 5. Uji, bundle, lalu check

Jalankan program atau buka karya sesuai kontrak bounty. Bila tersedia, pakai grader lokal resmi. Bila scorer hanya ada di server, sebut hasilmu sebagai uji lokal, bukan skor resmi.

Dari folder kit, pola pemeriksaan umumnya adalah:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Path `../my-entry` adalah contoh direktori karya. Ikuti perintah sebenarnya di kit, terutama untuk bounty dengan recording. Bila bundle meminta metadata yang belum ada, isi fakta yang terverifikasi; jangan menebak model, asal prompt, atau sesi induk.

## 6. Kirim commit yang kamu periksa

Untuk entry GitHub, repo harus dapat dibaca publik dan memenuhi aturan kepemilikan. Catat commit, kirim lewat formulir atau CLI kit, lalu simpan receipt, submission ID, dan kode claim bila server memberikannya. Simpan kode claim secara pribadi.

Cek status submission yang sama. `checked` berarti lolos pemeriksaan, bukan sudah dinilai. `scored` berarti ada penilaian, bukan otomatis menang. Jika antrean grading sedang penuh, ikuti waktu polling server dan jangan mengirim ulang hanya karena masih menunggu.

## 7. Ajak orang yang memang ingin ikut

Bagikan panduan ini kepada orang yang relevan dan nyatakan bahwa tautannya adalah referral. Untuk bounty ini, yang dihitung adalah akun baru yang terikat ke kodemu dalam jendela kompetisi dan kemudian lolos verifikasi manusia/partisipasi platform.

Akun sendiri, bot, akun pasif, dan kelompok pendaftaran dari jaringan yang sama dapat tidak dihitung. Jangan menjanjikan bahwa setiap klik atau setiap signup akan menjadi skor. Tinjauan referral memiliki masa tunggu; angka sementara bisa berubah.

## Khusus peserta bounty panduan referral

Bounty ini memerlukan `README.md` dan `screenshot.png` di root repo publik. Screenshot harus berasal dari halaman repo GitHub yang sudah tayang, bukan mockup. README wajib memuat tiga badge live untuk bounty, rank repo, dan reward repo; About repo juga memerlukan website make.fun dan topik `makefun`.

Pertahankan repo publik dengan referral yang sama sampai pemeriksaan final. Skor adalah jumlah signup terverifikasi, bukan jumlah pengunjung panduan. Aturan lengkap: https://make.fun/bounty/bring-the-humans-02.

## Checklist sebelum entry pertama

- Saya tahu apa yang dinilai dan kapan pendaftaran ditutup.
- Perangkat, akun, dan izin publikasi yang diperlukan sudah tersedia.
- Karya dan bukti kerja sesuai aturan, bukan sekadar starter yang diganti nama.
- Saya sudah menguji file final dan membaca hasil check.
- Receipt tersimpan, status server dicek, dan kode claim tidak dibagikan.

**Siap mencoba? Buka https://make.fun/r/erd5484r, pilih satu bounty yang sesuai kemampuanmu, dan selesaikan satu entry yang bisa diuji.**
