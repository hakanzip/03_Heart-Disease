# Kalp Hastalığı Tahmini - Makine Öğrenmesi Projesi

Bu projede, çeşitli hasta verileri kullanılarak kişilerin kalp hastalığı riski taşıyıp taşımadığını tahmin etmek amaçlanmıştır. Proje kapsamında veri analizi, görselleştirme, özellik mühendisliği ve farklı sınıflandırma modelleri uygulanmıştır.

## Veri Seti

Kaynak: [Heart Disease UCI - Kaggle]https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction  
Kullanılan dosya: heart.csv

## Proje Aşamaları

1. Veri Analizi ve Görselleştirme (EDA - Exploratory Data Analysis)  
   Yaş, cinsiyet, göğüs ağrısı tipi, egzersiz sırasında göğüs ağrısı gibi değişkenlerin kalp hastalığı ile ilişkileri analiz edilmiştir.  
   Sayısal değişkenler için dağılım grafikleri, kategorik değişkenler için oran analizleri yapılmıştır.

2. Özellik Mühendisliği (Feature Engineering)  
   Yeni değişkenler oluşturulmuş, kategorik değişkenler sayısallaştırılmış ve bazı sütunlar yeniden adlandırılmıştır.  
   Eksik değer kontrolü, aykırı değer tespiti ve gruplama işlemleri uygulanmıştır.

3. Modelleme (Model Training)  
   Lojistik regresyon, Random Forest ve XGBoost gibi sınıflandırma algoritmaları eğitilmiş, ROC eğrileri oluşturulmuştur.

4. Değerlendirme (Evaluation)  
   Accuracy, precision, recall, F1 skoru gibi metriklerle model başarıları değerlendirilmiştir.  
   ROC eğrileri karşılaştırmalı olarak sunulmuştur.

## Kullanılan Kütüphaneler

pandas  
numpy  
seaborn  
matplotlib  
scikit-learn  
os  
sys  
platform  
warnings  
importlib  

## Proje Yapısı

03_Heart-Disease/  
├── data/  
│   └── heart.csv  
├── notebook/  
│   └── heart_disease.ipynb  
├── images/  
│   ├── yas_dagilimi.png  
│   ├── cinsiyete_gore_kalp_hastaligi.png  
│   ├── gogus_agrisi_turleri_kalp_hastaligi.png  
│   ├── ekg_sonucu_kalp_hastaligi.png  
│   ├── egzersiz_gogus_agrisi_kalp_hastaligi.png  
│   ├── yas_grubu_kalp_hastaligi_orani.png  
│   ├── korelasyon_matrisi.png  
│   ├── onemli_5_ozellik.png  
│   └── roc_egirisi.png  
├── README.md  
├── requirements.txt  
└── .gitignore

## Notlar

Bu proje, sağlık verileri üzerinden sınıflandırma problemlerinin çözümüne dair temel bir örnektir.  
Modelleme süreci boyunca veri sızıntısı engellenmiş, eğitim ve test ayrımı dikkatle yapılmıştır.