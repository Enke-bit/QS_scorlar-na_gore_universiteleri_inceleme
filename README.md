# QS Dünya Üniversite Sıralamaları - Veri Analizi ve Tahminleme

Bu proje, QS Dünya Üniversite Sıralamaları verilerini analiz ederek QS Genel Skorunu tahmin etmeyi amaçlamaktadır. Proje, kapsamlı veri keşfi, görselleştirme ve model karşılaştırmalarını içermektedir. En iyi performans gösteren model, kullanıcıdan veri alarak tahmin yapabilen bir Tkinter tabanlı uygulamada kullanılmıştır.

## Proje Genel Bakışı

Proje aşağıdaki adımlarla yapılandırılmıştır:

### 1. Veri Keşfi
- **İlk Veri İncelemesi**: Veri setinin ilk ve son birkaç satırı incelenerek yapısı anlaşılmıştır.
- **Veri Yapısı**: Verinin şekli, veri türleri ve özet istatistikleri kontrol edilmiştir.
- **Eksik Veriler**: Eksik veriler belirlenmiş ve ele alınmıştır.

### 2. Veri Görselleştirmesi
- **Ülkelere Göre Üniversite Büyüklüğü**: Farklı ülkelerdeki üniversite büyüklükleri karşılaştırılmıştır.
- **İlk 100 Üniversite**: Ülkelere ve bölgelere göre en başarılı üniversiteler görselleştirilmiştir.
- **Coğrafi Dağılım**: İlk 100 üniversitenin dünya üzerindeki dağılımı harita üzerinde gösterilmiştir.
- **Akademik İtibar**: Ülkelerin akademik itibarı analiz edilmiştir.
- **İlk 10 Üniversite**: QS Genel Skoruna göre ilk 10 üniversite incelenmiştir.
- **Ülkelere Göre Ortalama QS Skorları**: Ülkelerin ortalama QS Genel Skorları karşılaştırılmıştır.

### 3. Model Kurulumu
- **Lineer Regresyon**: QS Genel Skorunu tahmin etmek için basit bir regresyon modeli kurulmuştur.
- **Ridge Regresyon**: Yüksek korelasyonlu özelliklerle başa çıkmak için Ridge regresyon modeli kullanılmıştır.
- **Lasso Regresyon**: Özellik seçimi ve düzenlileştirme amacıyla Lasso regresyon modeli uygulanmıştır.
- **ElasticNet**: Ridge ve Lasso düzenlileştirmelerini birleştiren ElasticNet modeli kurulmuştur.
- **K-En Yakın Komşu (KNN)**: Benzerlik temelli bir tahminleme modeli olan KNN kullanılmıştır.
- **Destek Vektör Makinesi (SVM)**: Karar düzlemleri üzerinden sınıflandırma yapan SVM modeli kullanılmıştır.
- **Karar Ağaçları (CART)**: Açıklayıcı ve görselleştirilebilir bir model olan karar ağaçları kurulmuştur.
- **Random Forest**: Birden fazla karar ağacını birleştirerek daha güçlü bir tahmin modeli olan Random Forest kullanılmıştır.
- **Gradient Boosting Machine (GBM)**: Hataları minimize eden bir model olan GBM kullanılmıştır.
- **XGBoost**: Hızlı ve etkili bir modelleme yöntemi olan XGBoost ile tahmin yapılmıştır.
- **LightGBM**: Büyük veri setlerinde hızlı sonuçlar almak için LightGBM modeli kullanılmıştır.
- **CatBoost**: Özellikle kategorik verilerle etkili çalışan CatBoost modeli kullanılmıştır.
- **Yapay Sinir Ağı**: Daha karmaşık veri yapıları için Yapay Sinir Ağı modeli kullanılmıştır.

### 4. Model Değerlendirmesi ve Karşılaştırması
- **Performans Metrikleri**: Modeller R-kare ve Ortalama Kare Hata (MSE) metriklerine göre karşılaştırılmıştır.
- **En İyi Model Seçimi**: En yüksek performansı gösteren model CatBoost olarak belirlenmiştir.

### 5. Etkileşimli Uygulama
- **Tkinter GUI**: Kullanıcıdan veri alarak QS Genel Skor tahmini yapabilen kullanıcı dostu bir arayüz geliştirilmiştir.

## Sonuçlar
Proje, CatBoost modelinin en iyi performansı gösterdiğini ortaya koymuştur:

R-kare: 0.9744
MSE: 9.43
Bu model, Tkinter arayüzünde gerçek zamanlı tahminler yapmak için kaydedilmiş ve kullanılmıştır.

## Katkıda Bulunma
Katkılarınızı memnuniyetle karşılıyoruz! Lütfen bir Pull Request gönderin.

## Lisans
Bu proje MIT Lisansı ile lisanslanmıştır - detaylar için LICENSE dosyasına bakabilirsiniz.

## Kurulum

Bu projeyi çalıştırmak için aşağıdaki Python kütüphanelerine ihtiyacınız olacak:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost lightgbm catboost tensorflow tkinter


