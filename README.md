# 📝 Ringkasan Tugas Hands-On 3: Employee Attrition Analysis

### Mahasiswa
- **Nama** : Aditya Beckham
- **NIM**  : 24552011066
- **Kelas**: TIF RP 24 B (24) & Kelas AI TIF RP 23 D

---

## Deskripsi Proyek
Proyek ini menganalisis dataset **Employee Attrition (Studi Kasus 5)** dengan total 1.200 baris data karyawan untuk mengidentifikasi pola dan faktor-faktor pendorong utama di balik keputusan karyawan meninggalkan perusahaan (`keluar_perusahaan = 1`).

## 📁 Struktur Pengumpulan
Sesuai dengan ketentuan tugas, berikut berkas-berkas yang telah berhasil dihasilkan dan siap dikumpulkan:
- `Aditya_Beckham_Tugas_Hands_On_3.ipynb` : Notebook utama yang bersih dan dapat dijalankan berurutan tanpa error.
- `data_bersih.csv` : Dataset hasil pembersihan, imputasi, dan mapping target.
- `kamus_data.csv` : Penjelasan teknis mengenai tipe data, nilai unik, dan missing value setiap kolom.
- `laporan_kualitas.csv` : Perbandingan kondisi kualitas data sebelum dan sesudah dibersihkan.
- `model_attrition.pkl` : Model klasifikasi berbasis Random Forest Classifier.

---

## 📊 3 Temuan Utama yang Dapat Ditindaklanjuti (Actionable Insights)

1. **Optimalisasi Kompensasi Karyawan Muda (Faktor Gaji & Usia):**
   - *Temuan:* Variabel `gaji_bulanan_idr` dan `usia` menduduki posisi puncak dalam peringkat kepentingan fitur model Random Forest. Karyawan muda dengan pendapatan di bawah rata-rata industri memiliki tingkat pengunduran diri tertinggi.
   - *Rekomendasi:* Merancang strategi penyesuaian gaji (*compensation review*) berkala agar tetap kompetitif guna meminimalkan hilangnya talenta muda berbakat.

2. **Evaluasi Beban Kerja & Kebijakan Lembur:**
   - *Temuan:* Adanya korelasi kuat antara frekuensi kerja lembur (`lembur_Ya`) dengan tingginya tingkat *attrition*.
   - *Rekomendasi:* Mengaudit pembagian beban kerja di departemen bersangkutan, membatasi akumulasi jam lembur bulanan, serta mempromosikan program *work-life balance*.

3. **Penyusunan Peta Karier yang Jelas:**
   - *Temuan:* Karyawan yang menetap pada posisi dan masa jabatan yang sama lebih dari 3 tahun berturut-turut menunjukkan penurunan tingkat retensi yang tajam.
   - *Rekomendasi:* Mengadakan program pengembangan keterampilan internal, jalur promosi transparan, serta rotasi jabatan berkala untuk menjaga motivasi karyawan.

---

## ⚙️ Cara Menjalankan Kode
1. Pastikan library penting terpasang:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn joblib
   ```
2. Buka berkas `Aditya_Beckham_Tugas_Hands_On_3.ipynb` pada Google Colab atau Jupyter.
3. Masukkan dataset mentah `case5_employee_attrition.csv` ke dalam direktori kerja.
4. Pilih menu **Runtime -> Run All** atau jalankan semua sel secara berurutan.
