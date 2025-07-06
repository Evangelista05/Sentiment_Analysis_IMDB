# Analisis Sentimen pada Dataset IMDB: Perbandingan Model LSTM vs CNN

## Ringkasan Proyek

Proyek ini bertujuan untuk melakukan **klasifikasi sentimen biner** (positif atau negatif) terhadap ulasan film dari dataset **IMDB** menggunakan dua pendekatan deep learning: **Long Short-Term Memory (LSTM)** dan **Convolutional Neural Network (CNN)**. Proyek ini juga membandingkan performa kedua arsitektur dalam hal akurasi dan loss.

Notebook ini dikembangkan sebagai bagian dari tes teknis dan menunjukkan kemampuan saya dalam:
- Menangani tugas Natural Language Processing (NLP)
- Melakukan pra-pemrosesan data teks
- Membangun, melatih, dan mengevaluasi model LSTM dan CNN menggunakan TensorFlow/Keras
- Menyajikan hasil analisis secara jelas dan sistematis

---

##  Permasalahan

Dataset IMDB terdiri dari 50.000 ulasan film yang telah diberi label sebagai **positif** atau **negatif**. Tugas utama dari proyek ini adalah:
- Melakukan pra-pemrosesan data teks agar bisa digunakan oleh model deep learning
- Melatih dan mengevaluasi dua arsitektur model berbeda (LSTM dan CNN)
- Membandingkan efektivitas keduanya dalam melakukan klasifikasi sentimen

---

##  Arsitektur Model

### 1. LSTM (Long Short-Term Memory)
- Merupakan jenis Recurrent Neural Network (RNN) yang mampu memahami konteks jangka panjang dalam data urutan (sequence).
- Cocok untuk data teks seperti kalimat dan dokumen panjang.
- Struktur:
  - Layer Embedding
  - Layer LSTM
  - Dense Output (Sigmoid)

### 2. CNN (Convolutional Neural Network)
- Mampu mengenali pola lokal dalam teks (misalnya frasa) dan memiliki waktu pelatihan lebih cepat dari RNN.
- Struktur:
  - Layer Embedding
  - Layer Conv1D
  - Global Max Pooling
  - Dense Output (Sigmoid)

---

##  Tools & Library yang Digunakan

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Google Colab

---

##  Metode Evaluasi

- **Akurasi**: Mengukur tingkat ketepatan model.
- **Loss (Binary Crossentropy)**: Mengukur kesalahan prediksi.
- Visualisasi dilakukan melalui grafik akurasi dan loss pada proses pelatihan dan validasi.

---

## Hasil Singkat

| Model | Akurasi Pengujian | Catatan |
|-------|-------------------|---------|
| LSTM  | ~86%              | Unggul dalam memahami konteks jangka panjang |
| CNN   | ~85%              | Pelatihan lebih cepat, efektif pada pola pendek |

> Model LSTM menunjukkan performa sedikit lebih baik dibanding CNN, namun keduanya cukup andal untuk tugas klasifikasi sentimen.


---

##  Kesimpulan

Proyek ini memperlihatkan bagaimana deep learning dapat digunakan untuk memahami sentimen dari data teks, serta pentingnya memilih arsitektur yang tepat untuk tugas tertentu. Harapannya, proyek ini bisa menjadi gambaran atas kemampuan teknis saya, kemampuan analisis, dan cara saya menyajikan data secara profesional.

Terima kasih telah meluangkan waktu untuk membaca proyek saya!
