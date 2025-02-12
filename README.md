# 🦠 COVID-19 Veri Analizi

## 📌 Proje Amacı
Bu proje, **Keşifsel Veri Analizi (EDA)** teknikleri kullanılarak COVID-19 verilerinin analiz edilmesini ve sağlık politikalarına yönelik çıkarımlar yapılmasını amaçlamaktadır. Analiz kapsamında vaka artışları, ölüm oranları, iyileşme oranları ve sağlık altyapısının etkisi incelenmiştir.

---

## 📊 Kullanılan Veri Setleri
Aşağıdaki veri setleri COVID-19'un küresel yayılımını analiz etmek için kullanılmıştır:

| Veri Seti                 | Açıklama |
|---------------------------|-------------|
| **country_wise_latest.csv** | Ülke bazında COVID-19 vaka, ölüm, iyileşen hasta ve aktif vaka sayıları. |
| **day_wise.csv** | Günlük COVID-19 vaka artış verileri. |
| **worldometer_data.csv** | Dünya genelindeki COVID-19 istatistikleri, nüfus ve sağlık kapasitesi bilgileri. |

🔹 **Kaynak:** Kaggle COVID-19 Veri Seti

---

## 🔍 Analiz Adımları

### 1️⃣ Veri Yükleme ve Temizleme
- CSV dosyaları **Pandas** kullanılarak yüklendi.
- Eksik veriler kontrol edilerek uygun şekilde dolduruldu.

### 2️⃣ Keşifsel Veri Analizi (EDA)
- Temel istatistiksel metrikler incelendi.
- **Vaka, Ölüm ve İyileşme Oranları** arasındaki korelasyon analiz edildi.
- Vaka dağılımları ve eğilimleri görselleştirildi.

### 3️⃣ Özellik Mühendisliği
- Yeni özellikler türetildi:
  - **Milyon Başına Vaka Sayısı** (Toplam vaka / Nüfus)
  - **Ölüm Oranı** (Ölümler / Toplam Vaka Sayısı)

### 4️⃣ Sonuçlar ve Öneriler
- COVID-19 **tahmin modelleri**, sağlık hizmetlerinin kapasite yönetiminde kullanılabilir.
- Hastaneler, vaka artış tahminlerine göre **kaynak tahsisi** yapabilir.

---

## 🛠️ Kullanılan Kütüphaneler
- **Pandas**: Veri işleme ve analiz
- **Matplotlib / Seaborn**: Veri görselleştirme
- **Scikit-learn**: Makine öğrenmesi modelleri
- **XGBoost**: Güçlü tahminleme modeli

---

## 📈 Önerilen Modeller
COVID-19 verilerini analiz etmek ve tahminler yapmak için aşağıdaki modeller kullanılmıştır:

- ✅ **Doğrusal Regresyon**
- ✅ **Random Forest**
- ✅ **XGBoost**
- ✅ **ARIMA (Zaman serisi analizi için)**

---

## 🚀 Kullanım
Projeyi çalıştırmak için aşağıdaki komut ile bağımlılıkları yükleyin:

```bash
pip install -r requirements.txt
```

Ana analiz betiğini çalıştırmak için:

```bash
python covid_analysis.py
```

---

## 🤝 Katkıda Bulunma
Projeye aşağıdaki yollarla katkıda bulunabilirsiniz:
- Yeni özellik mühendisliği teknikleri eklemek
- Alternatif tahmin modelleri geliştirmek
- Veri görselleştirme yöntemlerini optimize etmek


