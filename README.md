# Dataset Narkotika PN Semarang

Dataset untuk Tugas 2 (SubCPMK-2), UTS Temu Kembali Informasi, semester ganjil 2026/2027, Universitas Muhammadiyah Malang.

## Anggota kelompok

| **Nama** | **NIM** |
|---|---|
| Hafizh Al Bukhori | 202310370311097 |

Nama repository: **Dataset-Narkotika_097_XXX**.  
`XXX` disesuaikan dengan tiga digit terakhir NIM anggota kelompok kedua, jika ada. Repository pengumpulan harus bersifat **public**.

## Cakupan

- Pengadilan: **PN Semarang**.
- Direktori: **Pidana Khusus**; klasifikasi: **Narkotika dan Psikotropika**.
- Jumlah: **5 putusan pengadilan** dalam format PDF.
- Tahun putusan: disesuaikan dengan dokumen yang dikumpulkan, dengan rekomendasi rentang tahun 2023–2025.
- Sumber dokumen: Direktori Putusan Mahkamah Agung Republik Indonesia.
- Status putusan: putusan yang digunakan tidak boleh berstatus **Berkekuatan Hukum Tetap (BHT)**.

Jumlah 5 putusan mengikuti ketentuan pada poin 2 instruksi tugas. Pada poin 5a dan 5b terdapat penyebutan 50 dokumen dan 50 data putusan. Perbedaan jumlah tersebut perlu dikonfirmasi kepada dosen pengampu.

## Sumber dan pengumpulan

Dokumen putusan diperoleh melalui [Direktori Putusan Mahkamah Agung Republik Indonesia](https://putusan3.mahkamahagung.go.id/direktori.html).

Pengumpulan dilakukan dengan memilih direktori **Pidana Khusus**, klasifikasi **Narkotika dan Psikotropika**, serta **Pengadilan Negeri Semarang**. Dokumen putusan digunakan sebagai sumber data untuk penyusunan dataset dalam domain Temu Kembali Informasi (TKI).

Dokumen PDF yang dikumpulkan digunakan sebagai sumber utama untuk mengisi ringkasan pada file Overview.xlsx. Informasi nomor perkara, barang bukti, dan amar putusan disesuaikan dengan isi dokumen asli.

## Pemeriksaan status putusan

Sesuai ketentuan tugas, putusan dengan status **Berkekuatan Hukum Tetap (BHT)** tidak digunakan.

Pemeriksaan status dilakukan dengan memperhatikan informasi yang tersedia pada halaman detail putusan di Direktori Putusan Mahkamah Agung. Apabila status tidak dicantumkan secara jelas pada halaman sumber, informasi tersebut tidak disimpulkan sendiri dan perlu dicatat sebagai **Tidak tercantum**.

Keterangan status dalam dataset mengikuti informasi yang benar-benar tersedia pada sumber resmi.

## Struktur repository

```text
Dataset-Narkotika_097_XXX/
├── Dataset/
│   └── Narkotika.zip
├── Overview/
│   └── Overview.xlsx
└── README.md
```

File `Dataset/Narkotika.zip` berisi 5 dokumen putusan pengadilan dalam format PDF.

File `Overview/Overview.xlsx` berisi ringkasan informasi dari 5 putusan yang dikumpulkan.

## Isi Excel

Lembar **Overview** memuat 5 baris data putusan dengan lima kolom utama sesuai ketentuan tugas:

| **Kolom** | **Isi** |
|---|---|
| No | Nomor urut putusan |
| No Putusan | Identitas resmi nomor perkara |
| Lembaga Peradilan | Pengadilan Negeri Semarang |
| Barang Bukti | Rincian barang bukti berdasarkan dokumen putusan |
| Amar Putusan | Isi amar putusan berdasarkan bagian MENGADILI pada PDF asli |

Kolom Barang Bukti dan Amar Putusan memuat informasi sesuai dokumen sumber. Teks disusun agar mudah dibaca dan dicocokkan dengan PDF asli.

## Penyusunan ringkasan

Informasi barang bukti diambil dari bagian penetapan barang bukti dalam amar putusan. Informasi amar putusan diambil dari bagian **MENGADILI** pada dokumen PDF.

Penulisan ringkasan mempertahankan substansi informasi dari dokumen asli, termasuk nama, nomor perkara, jenis barang bukti, jumlah, berat, serta amar pidana yang dijatuhkan.

Ringkasan dalam Excel digunakan untuk memudahkan penelusuran dan pencocokan informasi. Dokumen PDF asli tetap menjadi sumber utama apabila diperlukan pemeriksaan lebih lanjut.

Dataset ini merupakan kumpulan dokumen untuk keperluan penugasan Temu Kembali Informasi, bukan sampel acak yang mewakili seluruh perkara narkotika di Pengadilan Negeri Semarang.

## Cara menggunakan

1. Unduh file `Dataset/Narkotika.zip`.
2. Ekstrak ZIP untuk memperoleh 5 dokumen PDF putusan pengadilan.
3. Buka `Overview/Overview.xlsx` untuk melihat ringkasan informasi setiap putusan.
4. Cocokkan nomor putusan dan informasi lainnya dengan dokumen PDF asli.
5. Gunakan dokumen dan ringkasan tersebut untuk keperluan pembelajaran serta eksperimen Temu Kembali Informasi.

## Tujuan penggunaan dataset

Dataset ini disusun untuk memenuhi penugasan Tugas 2 (SubCPMK-2) pada mata kuliah Temu Kembali Informasi, Universitas Muhammadiyah Malang.

Dataset dapat digunakan sebagai bahan pembelajaran untuk memahami proses akuisisi, pengelolaan, dan representasi dokumen hukum sebagai sumber informasi yang dapat dimanfaatkan dalam sistem Temu Kembali Informasi.

---

**Universitas Muhammadiyah Malang**  
**Temu Kembali Informasi — Semester Ganjil 2026/2027**