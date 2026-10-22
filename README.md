# Klasifikasi Spesies Iris Menggunakan Random Forest

Repositori ini mengandungi kod pelaksanaan untuk analisis penerokaan data dan pembinaan model pembelajaran mesin bagi mengelaskan spesies bunga Iris berdasarkan ukuran sepal dan kelopak.

## **1. Gambaran Keseluruhan Projek**
* **Dataset:** Menggunakan fail `IRIS.csv` yang mengandungi 150 sampel data dengan 4 ciri ukuran dan 3 kategori spesies[cite: 7].
* **Pra-pemprosesan (Preprocessing):** 
  * Membahagikan data kepada set latihan (*train*) dan ujian (*test*) pada nisbah 80:20 menggunakan `train_test_split` dengan tetapan *stratify*[cite: 7].
  * Melakukan penskalaan nilai ciri menggunakan `StandardScaler` bagi memastikan keseragaman skala data[cite: 7].
* **Model Pembelajaran Mesin:** Menggunakan algoritma *Random Forest Classifier* dengan parameter kedalaman maksimum `max_depth=4`[cite: 7].

---

## **2. Struktur Kod & Aliran Kerja**
1. **Pemuatan Pustaka & Data:** Mengimport modul penting seperti `pandas`, `numpy`, `matplotlib`, dan `StandardScaler`, serta membaca dataset `IRIS.csv`[cite: 7].
2. **Analisis Terokai Data (EDA):** Memeriksa struktur data, jenis data, statistik deskriptif, serta taburan kelas menggunakan fungsi seperti `df.info()`, `df.describe()`, dan `value_counts()`[cite: 7].
3. **Penyediaan Data:** Memisahkan pemboleh ubah input (`input_df`) dan sasaran (`output_df`) sebelum melalui proses pembahagian dan penskalaan[cite: 7].
4. **Latihan & Ramalan Model:** Melatih model `RandomForestClassifier` menggunakan data latihan yang telah disiar skala dan membuat ramalan pada data ujian[cite: 7].
5. **Evaluasi Model:** Menilai prestasi model menggunakan `classification_report` untuk mendapatkan nilai *precision*, *recall*, dan *f1-score*[cite: 7].

---

## **3. Keperluan Sistem & Pustaka**
Pastikan pustaka Python berikut telah dipasang sebelum menjalankan kod:
```bash
pip install pandas numpy matplotlib scikit-learn
