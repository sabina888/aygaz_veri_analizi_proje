# COVID-19 Veri Analizi

## Proje Amacı
Bu projede, **COVID-19** verileri üzerinde **Keşifsel Veri Analizi (EDA)** gerçekleştirilmiş ve elde edilen bulgular ışığında sağlık sektörü ve politika kararlarına yönelik önerilerde bulunulmuştur. Verilerin analizi yapılarak, COVID-19 vaka sayıları, ölüm oranları, iyileşen hasta oranları ve sağlık altyapısının etkisi incelenmiştir. 

## Kullanılan Veri Setleri
Veri setleri, COVID-19'un küresel yayılımını analiz etmek amacıyla kullanılan aşağıdaki verilerle desteklenmiştir:
1. **`country_wise_latest.csv`**: Ülkeler bazında COVID-19 vakaları, ölümler, iyileşen hasta sayıları, aktif vakalar gibi verileri içerir.
2. **`day_wise.csv`**: COVID-19 vaka sayılarının günlük artışlarını içerir.
3. **`worldometer_data.csv`**: Dünya genelindeki COVID-19 verilerini içerir.

Veriler, **Kaggle COVID-19 Dataset** 

## Proje Adımları

### 1. Veri Yükleme ve Temizleme
İlk adımda, veriler **Pandas** ile yüklenmiş ve eksik değerler kontrol edilerek uygun şekilde doldurulmuştur. Eksik veriler için ileriye doğru doldurma (**forward fill**) yöntemi kullanılmıştır.

```python
import pandas as pd

# Veri setini yükleme
df = pd.read_csv('/path/to/country_wise_latest.csv')

# Eksik değerlerin kontrolü
print(df.isnull().sum())

# Eksik verileri ileriye doğru doldurma (forward fill)
df_filled = df.fillna(method="ffill")
