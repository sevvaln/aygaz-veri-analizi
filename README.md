# Aygaz Veri Analizi Projesi- International Energy Statistics

![dataset-cover (1)](https://github.com/user-attachments/assets/19fff067-bdd7-46bf-a49c-a12e1dabad9a)


Bu proje, Aygaz'ın enerji verileri üzerinde çeşitli veri analizi ve makine öğrenimi teknikleri uygulanarak gerçekleştirilmiştir. Projede kullanılan veri seti, enerji üretimi ve tüketimiyle ilgili kapsamlı bilgiler içermektedir.

## Proje Amaçları
- Enerji verilerini analiz ederek belirli bölgelerdeki enerji tüketim alışkanlıklarını anlamak.
- Aykırı değerlerin tespiti ve temizlenmesi.
- Enerji tüketimi ve üretim trendlerini belirlemek.
- Veri setine uygun özellik mühendisliği (Feature Engineering) uygulayarak daha iyi bir veri seti oluşturmak.
- Segmentasyon yaparak belirli kategorileri gruplandırmak.
- Gelecekte kullanılabilecek bir model için temel oluşturmak.

---

## Kullanılan Teknolojiler ve Kütüphaneler
Bu proje, aşağıdaki teknolojiler ve kütüphaneler kullanılarak geliştirilmiştir:
- **Python**: Veri analizi ve görselleştirme için.
- **Pandas**: Veri manipülasyonu ve analizi.
- **NumPy**: Matematiksel işlemler.
- **Matplotlib** & **Seaborn**: Veri görselleştirme.
- **Scikit-learn**: Aykırı değer analizi (LOF) ve PCA (Principal Component Analysis).
- **Jupyter Notebook**: Kodların yazılması ve çalıştırılması için.

---

## Uygulanan Teknikler ve Adımlar
### 1. Veri Analizi
- Veri setindeki eksik ve aykırı değerler analiz edildi.
- Logaritmik dönüşüm ve standartlaştırma gibi yöntemler uygulandı.

### 2. Aykırı Değerlerin Tespiti
- **Local Outlier Factor (LOF)** algoritması kullanılarak aykırı değerler belirlendi.
- Aykırı değerler için görselleştirme yapıldı.

### 3. Özellik Mühendisliği (Feature Engineering)
- Logaritmik, kök, normalizasyon ve standartlaştırma gibi dönüşümler uygulandı.
- Yeni kategoriler oluşturularak segmentasyon yapıldı.

### 4. PCA (Principal Component Analysis)
- Veri setinin boyutunu azaltarak önemli özellikler belirlendi.
- Görselleştirme ile PCA sonuçları incelendi.

---

## Yapılan Görselleştirmeler
1. **Boxplot:** 
   - "Quantity" değişkeninin aykırı değerlerini analiz etmek için.
2. **Histogram:** 
   - Enerji miktarlarının dağılımını incelemek için.
3. **Violin Plot:** 
   - Enerji türlerinin miktar bazında dağılımını göstermek için.
4. **Scatter Plot:** 
   - Enerji miktarları ve diğer değişkenler arasındaki ilişkileri incelemek için.
5. **Trend Analizi (Line Plot):**
   - Yıllara göre enerji tüketim ve üretim değişimlerini analiz etmek için.

---
## Sonuç ve Öneriler

Bu proje, enerji verileri üzerinde yapılan analizlerle enerji sektöründeki karar alma süreçlerine rehberlik etmek için tasarlanmıştır. Yapılan çalışmalar ve çıkarımlar, hem mevcut durumu anlamak hem de gelecekteki projeler için stratejik yönlendirmeler sunmak adına değerlidir.

### **Sonuçlar**
1. **Veri Temizliği ve Hazırlığı**:
   - Eksik ve aykırı değerler başarılı bir şekilde tespit edilerek veri temizleme adımları tamamlanmıştır.
   - Enerji miktarlarına logaritmik dönüşüm uygulanmış ve standardizasyon sağlanarak veri analize uygun hale getirilmiştir.

2. **Segmentasyon ve Kategorik Analiz**:
   - Ülkeler ve enerji türleri bazında segmentasyon yapılmıştır:
     - Düşük, orta ve yüksek tüketim grupları oluşturulmuştur.
   - Özellikle **Avusturya** ve **Belçika** gibi ülkelerdeki enerji tüketim eğilimleri analiz edilmiştir.

3. **Aykırı Değer Analizi**:
   - Local Outlier Factor (LOF) yöntemi kullanılarak enerji tüketiminde anomaliler tespit edilmiştir.
   - Bu aykırı değerlerin olası nedenleri incelenmiş ve enerji verilerindeki sapmalar belirlenmiştir.

4. **Trend Analizi**:
   - Yıllara göre enerji tüketim ve üretim miktarlarının değişimi incelenmiştir.
   - Trend analizi ile enerji türlerindeki büyüme ve daralma oranları hesaplanmıştır.

### **Öneriler**
1. **Enerji Verimliliği**:
   - Segmentasyon sonuçlarına göre enerji verimliliği düşük olan bölgelerde sürdürülebilir enerji projeleri başlatılabilir.
   - Düşük enerji tüketim segmentlerinde yenilenebilir enerji kaynaklarının kullanımı teşvik edilebilir.

2. **Anomali Yönetimi**:
   - Tespit edilen aykırı değerlerin nedenleri incelenerek enerji talep ve arzında olası sorunlar önlenebilir.
   - Bu aykırılıklar, talep dalgalanmalarını öngörmek ve planlama yapmak için kullanılabilir.

3. **Makine Öğrenimi Modelleri**:
   - Regresyon tabanlı modellerle enerji tüketimi ve üretimi tahmin edilebilir.
     - Önerilen modeller: **Linear Regression**, **Random Forest**, veya **Gradient Boosting**.
   - Zaman serisi analizi (örneğin, **ARIMA** veya **Prophet**) ile enerji trendleri öngörülebilir.

4. **Karar Destek Sistemleri**:
   - Analiz sonuçları, enerji sektörü için karar destek sistemlerinin geliştirilmesine olanak sağlar.
   - Özellikle talep tahmini ve kaynak tahsisi süreçleri bu analizlerle optimize edilebilir.

Bu öneriler, enerji verilerinin daha verimli ve sürdürülebilir bir şekilde yönetilmesi için temel oluşturabilir.


---

## Dosyalar
- `notebook.ipynb`: Projenin Jupyter Notebook dosyası.
- `all_energy_statistics.csv`: Kullanılan veri seti.
- `README.md`: Proje açıklaması ve dokümantasyonu.

---
Projenin Kaggle Linki: https://www.kaggle.com/code/evvalarslan/notebookf971f50239


