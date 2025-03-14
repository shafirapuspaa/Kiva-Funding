# Kiva-Funding
Kiva adalah organisasi non-profit yang menyediakan platform bagi individu di seluruh dunia untuk memberikan pinjaman mikro kepada wirausahawan, pelajar, dan individu yang membutuhkan dukungan keuangan. Melalui sistem crowdfunding, Kiva memungkinkan orang-orang untuk meminjam uang dari donor individu dengan bunga rendah atau tanpa bunga untuk membiayai usaha kecil, pendidikan, atau kebutuhan dasar.

Bagaimana Kiva bekerja?

- Pengajuan Pinjaman – Wirausahawan atau individu yang membutuhkan dana mengajukan pinjaman melalui organisasi mitra yang bekerja sama dengan Kiva.
- Peninjauan dan Persetujuan – Organisasi mitra mengevaluasi permohonan berdasarkan kelayakan dan kebutuhan finansial.
- Pendanaan oleh Peminjam – Pinjaman yang telah disetujui akan diunggah ke platform Kiva, dan individu di seluruh dunia dapat memilih untuk meminjamkan dana.
- Pengembalian Dana – Setelah dana diberikan, peminjam menggunakannya untuk usaha mereka dan mengembalikan pinjaman secara berkala sesuai kesepakatan.
- Dampak Positif – Uang yang dipinjamkan membantu pengusaha kecil mengembangkan bisnisnya, menciptakan lapangan kerja, dan meningkatkan kondisi ekonomi komunitas mereka.
- Kiva membantu meningkatkan inklusi keuangan dengan menjembatani kesenjangan akses kredit bagi masyarakat kurang mampu.

## Dataset
Dataset yang digunakan dalam proyek ini berasal dari Kaggle:
Sumber: [https://www.kaggle.com/datasets/kiva/data-science-for-good-kiva-crowdfunding/data](https://www.kaggle.com/datasets/kiva/data-science-for-good-kiva-crowdfunding/data)

## Langkah Analisis
1. Impor Data
    - import pandas
    - import numpy
    - import seaborn
    - import mathplotlib
    - import datetime
2. Membaca Data
3. Merubah Tipe Data
4. Mengubah Missing Value
5. Analisis Data
    - Uji korelasi hubungan `loan_amount` dan `lender_count`
    - Mencari sektor dengan pinjaman terbesar
    - Mencari sektor dengan lender_count (kreditur yang berkontribusi) terbanyak jika target pinjamn terpenuhi
    - Mencari country terbaik dengan spesifikasi sektor pertanian, kondisi durasi pencairan pinjaman kurang dari rata rata, dan kondisi target peminjam terpenuhi dibawah rata rata hari
    - Mencari activity terbesar jika spesifikasi sektor pertanian, kondisi durasi pencairan pinjaman kurang dari rata rata, kondisi target peminjam terpenuhi dibawah rata rata hari, dan country Philippines
    - Mencari region terbesar jika spesifikasi sektor pertanian, kondisi durasi pencairan pinjaman kurang dari rata rata, dan kondisi target peminjam terpenuhi dibawah rata rata hari, activity pigs, dan country Philippines.

## Deskripsi Kolom 
Berikut adalah deskripsi dari masing-masing kolom:
- `id`: Unique ID untuk masing-masing loan (loan ID)
- `funded_amount`: Jumlah yang dicairkan oleh Kiva ke agen (USD)
-	 `loan_amount`: Jumlah yang disalurkan oleh agen ke peminjam (USD)
-	 `activity`: Kategori lebih spesifik dari `sector`
-	 `sector`: Kategori dari loan
-	 `country`: Nama negara lengkap, tempat pinjaman dicairkan
-	`region`: Nama wilayah lengkap dari `country`
-	`currency`: Mata uang
-	`partner_id`: ID untuk organisasi partner
-	`posted_time`: Waktu pinjaman di-posting di Kiva oleh agen
-	`funded_time`: Waktu pinjaman telah sepenuhnya dibiayai oleh pemberi pinjaman
-	`term_in_months`: Durasi pencairan pinjaman (dalam satuan bulan)
-	`lender_count`: Banyaknya peminjam yang berkontribusi
-	`repayment_interval`: Cara pelunasan peminjaman
  
## Tableau public
[Tableau](https://public.tableau.com/shared/HC2PF7RHH?:display_count=n&:origin=viz_share_link)
