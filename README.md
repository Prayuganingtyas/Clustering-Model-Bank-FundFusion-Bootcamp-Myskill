# Clustering-Model-Bank-FundFusion-Bootcamp-Myskill
This project was developed as part of my learning experience in the Data Analyst Bootcamp at Myskill, where I focused on applying Python code for Clustering Model analysis.

### **PROBLEM STATEMENT**

Belum memiliki strategi yang tepat untuk menawarkan jenis produk yang sesuai dengan segmen calon nasabah yang akan direkrut

### **OBJECTIVE**

Membuat Sebuah Model Clustering untuk mengetahui kepemilikan produk berdasarkan demografi nasabah yang saat ini sudah menggunakan layanan FundFusion dengan Silhouette Score >0.7


### **VARIABEL YANG TERSEDIA**

Dari dataset yang dimiliki terdapat beberapa data yang tersedia:


---
**1. GCIF                     :** Unique Identifier Nasabah\
**2. Area                     :** Lokasi Nasabah (Jakarta,Bogor,Bandung,Surabaya,Jogja,Solo)\
**3. Jalur_Pembukaan          :** Touch Points Nasabah membuka produk --> Cabang, Telemarketing, Aplikasi Digital, Internet Banking\
**4. Vintage                  :** Durasi Menjadi Nasabah (Sejak membuka akun)\
**5. Usia                     :** Usia Nasabah\
**6. Jenis_Kelamin            :** Laki-laki (1) & Perempuan (0)\
**7. Status_Perkawinan        :** Belum Menikah (0), Menikah (1), Cerai (2), Janda/Duda (3)\
**8. Jumlah_Anak              :** Jumlah Anak Nasabah (numerik)\
**9. Pendidikan               :** Status Pendidikan Terakhir --> Tidak Memiliki Pendidikan Formal (0), SD (1), SMP (2), SMA (3), Sarjana (4), Magister (5), Doktor (6)\
**10. Produk_Tabungan         :** Status Kepemilikan Produk (Yes/1, No/0)\
**11. Produk_Deposito         :** Status Kepemilikan Produk (Yes/1, No/0)\
**12. Produk_Kartu_Kredit     :** Status Kepemilikan Produk (Yes/1, No/0)\
**13. Produk_Kredit_Rumah     :** Status Kepemilikan Produk (Yes/1, No/0)\
**14. Produk_Kredit_Kendaraan :** Status Kepemilikan Produk (Yes/1, No/0)\
**15. Produk_Kredit_Dana_Tunai:** Status Kepemilikan Produk (Yes/1, No/0)\
**16. Total_Kepemilikan_Produk:** Jumlah Produk Yang Dimiliki (Penjumlahan dari Produk2)\
**17. Pendapatan_Tahunan      :** Rata-rata Pendapatan Dalam Setahun\
**18. Total_Relationship_Balance :** Total Asset Nasabah dalam Cutoff Bulan Observasi\





# **EXPERIMENT**

Point of View:
1. Dikelompokkan berdasarkan demografis untuk dicari pattern kepemilikan produk
2. Dikelompookan berdasarkan kepemilikan produk untuk dicari patter berdasarkan demografisnya

# **SARAN DAN KESIMPULAN**

## Saran

### **1. Kluster 0:**
   - **Profil:** Memiliki total balance sangat tinggi (sekitar 400 juta) dan rata-rata jumlah anak yang relatif kecil. Nasabah di kluster ini sudah banyak memiliki produk tabungan dan deposito.
   - **Strategi Penawaran Produk:**
     - **Deposito Premium:** Tingkatkan penawaran deposito dengan suku bunga kompetitif, mengingat mereka memiliki balance tinggi.
     - **Kartu Kredit dengan Limit Tinggi:** Tawarkan kartu kredit premium dengan limit yang lebih tinggi dan program rewards eksklusif untuk meningkatkan penggunaan.
     - **Kredit Rumah atau Kendaraan Mewah:** Dengan total balance yang tinggi, nasabah ini mungkin tertarik pada kredit rumah atau kredit kendaraan mewah.

### **2. Kluster 1:**
   - **Profil:** Memiliki total balance menengah (sekitar 172 juta) dan rata-rata jumlah anak mirip dengan kluster lain. Mereka dominan memiliki tabungan dan deposito, tetapi penggunaan kartu kredit dan kredit rumah masih rendah.
   - **Strategi Penawaran Produk:**
     - **Kredit Rumah:** Dorong kepemilikan kredit rumah dengan menawarkan skema pembiayaan yang terjangkau.
     - **Kartu Kredit dengan Promosi Menarik:** Tawarkan kartu kredit dengan cashback atau poin rewards untuk meningkatkan daya tarik.
     - **Deposito Berjangka:** Untuk nasabah yang mencari investasi aman, tawarkan deposito berjangka dengan bunga kompetitif.

### **3. Kluster 2:**
   - **Profil:** Total balance menengah ke atas (sekitar 284 juta), dengan rata-rata jumlah anak sedikit lebih tinggi dari kluster lainnya. Produk utama mereka adalah tabungan dan kredit rumah.
   - **Strategi Penawaran Produk:**
     - **Bundling Produk Tabungan dan Deposito:** Tawarkan bundling tabungan dan deposito untuk meningkatkan kepemilikan produk investasi yang aman.
     - **Kredit Kendaraan:** Kluster ini berpotensi untuk produk kredit kendaraan, terutama bagi mereka yang sudah memiliki rumah.
     - **Kartu Kredit dengan Limit Menengah:** Tawarkan kartu kredit dengan limit menengah dan program rewards yang berfokus pada kebutuhan sehari-hari.

### **4. Kluster 3:**
   - **Profil:** Memiliki total balance yang relatif rendah (sekitar 59 juta) dan jumlah anak yang sedikit lebih tinggi dari rata-rata. Produk utama mereka adalah tabungan dan kredit rumah, sedangkan kartu kredit kurang diminati.
   - **Strategi Penawaran Produk:**
     - **Kredit Kendaraan atau Kredit Dana Tunai:** Tawarkan kredit kendaraan atau dana tunai dengan suku bunga ringan, mengingat kluster ini mungkin memerlukan dukungan finansial untuk kebutuhan sehari-hari.
     - **Program Tabungan Berkelanjutan:** Berikan program menabung dengan setoran rutin yang otomatis untuk mendorong akumulasi balance.
     - **Kartu Kredit Dasar:** Tawarkan kartu kredit dengan limit rendah dan biaya tahunan minimal, terutama bagi nasabah yang belum memiliki kartu kredit.

### **5. Kluster 4:**
   - **Profil:** Memiliki total balance yang sangat tinggi (sekitar 607 juta) dengan jumlah anak yang lebih tinggi. Kluster ini memiliki ketertarikan tinggi pada semua produk, termasuk tabungan, deposito, kartu kredit, dan kredit rumah.
   - **Strategi Penawaran Produk:**
     - **Kredit Rumah Eksklusif:** Tawarkan produk kredit rumah dengan bunga khusus dan layanan tambahan, mengingat minat tinggi terhadap kredit rumah.
     - **Kartu Kredit Premium dengan Fasilitas Eksklusif:** Tawarkan kartu kredit premium yang memberikan akses ke program eksklusif, seperti lounge bandara atau cashback khusus.
     - **Kredit Kendaraan atau Dana Tunai dengan Suku Bunga Kompetitif:** Nasabah dengan total balance tinggi bisa jadi tertarik dengan produk kredit kendaraan atau kredit dana tunai yang memberikan fleksibilitas pembiayaan.

### **Kesimpulan:**
Dengan strategi yang disesuaikan seperti di atas, klien dapat menawarkan produk yang lebih relevan bagi setiap kluster nasabah:

1. **Kluster 0** – Fokus pada produk investasi, kredit rumah, dan kartu kredit premium.
2. **Kluster 1** – Fokus pada kredit rumah, deposito berjangka, dan kartu kredit dengan promosi menarik.
3. **Kluster 2** – Dorong kredit kendaraan dan bundling produk tabungan dan deposito.
4. **Kluster 3** – Utamakan kredit kendaraan atau dana tunai, serta kartu kredit dengan limit rendah.
5. **Kluster 4** – Sasar produk kredit rumah eksklusif, kartu kredit premium, dan kredit kendaraan atau dana tunai kompetitif.

Dari hasil clustering, yang menjadi pembeda adalah Total Relationship Balance. Namun, bila hanya dari segi Total Relationship Balance kita belum bisa melakukan segmentasi nasabah dengan baik (dilihat dari silhouette score yang masih belum mencapai 0.7). Hal yang dapat dilakukan ke depannya adalah dengan memperbanyak variabel dan melakukan iterasi lebih banyak.

