**Data Science Project: Prediksi Harga Rumah Second di Depok**

### Business Understanding

Kota Depok, sebagai salah satu kawasan urban yang berkembang pesat di Indonesia, menghadapi peningkatan permintaan terhadap rumah second. Dengan pertumbuhan populasi yang cepat, pasar real estate di Depok menawarkan berbagai peluang, terutama pada segmen rumah second. Oleh karena itu, penting untuk menganalisis faktor-faktor yang memengaruhi harga rumah second dan mengembangkan model prediktif yang dapat membantu berbagai pihak terkait.

### Permasalahan Bisnis

Pemilik rumah, calon pembeli, dan agen properti sering menghadapi tantangan dalam menentukan harga rumah second yang sesuai dengan kondisi pasar saat ini. Beberapa permasalahan utama yang dihadapi adalah:

1. **Penetapan Harga yang Tidak Akurat:** Harga rumah yang terlalu tinggi atau terlalu rendah dapat mengakibatkan kerugian finansial.
2. **Keterbatasan Informasi:** Calon pembeli dan agen sering kekurangan data yang dapat diandalkan untuk memprediksi harga properti.
3. **Persaingan Pasar yang Ketat:** Dengan meningkatnya jumlah properti yang tersedia, penentuan harga yang kompetitif menjadi sangat penting.

### Cakupan Proyek

1. **Mengumpulkan dan memproses data** melalui web scraping dari situs jual beli rumah untuk mendapatkan informasi seperti jumlah kamar tidur, luas tanah, luas bangunan, jenis sertifikat rumah, dan lokasi kecamatan.
2. **Menganalisis data** untuk mengidentifikasi faktor-faktor yang paling memengaruhi harga rumah second.
3. **Membangun model prediktif** dengan mencari berbagai algoritma machine learning.
4. **Membuat aplikasi web** untuk memprediksi harga rumah second di Depok berdasarkan input pengguna.
5. **Memberikan rekomendasi** kepada pemilik rumah, calon pembeli, dan agen properti untuk penetapan harga yang lebih baik.

### Persiapan

#### Sumber Data
Data historis harga rumah second di Depok yang mencakup kolom-kolom berikut:
- **Jumlah Kamar Tidur**
- **Luas Tanah**
- **Luas Bangunan**
- **Jenis Sertifikat Rumah**
- **Lokasi Kecamatan**

#### Setup Environment

Untuk memulai, berikut adalah langkah-langkah untuk menyiapkan lingkungan kerja:

1. **Buka terminal atau PowerShell.**
2. **Jalankan perintah berikut untuk membuat virtual environment:**
   ```bash
   conda create --name prediksi_harga python=3.9
   ```
3. **Aktifkan virtual environment:**
   ```bash
   conda activate prediksi_harga
   ```
4. **Instal library yang dibutuhkan:**
   ```bash
   pip install streamlit==1.40.1 pandas==2.2.2 joblib==1.4.2 scikit-learn==1.5.2
   ```
5. **Buka Jupyter Notebook:**
   ```bash
   jupyter-notebook
   ```
6. **Buka file Python `prediction.py`.**
7. **Masukkan data pada variabel input dan jalankan kode untuk melihat hasil prediksi.**
8. **Atau akses aplikasi Streamlit pada tautan berikut:**
   [https://prediksirumah-depok.streamlit.app/](https://prediksirumah-depok.streamlit.app/)

### Conclusion

Dari analisis yang dilakukan, beberapa temuan penting adalah:

1. **Kecamatan dengan Harga Rata-Rata Tertinggi:**
   - Empat dari lima kecamatan dengan harga rata-rata rumah second tertinggi di Depok (Cinere, Beji, Cimanggis, dan Limo) bersebelahan langsung dengan Jakarta Selatan, yang memengaruhi nilai jual rumah.

2. **Faktor yang Memengaruhi Harga:**
   - Data numerik:
     1. Luas Tanah
     2. Luas Bangunan
     3. Jumlah Kamar Tidur
   - Data kategorikal:
     1. Jenis Sertifikat
     2. Lokasi Kecamatan

3. **Model Prediktif:**
   - Model regresi linier memberikan prediksi harga rumah dengan mempertimbangkan faktor-faktor di atas.

### Rekomendasi Action Items

1. **Fokus pada Lokasi Strategis:**
   - Promosikan rumah di kecamatan seperti Cinere, Beji, Cimanggis, dan Limo yang memiliki potensi nilai jual lebih tinggi.

2. **Optimalisasi Faktor Utama:**
   - Perhatikan luas tanah dan bangunan sebagai faktor utama dalam menentukan harga rumah.



