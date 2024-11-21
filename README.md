Enerji Verileri Analizi
Projenin Amacı
Bu proje, enerji sektörüne ait çeşitli ülkelerin enerji üretim, tüketim ve dönüşüm istatistiklerini içeren bir veri setini analiz etmeyi amaçlamaktadır. Analiz kapsamında:

-Enerji tüketimindeki anomalilerin tespit edilmesi,
-Ülkelere ve enerji türlerine göre segmentasyon oluşturulması,
-Enerji miktarlarının zaman içindeki trendlerinin incelenmesi hedeflenmiştir.
Bu çalışmalar, enerji sektöründe karar alma süreçlerini destekleyecek içgörüler sunmayı ve ilgili bir makine öğrenimi modeline temel oluşturmayı amaçlamaktadır.

Kullanılan Veri Seti
-Veri Kaynağı: All_Energy_Statistics.csv
-İçerik:
  -Ülkeler ve bölgeler bazında enerji üretim, tüketim ve transfer istatistikleri.
  -Birim, kategori, yıl ve miktar gibi özellikler.

Yapılan Çalışmalar

1. Veri Hazırlama
-Eksik ve hatalı değerler analiz edildi ve temizlendi.
-"Quantity" sütunundaki değerler normalleştirildi ve logaritmik dönüşüm uygulandı.
-Önemli metrikler (medyan, maksimum, minimum) hesaplandı.

2. Anomali Tespiti
-Local Outlier Factor (LOF) algoritması kullanılarak anormal enerji miktarları tespit edildi.
-Aykırı değerler görselleştirilerek dağılımları incelendi.

3. Feature Engineering
-"Quantity" için logaritmik, normalize edilmiş ve karekök dönüşümü gibi özellikler oluşturuldu.
Enerji kategorilerinin frekansları hesaplanarak "category_freq" özelliği eklendi.

4. Segmentasyon
-Ülkeler bazında enerji miktarlarına göre segmentasyon (Low, Medium, High) yapıldı.
-Belçika ve Avusturya gibi ülkeler özelinde segmentasyon analizi gerçekleştirildi.

5. Trend Analizi
-Ülke ve kategori bazında enerji miktarlarının yıllara göre değişimi incelendi.
-Zaman serisi verilerindeki yıllık değişim yüzdeleri analiz edildi.


Sonuçlar
-Anomali Tespiti: Aykırı enerji tüketim ve üretim değerleri tespit edilerek olası veri sorunları veya olağan dışı durumlar işaretlendi.
-Segmentasyon: Ülkeler ve enerji türlerine göre segmentler oluşturularak enerji kullanımında farklı eğilimler belirlendi.
-Trend Analizi: Enerji türlerinin yıllık değişim yüzdeleri analiz edilerek enerji dönüşümü ve sürdürülebilirlik stratejileri için önemli bilgiler sağlandı.

Proje Çıktılarının Kullanımı
Bu proje, enerji sektörü için aşağıdaki alanlarda çözüm sunabilir:

-Kaynak Tahsisi: Ülkeler bazında enerji ihtiyaçlarını önceliklendirmek.
-Sürdürülebilirlik: Düşük enerji tüketim segmentinde yer alan ülkeler için sürdürülebilir enerji politikaları geliştirmek.
-Anomali Tespiti: Anormal değerler, veri kalitesini artırmak ve karar alma süreçlerini iyileştirmek için kullanılabilir.
-Makine Öğrenimi Temeli:
-Segmentasyon ve özellik mühendisliği süreçleri, bir tahmin modeli (örneğin, regresyon veya zaman serisi modelleme) geliştirmek için kullanılabilir.

Öneriler

-Makine Öğrenimi Modelleri:
 -Regresyon Modelleri: Enerji tüketimini tahmin etmek için. (Örneğin, Linear Regression veya Random Forest.)
 -Clustering Modelleri: Segmentasyon süreçlerini daha iyi yönetmek için. (KMeans veya DBSCAN önerilebilir.)
 -Zaman Serisi Analizi: ARIMA veya Prophet gibi modellerle enerji trendlerini tahmin etmek.
 
-Veri Geliştirme:
 -Daha fazla coğrafi ve ekonomik özellik (örneğin, GDP, nüfus) entegre edilerek veri zenginleştirilebilir.



Aşağıda, projeyi açıklamak için uygun bir Sonuç ve Öneriler bölümü ve README dosyasına ekleyebileceğiniz tam metni hazırladım. Bu metin, veri analizi sürecinizi özetler, proje çıktılarınızı açıklar ve gelecekteki ML uygulamaları için öneriler sunar.

README: Enerji Verileri Analizi
Projenin Amacı
Bu proje, enerji sektörüne ait çeşitli ülkelerin enerji üretim, tüketim ve dönüşüm istatistiklerini içeren bir veri setini analiz etmeyi amaçlamaktadır. Analiz kapsamında:

Enerji tüketimindeki anomalilerin tespit edilmesi,
Ülkelere ve enerji türlerine göre segmentasyon oluşturulması,
Enerji miktarlarının zaman içindeki trendlerinin incelenmesi hedeflenmiştir.
Bu çalışmalar, enerji sektöründe karar alma süreçlerini destekleyecek içgörüler sunmayı ve ilgili bir makine öğrenimi modeline temel oluşturmayı amaçlamaktadır.

Kullanılan Veri Seti
Veri Kaynağı: All_Energy_Statistics.csv
İçerik:
Ülkeler ve bölgeler bazında enerji üretim, tüketim ve transfer istatistikleri.
Birim, kategori, yıl ve miktar gibi özellikler.
Yapılan Çalışmalar
Veri Hazırlama

Eksik ve hatalı değerler analiz edildi ve temizlendi.
"Quantity" sütunundaki değerler normalleştirildi ve logaritmik dönüşüm uygulandı.
Önemli metrikler (medyan, maksimum, minimum) hesaplandı.
Anomali Tespiti

Local Outlier Factor (LOF) algoritması kullanılarak anormal enerji miktarları tespit edildi.
Aykırı değerler görselleştirilerek dağılımları incelendi.
Feature Engineering

"Quantity" için logaritmik, normalize edilmiş ve karekök dönüşümü gibi özellikler oluşturuldu.
Enerji kategorilerinin frekansları hesaplanarak "category_freq" özelliği eklendi.
Segmentasyon

Ülkeler bazında enerji miktarlarına göre segmentasyon (Low, Medium, High) yapıldı.
Belçika ve Avusturya gibi ülkeler özelinde segmentasyon analizi gerçekleştirildi.
Trend Analizi

Ülke ve kategori bazında enerji miktarlarının yıllara göre değişimi incelendi.
Zaman serisi verilerindeki yıllık değişim yüzdeleri analiz edildi.
Sonuçlar
Anomali Tespiti: Aykırı enerji tüketim ve üretim değerleri tespit edilerek olası veri sorunları veya olağan dışı durumlar işaretlendi.
Segmentasyon: Ülkeler ve enerji türlerine göre segmentler oluşturularak enerji kullanımında farklı eğilimler belirlendi.
Trend Analizi: Enerji türlerinin yıllık değişim yüzdeleri analiz edilerek enerji dönüşümü ve sürdürülebilirlik stratejileri için önemli bilgiler sağlandı.
Proje Çıktılarının Kullanımı
Bu proje, enerji sektörü için aşağıdaki alanlarda çözüm sunabilir:

Kaynak Tahsisi: Ülkeler bazında enerji ihtiyaçlarını önceliklendirmek.
Sürdürülebilirlik: Düşük enerji tüketim segmentinde yer alan ülkeler için sürdürülebilir enerji politikaları geliştirmek.
Anomali Tespiti: Anormal değerler, veri kalitesini artırmak ve karar alma süreçlerini iyileştirmek için kullanılabilir.
Makine Öğrenimi Temeli:
Segmentasyon ve özellik mühendisliği süreçleri, bir tahmin modeli (örneğin, regresyon veya zaman serisi modelleme) geliştirmek için kullanılabilir.

Öneriler

-Makine Öğrenimi Modelleri:
 -Regresyon Modelleri: Enerji tüketimini tahmin etmek için. (Örneğin, Linear Regression veya Random Forest.)
 -Clustering Modelleri: Segmentasyon süreçlerini daha iyi yönetmek için. (KMeans veya DBSCAN önerilebilir.)
 -Zaman Serisi Analizi: ARIMA veya Prophet gibi modellerle enerji trendlerini tahmin etmek.
-Veri Geliştirme:
 -Daha fazla coğrafi ve ekonomik özellik (örneğin, GDP, nüfus) entegre edilerek veri zenginleştirilebilir.

Projenin Kaggle Linki: https://www.kaggle.com/code/evvalarslan/notebookf971f50239

