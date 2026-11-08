# Oil-Palm-Productivity-Report
This is my dummy project using Google Sheets to analyse palm productivity based on total productive palms and  the width of the area. Further analyses, such as seed type and plant age, will be analysed in the future.

Dataset source: [Long-Term Block-Level Oil Palm Productivity Dataset with Leaf Nutrient and Soil Fertility Measurements from an Indonesian Plantation](https://data.mendeley.com/datasets/93k3733p6x/2?utm_source=chatgpt.com)

## Analysis
### 1. Data Quality
### 2. Productivity Analysis
### 3. Correlation Analysis

## Insight
### 1. Data Quality Assessment

Berdasarkan hasil data cleaning dan validasi pada sheet `Cleaned_Data` serta `Block_Master`, ditemukan bahwa sebanyak **4,76% blok teridentifikasi sebagai outlier pada variabel `Area_Ha`**.

Meskipun proporsinya relatif kecil, data outlier tetap dipertahankan dalam dataset agar tidak menghilangkan informasi sebelum penyebab anomali diketahui.

**Rekomendasi:**
- Melakukan validasi luas lahan pada blok yang teridentifikasi sebagai outlier.
- Membandingkan data luas lahan dengan catatan administrasi atau hasil pengukuran lapangan.
- Melakukan evaluasi ulang terhadap produktivitas blok setelah validasi luas lahan selesai.

### 2. Relationship Between Palm Density and Annual Production

Berdasarkan hasil analisis pada sheet `Dashboard`, ditemukan hubungan linear positif antara kepadatan pohon produktif (`Palms_per_Ha`) dan total produksi TBS tahunan (`Annual_Production_kg`).

Temuan ini menunjukkan bahwa blok dengan kepadatan pohon produktif yang lebih tinggi cenderung menghasilkan total produksi TBS tahunan yang lebih besar.

Namun, hubungan tersebut juga dapat dipengaruhi oleh perbedaan luas masing-masing blok, umur tanaman, dan karakteristik lainnya. Oleh karena itu, korelasi yang ditemukan tidak dapat langsung diinterpretasikan sebagai hubungan sebab-akibat.

**Rekomendasi:**
- Melakukan evaluasi terhadap jumlah pohon produktif pada setiap blok.

### 3. Low Productivity and Area Outlier Assessment — 2024

Berdasarkan hasil pemeringkatan produktivitas pada sheet `Clear_Block_Performance`, blok **B011** teridentifikasi sebagai salah satu blok dengan produktivitas rendah pada tahun 2024 dan termasuk dalam kategori outlier pada variabel `Area_Ha`.

Kondisi ini perlu mendapatkan perhatian karena ketidakakuratan pencatatan luas lahan dapat memengaruhi hasil perhitungan produktivitas per hektare dan posisi peringkat blok.

**Rekomendasi:**
- Memprioritaskan validasi luas lahan blok B011.
- Menghitung ulang produktivitas serta mengevaluasi perubahan peringkat setelah proses validasi.

### 4. Low Productivity and Low Palm Density Assessment — 2024

Dari 10 blok dengan peringkat produktivitas terendah pada tahun 2024, ditemukan bahwa **delapan blok memiliki kepadatan pohon (`Palms_per_Ha`) di bawah lower limit** berdasarkan batas statistik yang digunakan dalam analisis.

Temuan ini mengindikasikan adanya populasi pohon produktif yang relatif rendah dibandingkan distribusi kepadatan pada blok-blok yang dianalisis.

**Rekomendasi:**
- Memeriksa kemungkinan adanya pohon mati, tidak produktif, atau area yang belum ditanami.
- Mengevaluasi kondisi dan pola penanaman pada blok terkait.

### 5. Further Operational Assessment on Low Productivity Blocks

Tiga blok lainnya dalam kelompok sebelas blok dengan produktivitas terendah pada tahun 2024 tidak menunjukkan indikasi kepadatan pohon di bawah lower limit. Dengan demikian, rendahnya produktivitas pada ketiga blok tersebut belum dapat dijelaskan melalui indikator kepadatan pohon saja.

Diperlukan pemeriksaan terhadap faktor operasional dan lingkungan yang berpotensi memengaruhi produksi.

**Rekomendasi:**
- Mengevaluasi kondisi kesehatan dan perkembangan tanaman.
- Memeriksa pelaksanaan pemupukan, termasuk dosis dan jadwal aplikasi.
- Meninjau kualitas panen serta potensi kehilangan hasil panen.
- Mempertimbangkan faktor lingkungan seperti curah hujan, drainase, dan kondisi tanah.

## Overall Conclusion and Operational Recommendations

Hasil analisis menunjukkan beberapa aspek yang perlu mendapatkan perhatian dalam evaluasi kinerja perkebunan kelapa sawit, yaitu kualitas data luas lahan, hubungan kepadatan pohon produktif dengan total produksi, serta variasi produktivitas antarblok.

Berdasarkan temuan tersebut, tindakan evaluasi direkomendasikan berdasarkan tiga prioritas:

1. **Data validation:** Memvalidasi luas lahan pada blok yang teridentifikasi sebagai outlier, khususnya B011.
2. **Plant population assessment:** Memeriksa jumlah dan kondisi pohon produktif pada delapan blok dengan kepadatan di bawah lower limit.
3. **Operational assessment:** Mengevaluasi kondisi tanaman, pemupukan, dan kualitas panen pada tiga blok lainnya.

Analisis lebih lanjut menggunakan data pemupukan, kondisi tanah, curah hujan, dan kualitas panen diperlukan untuk memperoleh pemahaman yang lebih mendalam mengenai faktor-faktor yang memengaruhi produktivitas perkebunan.
