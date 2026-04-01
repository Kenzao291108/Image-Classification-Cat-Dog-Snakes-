# Animal Image Classifier (Cats, Dogs, Snakes) 🐱🐶🐍

Proyek ini merupakan sistem klasifikasi gambar hewan (kucing, anjing, ular) menggunakan transfer learning dengan MobileNetV2. Model dikembangkan menggunakan TensorFlow dan diekspor ke format SavedModel, TensorFlow Lite (TFLite), dan TensorFlow\.js (TFJS) agar bisa digunakan di berbagai platform seperti server, mobile, dan browser.

---

## 📁 Struktur Folder

```
submission/
├── tfjs_model/
│   ├── group1-shard1of1.bin
│   └── model.json
├── tflite/
│   ├── model.tflite
│   └── label.txt
├── saved_model/
│   ├── saved_model.pb
│   └── variables/
├── dataset/
│   └── Animals.zip
├── notebook.ipynb
├── README.md
└── requirements.txt
```

---

## 🚀 Fitur Proyek

- Data Augmentation & Preprocessing menggunakan `ImageDataGenerator`
- Transfer Learning menggunakan MobileNetV2 (pretrained ImageNet)
- Fine-tuning pada beberapa layer atas MobileNetV2
- Evaluasi menggunakan Classification Report (precision, recall, f1-score)
- Ekspor model ke:
  - SavedModel (standar TensorFlow)
  - TensorFlow Lite (.tflite) untuk mobile/embedded
  - TensorFlow\.js (.json + .bin) untuk browser

---

## 🛠️ Cara Menjalankan Proyek

1. **Clone repo / buka notebook**

2. **Install library yang diperlukan**

   ```bash
   pip install -r requirements.txt
   ```

3. **Dataset**

   - Struktur folder dataset:
     ```
     Animals/
     ├── cats/
     ├── dogs/
     └── snakes/
     ```
   - Tempatkan dataset di dalam direktori `/content/Animals` jika menggunakan Google Colab.

4. **Jalankan notebook**

   - Notebook akan melakukan training, fine-tuning, evaluasi, dan export model.

---

## 🛆 Output

- **saved\_model/** : untuk deployment di server atau cloud
- **tflite/** : untuk deployment di perangkat mobile/embedded
- **tfjs\_model/** : untuk deployment di aplikasi berbasis browser

---

## 🔗 Dependencies

- TensorFlow >= 2.x
- TensorFlow\.js converter
- Scikit-learn
- Numpy

---

## ✨ Credits

Dikembangkan oleh Dzulfikar Ibnu dari MS-02 untuk keperluan tugas proyek Machine Learning.

---

