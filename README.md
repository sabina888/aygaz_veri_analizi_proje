# COVID-19 Veri Analizi

## Proje Amacı
Bu projede, **COVID-19** verileri üzerinde **Keşifsel Veri Analizi (EDA)** gerçekleştirilmiş ve elde edilen bulgular ışığında sağlık sektörü ve politika kararlarına yönelik önerilerde bulunulmuştur. Verilerin analizi yapılarak, COVID-19 vaka sayıları, ölüm oranları, iyileşen hasta oranları ve sağlık altyapısının etkisi incelenmiştir. 

## Kullanılan Veri Setleri
Veri setleri, COVID-19'un küresel yayılımını analiz etmek amacıyla kullanılan aşağıdaki verilerle desteklenmiştir:
1. **`country_wise_latest.csv`**: Ülkeler bazında COVID-19 vakaları, ölümler, iyileşen hasta sayıları, aktif vakalar gibi verileri içerir.
2. **`day_wise.csv`**: COVID-19 vaka sayılarının günlük artışlarını içerir.
3. **`worldometer_data.csv`**: Dünya genelindeki COVID-19 verilerini içerir.

Veriler, **Kaggle COVID-19 Dataset** 
## Adımlar
### 1. Veri Yükleme ve Temizleme
- CSV dosyaları **Pandas** ile yüklenmiştir.
- Eksik değerler kontrol edilmiş ve uygun şekilde doldurulmuştur.
  
### 2. Keşifsel Veri Analizi (EDA)
- Veri setindeki temel istatistikler analiz edilmiştir.
- **`Confirmed`**, **`Deaths`** ve **`Recovered`** gibi sütunlar arasındaki korelasyon incelenmiştir.
- Vaka sayılarının dağılımı ve diğer görselleştirmeler yapılmıştır.

### 3. Özellik Mühendisliği
- **`Cases per Million`** (Vaka sayısı / Nüfus) gibi yeni özellikler oluşturulmuştur.
- **`Death Rate`** (Ölüm Oranı) gibi oranlar hesaplanmıştır.


### 4. Sonuçlar ve Öneriler
- **COVID-19 vaka tahmin modelleri**, sağlık hizmetlerinin kapasite yönetiminde kullanılabilir.
- Sağlık kuruluşları, **vaka artış tahminlerine** göre **kaynak tahsisini** yapabilir.

## Kullanılan Kütüphaneler
- **Pandas**: Veri işleme ve analizi.
- **Matplotlib / Seaborn**: Görselleştirme.
- **Scikit-learn**: Makine öğrenmesi modelleri.
- **XGBoost**: Güçlü tahmin modeli.
### 6.Önerilen modeller
**Doğrusal Regresyon**
- **Random Forest**
- **XGBoost**
- **ARIMA**
