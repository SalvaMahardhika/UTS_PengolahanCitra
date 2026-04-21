# Face Mask Detection using MobileNetV2 and YOLOv8 😷

## 📌 Deskripsi
Project ini bertujuan untuk mendeteksi penggunaan masker pada wajah menggunakan teknologi computer vision.  

Metode yang digunakan:
- MobileNetV2 (klasifikasi citra)
- YOLOv8 (deteksi objek)

Mendukung SDG 3 (Good Health and Well-Being).

---

## 🎯 Tujuan
- Mengembangkan sistem deteksi masker
- Mengimplementasikan MobileNetV2 dan YOLOv8
- Membandingkan performa model

---

## 🗂️ Dataset
- Face Mask Detection Dataset (Kaggle)
- Kelas:
  - with_mask
  - without_mask

---

## ⚙️ Pipeline

Dataset → Preprocessing → Training → Evaluation → Comparison

### MobileNetV2
Crop wajah → Resize (224x224) → Training → Output label

### YOLOv8
Convert ke format YOLO → Training → Output bounding box + label

---

## 🧠 Model

### MobileNetV2
- Klasifikasi citra
- Input: 224x224

### YOLOv8
- Deteksi objek
- Multi-face detection

---

## 📊 Hasil Evaluasi

| Model        | Accuracy | Precision | Recall |
|-------------|---------|----------|--------|
| MobileNetV2 | 76.77%  | 72.30%   | 76.77% |
| YOLOv8      | 61.44%  | 71.75%   | 51.12% |

---

## 🔍 Analisis
- MobileNetV2 unggul pada akurasi klasifikasi
- YOLOv8 unggul pada deteksi multi-objek dan real-time

---

## 🚀 Cara Menjalankan

### Install Dependency
pip install ultralytics tensorflow opencv-python matplotlib

### Train YOLO
yolo detect train data=data.yaml model=yolov8n.pt epochs=5 imgsz=224

---

## 📁 Struktur Folder

project/
├── dataset/
├── mobilenet.ipynb
├── yolo.ipynb
├── data.yaml
├── runs/
└── README.md

---

## 👨‍💻 Author
- Salva Mahardhika Pratama  
- Alfonsus William Hamonangan Sinaga
