# Titanic Yolcu Hayatta Kalma Tahmini

Bu proje, **Akbank Gençlik Akademisi & Global AI Hub** tarafından düzenlenen Makine Öğrenmesi Bootcamp'inde bir bitirme projesi olarak geliştirilmiştir. Projenin amacı, Titanic gemisindeki yolcuların hayatta kalıp kalmayacağını makine öğrenmesi algoritmaları ile tahmin etmektir.

---

## 📊 Kullanılan Veri Seti

Veri seti, `seaborn` kütüphanesindeki hazır **Titanic** veri setidir. Yolcuların yaş, cinsiyet, sınıf gibi özelliklerine göre `survived` (0 = hayatta kalmadı, 1 = hayatta kaldı) değişkeni tahmin edilmeye çalışılmıştır.

---

## 🧠 Uygulanan Adımlar

- **Veri analizi (EDA)**: Eksik veriler, değişken dağılımları ve korelasyonlar incelendi.
- **Veri ön işleme**:
  - Eksik veriler ortalama / mod ile dolduruldu.
  - Kategorik değişkenler sayısal forma çevrildi (Label Encoding).
  - Veriler eğitim ve test setine ayrıldı.
- **Model eğitimi**:
  - Logistic Regression algoritması kullanıldı.
  - GridSearchCV ile hiperparametre optimizasyonu yapıldı.
- **Model değerlendirme**:
  - Accuracy: **%79.3**
  - Sınıflandırma Raporu ve Confusion Matrix yorumlandı.

---

## 🔧 Kullanılan Teknolojiler

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn (sklearn)
- Google Colab (geliştirme ortamı)

---

## 📈 Model Performansı

| Metric       | Value  |
|--------------|--------|
| Accuracy     | 79.3%  |
| Precision    | 80% (class 0) / 78% (class 1) |
| Recall       | 87% (class 0) / 69% (class 1) |

Model, "hayatta kalmayan" yolcuları daha yüksek doğrulukla tahmin etmektedir.

---

## 🔗 Bağlantılar

- 📁 [Notebook dosyası (Kaggle)](https://www.kaggle.com/code/alihamzapeenek/titanic-survival-prediction-logistic-regression)
- 📌 [Proje Raporu (.ipynb)](./titanic_survival_prediction.ipynb)

---

## 🚀 Geliştirme Fikirleri

- Sınıf dengesizliği için `SMOTE` veya `class_weight='balanced'` gibi teknikler denenebilir.
- Streamlit ile basit bir kullanıcı arayüzü geliştirilebilir.
- Daha karmaşık modeller (Random Forest, XGBoost) test edilebilir.

---

## 🧑‍🎓 Katılımcı

- Ali Hamza Peçenek (Türk-Alman Üniversitesi, Bilgisayar Mühendisliği 2. Sınıf Öğrencisi)
- hamza.petschenek@gmail.com
