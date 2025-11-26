# Analisis Kinerja Antrean ATM BNI ITERA Menggunakan Model M/M/1

Sebuah studi kasus pemodelan stokastik untuk mengevaluasi efisiensi layanan ATM BNI di lingkungan kampus Institut Teknologi Sumatera (ITERA).

## Ringkasan Proyek

Penelitian ini menganalisis perilaku antrean pada mesin ATM BNI ITERA dengan menerapkan **Model Antrean M/M/1** (Kedatangan Poisson, Pelayanan Eksponensial, Satu Server). Tujuannya adalah untuk menghitung parameter kinerja kunci seperti laju kedatangan $(\lambda)$, laju pelayanan $(\mu)$, tingkat utilisasi sistem $(\rho)$, rata-rata panjang antrean $(L_q)$, dan waktu tunggu $(W_q)$ untuk mengidentifikasi titik kritis layanan.

## Temuan Utama

Hasil analisis menunjukkan variasi kinerja sistem yang signifikan antara hari kerja normal dan hari dengan beban tinggi.

### 1. Pola Kedatangan dan Pelayanan (Validasi M/M/1)
* **Waktu Pelayanan** terbukti mengikuti **Distribusi Eksponensial**, yang memvalidasi asumsi dasar untuk penggunaan model M/M/1.
* Mayoritas transaksi diselesaikan dalam waktu yang relatif singkat, mengindikasikan bahwa proses pelayanan ATM bersifat acak (*memoryless*).

### 2. Tingkat Utilisasi Sistem $(\rho)$

| Hari | Utilisasi Sistem ($\rho$) | Keterangan |
| :--- | :--- | :--- |
| **Senin - Kamis** | **31,7% - 42,2%** | **Sangat Stabil**. Sistem memiliki kapasitas yang cukup dan pengguna umumnya dilayani tanpa antrean yang berarti. |
| **Jumat** | **83,3%** | **Mendekati Batas Kapasitas**. Terjadi lonjakan beban sistem yang drastis.Hail ini dipicu oleh tingginya aktivitas kampus yaitu acara Riuh Wisuda. |

### 3. Metrik Antrean dan Waktu Tunggu

| Hari | Rata-rata Panjang Antrean ($L_q$) | Rata-rata Waktu Tunggu ($W_q$) |
| :--- | :--- | :--- |
| **Senin - Kamis** | $\leq$ 0.8 orang | Sangat singkat, $\leq$ 1.2 menit |
| **Jumat** | 4.167 orang | 6.522 menit |

Lonjakan pada hari Jumat ini mengindikasikan penurunan signifikan dalam Kualitas Layanan (*QoS*) pada waktu-waktu kritis.

## Data dan Metode

* **Jenis Data:** Data Primer
* **Teknik Pengumpulan Data:** Observasi Langsung  di lokasi ATM BNI ITERA.
* **Total Data:** 313 data pelanggan.
* **Periode Observasi:** 5 hari kerja (Senin-Jumat), dibagi menjadi 3 sesi per hari (Pagi, Siang, Sore) untuk menangkap variasi intensitas.

## Implikasi dan Rekomendasi

Berdasarkan hasil observasi dan analisis:

1.  **Pemeliharaan Preventif:** Pihak pengelola disarankan melakukan pemeliharaan secara berkala sebelum memasuki jam-jam sibuk agar mesin ATM tetap berfungsi optimal.
2.  **Peningkatan Kapasitas:** Jika pola peningkatan jumlah pengguna ini terjadi secara berulang, **penambahan mesin ATM** atau alternatif fasilitas lainnya dapat dipertimbangkan agar menghindari antrean panjang.
3.  **Saran Penelitian Lanjutan:** Durasi pengamatan perlu diperluas (seperti mencakup periode awal bulan atau momen tertentu yang meningkatkan aktivitas transaksi), serta membandingkan penelitian dengan model antrean lain atau simulasi kejadian diskrit untuk memperoleh evaluasi kinerja sistem yang lebih menyeluruh.

---

*Proyek ini disusun untuk memenuhi Tugas Besar Mata Kuliah Pemodelan Stokastik, Program Studi Sains Data, Institut Teknologi Sumatera (ITERA).*

**Kelompok 12 Stokastik RA**
* Ibrahim Al Kahfi - 122450100 
* Novelia Adinda - 122450104 
* Rendra Eka Prayoga - 122450112 
* Smertniki Javid Ahmedthian - 122450115
