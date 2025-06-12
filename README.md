# 🔍 CNN Buatan vs AlexNet pada Dataset CIFAR-10

Proyek ini bertujuan untuk **membandingkan performa arsitektur Convolutional Neural Network (CNN) buatan sendiri dengan AlexNet** dalam menyelesaikan tugas klasifikasi gambar menggunakan dataset **CIFAR-10**.

---

## 📦 Dataset

- **CIFAR-10** berisi 60.000 gambar berwarna berukuran 32x32 piksel, terbagi dalam 10 kelas.
- Terdiri dari 50.000 data latih dan 10.000 data uji.
- Kelas-kelas: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck.

---

## 🧠 Arsitektur Model

### 1. CNN (Baseline)
Model sederhana dengan 2 layer konvolusi, max pooling, dan fully connected layer.

### 2. AlexNet
Versi modifikasi dari AlexNet yang disesuaikan dengan ukuran CIFAR-10 (32x32). Memiliki lebih banyak lapisan dan parameter dibanding CNN biasa.

### 3. CNN2 (Model Perbaikan)
Versi yang ditingkatkan dari CNN awal:
- 3 blok konvolusi
- Batch Normalization
- Dropout
- Fully Connected Layer yang lebih besar

---

## 🏃 Strategi Pelatihan

- Optimizer: Adam
- Loss Function: CrossEntropyLoss
- Epoch: 25
- Augmentasi Data: RandomCrop, HorizontalFlip
- Metrik Evaluasi: Accuracy, Precision, Recall, F1 Score (Macro)

---

## 📊 Hasil Evaluasi

| Model   | Akurasi    | F1 Score (Macro) |
|---------|------------|------------------|
| CNN     | 72.34%     | 71.93%           |
| AlexNet | 77.70%     | 77.81%           |
| CNN2    | **84.94%** | **84.91%**       |

✅ **Model CNN2 menunjukkan performa terbaik dibandingkan CNN awal dan AlexNet**, baik dari segi akurasi maupun F1 Score.

---

## 🔍 Visualisasi Grad-CAM

Grad-CAM digunakan untuk melihat area fokus model ketika membuat prediksi. Hasil menunjukkan bahwa **CNN2 memiliki area perhatian yang lebih tepat pada objek utama**, sementara CNN awal dan AlexNet cenderung lebih menyebar.

---


---

## 🧪 Kesimpulan

Melalui proyek ini, dapat disimpulkan bahwa **arsitektur CNN yang lebih sederhana dari AlexNet tetap dapat memberikan hasil lebih baik** jika menggunakan teknik seperti **Batch Normalization**, **Dropout**, dan penambahan kedalaman yang seimbang.

---

## 📚 Referensi

- Dataset CIFAR-10: https://www.cs.toronto.edu/~kriz/cifar.html  
- Paper AlexNet: [ImageNet Classification with Deep Convolutional Neural Networks](https://papers.nips.cc/paper_files/paper/2012/file/c399862d3b9d6b76c8436e924a68c45b-Paper.pdf)  
- Grad-CAM: https://arxiv.org/abs/1610.02391

---

## 👤 Penulis

- Nama: *[Dani Hidayat]*
- Institusi: *UIN Syarif Hidayatullah Jakarta*
- Proyek ini dibuat untuk keperluan pembelajaran dan eksperimen dalam bidang CNN.


