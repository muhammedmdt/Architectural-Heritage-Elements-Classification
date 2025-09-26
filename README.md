# Architectural-Heritage-Elements-Classification
Architectural Heritage Elements Classification - Akbank Derin Öğrenme Bootcamp Projesi - Mimari Miras Elemanları Sınıflandırması
# Architectural Heritage Elements Classification 🏛️

Akbank Derin Öğrenme Bootcamp Projesi - Mimari Miras Elemanları Sınıflandırması

## 📊 Proje Özeti

Bu projede, 10 farklı mimari miras elemanının görüntülerden otomatik olarak sınıflandırılması için bir derin öğrenme modeli geliştirilmiştir.

| Metric | Değer |
|--------|-------|
| **Test Accuracy** | 77.71% |
| **Test Loss** | 0.6661 |
| **Sınıf Sayısı** | 10 |
| **Model Tipi** | CNN |

## 🏗️ Mimari Elemanlar

- altar (sunak)
- apse (apsis) 
- bell_tower (çan kulesi)
- column (sütun)
- dome(inner) (iç kubbe)
- dome(outer) (dış kubbe)
- flying_buttress (uçan payanda)
- gargoyle (grotesk)
- stained_glass (vitray)
- vault (tonoz)

## 📈 Model Performansı

### Confusion Matrix
<img width="938" height="760" alt="image" src="https://github.com/user-attachments/assets/90883902-1c07-40bf-ae2c-381dd9d07e49" />


### Eğitim Grafikleri
<img width="1197" height="381" alt="image" src="https://github.com/user-attachments/assets/0e0243c4-1b8c-4d5a-aff4-4d5214cc1f53" />


### Sınıf Bazlı Doğruluk
<img width="994" height="460" alt="image" src="https://github.com/user-attachments/assets/5e9b93c8-9531-4de5-8fe1-1c60ccb20bb3" />


## 🔍 Grad-CAM Analizi

### Grad-CAM Sonuçları
<img width="1029" height="338" alt="image" src="https://github.com/user-attachments/assets/48ba035c-5410-4771-90cb-5ec08365c14f" />


### Hiperparametre Optimizasyonu
<img width="1240" height="395" alt="image" src="https://github.com/user-attachments/assets/226f8865-51cc-49c7-817d-0ffefa7bf4f5" />


## 🚀 Proje Adımları

### 1. Veri Ön İşleme
- Görüntülerin 224x224 boyutuna dönüştürülmesi
- Data Augmentation (rotation, flip, zoom)
- Train/Validation/Test split (%80/%10/%10)

### 2. CNN Modeli
python
Model: Sequential
├── Conv2D(32) -> BatchNorm -> MaxPooling -> Dropout
├── Conv2D(64) -> BatchNorm -> MaxPooling -> Dropout  
├── Conv2D(128) -> BatchNorm -> MaxPooling -> Dropout
└── Dense(512) -> Dropout -> Dense(10) -> Softmax

3. Model Değerlendirme
Accuracy: 77.71%

Loss: 0.6661

Confusion Matrix analizi

Sınıf bazlı accuracy değerlendirmesi

4. Grad-CAM Görselleştirme
Model karar mekanizmasının analizi

Problemli sınıfların tespiti (bell_tower, flying_buttress)

5. Hiperparametre Optimizasyonu
Learning Rate tuning

Dropout oranı optimizasyonu

Batch Size optimizasyonu

🔧 Teknolojiler
Python 3.11

TensorFlow/Keras

OpenCV

Matplotlib/Seaborn

Scikit-learn

👤 Author
Muhammed Durmuş TOPRAK

Akbank Derin Öğrenme Bootcamp Katılımcısı

🔗 Links
Kaggle Notebook: https://www.kaggle.com/code/muhammedmdt/notebook0c7e813cbf/edit

Dataset: https://www.kaggle.com/datasets/xhlulu/archi-heritage-elements


