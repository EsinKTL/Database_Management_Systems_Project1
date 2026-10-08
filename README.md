# Database_Management_Systems_Project1

# Dünya Gelişmişlik Göstergeleri Veri Seti (2021–2025)

Bu proje, **Dünya Bankası Dünya Gelişmişlik Göstergeleri (World Development Indicators – WDI)** veri tabanından elde edilen küresel sosyo-ekonomik, teknolojik, çevresel ve demografik göstergeleri içermektedir.

Veri seti, **2021–2025** dönemini kapsamakta ve ülkeler, bölgeler ve ekonomik topluluklar için çeşitli gelişmişlik göstergelerini bir araya getirmektedir.

Proje içerisinde aynı veri kümesinin **ham veri, işlenmiş CSV, metadata ve birleştirilmiş nihai Excel** formatları bulunmaktadır.

---

## 📂 Proje Dosya Yapısı

```text
.
├── Data_Extract_FromWorld Development Indicators (1).xlsx
│   └── [1] Ham Dünya Bankası verisi
│
├── 21ff240d-8d5c-41c9-99c8-754be6895522_Data.csv
│   └── [2.A] İşlenmiş sayısal veri
│
├── 21ff240d-8d5c-41c9-99c8-754be6895522_Series - Metadata.csv
│   └── [2.B] Gösterge metadata ve veri sözlüğü
│
├── P_Data_Extract_From_World_Development_Indicators.xlsx
│   └── [3] Birleştirilmiş ve düzenlenmiş nihai veri seti
│
└── README.md
    └── [4] Proje dokümantasyonu
```

---

## 🔄 Veri İşleme Akışı

Projede bulunan dosyalar farklı veri kümelerini değil, aynı veri setinin farklı işleme ve sunum aşamalarını temsil etmektedir.

```text
Dünya Bankası WDI
       │
       ▼
┌─────────────────────────────────────────────┐
│ Ham Excel Verisi                             │
│ Data_Extract_FromWorld Development          │
│ Indicators (1).xlsx                         │
└─────────────────────────────────────────────┘
       │
       ▼
┌─────────────────────────────────────────────┐
│ Temizlenmiş Veri                            │
│ 21ff..._Data.csv                            │
└─────────────────────────────────────────────┘
       │
       ├──────────────────────────────┐
       ▼                              ▼
┌───────────────────────┐    ┌───────────────────────┐
│ Veri                  │    │ Metadata              │
│ Data.csv              │    │ Series - Metadata.csv│
└───────────────────────┘    └───────────────────────┘
       │                              │
       └──────────────┬───────────────┘
                      ▼
┌─────────────────────────────────────────────┐
│ Nihai Birleştirilmiş Excel                  │
│ P_Data_Extract_From_World_Development_     │
│ Indicators.xlsx                             │
│                                             │
│  ├── Data                                   │
│  └── Series - Metadata                      │
└─────────────────────────────────────────────┘
```

---

# 📊 Veri Seti Genel Bilgileri

| Özellik              |                                           Değer |
| -------------------- | ----------------------------------------------: |
| Veri kaynağı         | World Bank – World Development Indicators (WDI) |
| Zaman aralığı        |                                       2021–2025 |
| Yıl sayısı           |                                               5 |
| Coğrafi kapsam       |            265 ülke, bölge ve ekonomik topluluk |
| Net veri satırı      |                                           1.325 |
| Toplam satır         |                                           1.330 |
| Gösterge sütunu      |                                              41 |
| Veri formatları      |                                       XLSX, CSV |
| Eksik veri gösterimi |                                            `..` |

### Veri satırı hesabı

```text
265 ülke/bölge × 5 yıl = 1.325 veri satırı
```

Nihai Excel dosyasındaki toplam satır sayısı **1.330** olup, veri satırlarına ek olarak alt/dipnot satırlarını da içermektedir.

---

# 🧩 Veri Setinin Yapısı

Veri setindeki 41 sütun, analiz kolaylığı sağlamak amacıyla 6 ana kategori altında gruplandırılmıştır.

## 1. Kimlik ve Zaman Bilgileri

|  # | Sütun          | Veri Tipi | Açıklama                                 |
| -: | -------------- | --------- | ---------------------------------------- |
|  1 | `Time`         | Sayısal   | Verinin ait olduğu yıl                   |
|  2 | `Time Code`    | Metin     | Standart yıl kodu, ör. `YR2021`          |
|  3 | `Country Name` | Metin     | Ülke, bölge veya ekonomik topluluğun adı |
|  4 | `Country Code` | Metin     | 3 karakterli Dünya Bankası ülke kodu     |

---

## 2. Makroekonomi ve Dış Ticaret

|  # | Sütun                                               | Açıklama                                                |
| -: | --------------------------------------------------- | ------------------------------------------------------- |
|  5 | `GDP (constant 2015 US$)`                           | Sabit 2015 ABD doları cinsinden GSYH                    |
|  6 | `GDP growth (annual %)`                             | Yıllık reel GSYH büyüme oranı                           |
|  7 | `GDP per capita (constant 2015 US$)`                | Kişi başına GSYH                                        |
|  8 | `Inflation, consumer prices (annual %)`             | Yıllık tüketici enflasyonu                              |
|  9 | `Foreign direct investment, net inflows (% of GDP)` | Net doğrudan yabancı yatırım girişlerinin GSYH'ye oranı |
| 10 | `Exports of goods and services (% of GDP)`          | Mal ve hizmet ihracatının GSYH'ye oranı                 |
| 11 | `Imports of goods and services (% of GDP)`          | Mal ve hizmet ithalatının GSYH'ye oranı                 |
| 12 | `Total natural resources rents (% of GDP)`          | Doğal kaynak gelirlerinin GSYH'ye oranı                 |

---

## 3. Teknoloji, Dijitalleşme ve Ar-Ge

|  # | Sütun                                                 | Açıklama                                               |
| -: | ----------------------------------------------------- | ------------------------------------------------------ |
| 13 | `Individuals using the Internet (% of population)`    | İnternet kullanan nüfus oranı                          |
| 14 | `Fixed broadband subscriptions (per 100 people)`      | Her 100 kişiye düşen sabit geniş bant aboneliği        |
| 15 | `Mobile cellular subscriptions (per 100 people)`      | Her 100 kişiye düşen mobil abonelik                    |
| 16 | `Secure Internet servers (per 1 million people)`      | Her 1 milyon kişiye düşen güvenli internet sunucusu    |
| 17 | `High-technology exports (% of manufactured exports)` | Yüksek teknoloji ihracatının imalat ihracatındaki payı |
| 18 | `Research and development expenditure (% of GDP)`     | Ar-Ge harcamalarının GSYH'ye oranı                     |
| 19 | `Technicians in R&D (per million people)`             | Her 1 milyon kişiye düşen Ar-Ge teknisyeni             |

---

## 4. Enerji, Çevre ve İklim Değişikliği

|  # | Sütun                                                                  | Açıklama                                                              |
| -: | ---------------------------------------------------------------------- | --------------------------------------------------------------------- |
| 20 | `Access to electricity (% of population)`                              | Elektriğe erişimi olan nüfus oranı                                    |
| 21 | `Renewable energy consumption (% of total final energy consumption)`   | Yenilenebilir enerjinin nihai enerji tüketimindeki payı               |
| 22 | `Renewable electricity output (% of total electricity output)`         | Yenilenebilir kaynaklardan elektrik üretiminin toplam üretimdeki payı |
| 23 | `Electricity production from coal sources (% of total)`                | Kömür kaynaklı elektrik üretiminin toplam üretimdeki payı             |
| 24 | `Energy use (kg of oil equivalent per capita)`                         | Kişi başına enerji kullanımı                                          |
| 25 | `Energy intensity level of primary energy (MJ/$2021 PPP GDP)`          | Birincil enerji yoğunluğu                                             |
| 26 | `Forest area (% of land area)`                                         | Ormanlık alanın toplam kara alanına oranı                             |
| 27 | `PM2.5 air pollution, mean annual exposure`                            | Yıllık ortalama PM2.5 maruziyeti                                      |
| 28 | `Total greenhouse gas emissions excluding LULUCF (% change from 1990)` | Sera gazı emisyonlarının 1990'a göre değişimi                         |
| 29 | `Total greenhouse gas emissions excluding LULUCF (Mt CO2e)`            | Toplam sera gazı emisyonu                                             |
| 30 | `Nitrous oxide (N2O) emissions (total) excluding LULUCF (Mt CO2e)`     | Toplam N₂O emisyonu                                                   |
| 31 | `Total fisheries production (metric tons)`                             | Toplam balıkçılık ve su ürünleri üretimi                              |

---

## 5. Nüfus, Demografi ve Sağlık

|  # | Sütun                                      | Açıklama                            |
| -: | ------------------------------------------ | ----------------------------------- |
| 32 | `Population, total`                        | Toplam nüfus                        |
| 33 | `Population, female`                       | Kadın nüfusu                        |
| 34 | `Population, male`                         | Erkek nüfusu                        |
| 35 | `Population growth (annual %)`             | Yıllık nüfus artış oranı            |
| 36 | `Urban population (% of total population)` | Kentsel nüfusun toplam nüfusa oranı |
| 37 | `Life expectancy at birth, total (years)`  | Doğuşta beklenen yaşam süresi       |

---

## 6. İşgücü ve Eğitim

|  # | Sütun                                          | Açıklama                           |
| -: | ---------------------------------------------- | ---------------------------------- |
| 38 | `Labor force, total`                           | Toplam aktif işgücü                |
| 39 | `Unemployment, total (% of total labor force)` | Toplam işsizlik oranı              |
| 40 | `Compulsory education, duration (years)`       | Zorunlu eğitim süresi              |
| 41 | `School enrollment, tertiary (% gross)`        | Yükseköğretim brüt okullaşma oranı |

---

# 🗃️ Veri Dosyaları

## 1. Ham Veri – Excel

**`Data_Extract_FromWorld Development Indicators (1).xlsx`**

Dünya Bankası WDI sisteminden elde edilen ham Excel çıktısıdır.

Bu dosyada:

* Ham ülke ve bölge bilgileri
* Yıl bilgileri
* Gösterge değerleri
* Üst ve alt başlıklar
* Dipnot ve metadata satırları

bulunmaktadır.

Analizden önce bu dosyanın temizlenmesi önerilir.

---

## 2. İşlenmiş Veri – CSV

**`21ff240d-8d5c-41c9-99c8-754be6895522_Data.csv`**

Ham verinin analiz ve yazılım uygulamalarında kullanılmak üzere düzenlenmiş CSV sürümüdür.

Python, R, SQL veya diğer veri analiz araçlarıyla kullanılabilir.

Örnek Python kullanımı:

```python
import pandas as pd

df = pd.read_csv(
    "21ff240d-8d5c-41c9-99c8-754be6895522_Data.csv"
)

print(df.head())
print(df.shape)
```

---

## 3. Metadata – CSV

**`21ff240d-8d5c-41c9-99c8-754be6895522_Series - Metadata.csv`**

Veri setindeki göstergelerin teknik açıklamalarını içeren metadata dosyasıdır.

İçerisinde göstergelerin:

* Gösterge kodları
* İsimleri
* Tanımları
* Ölçüm birimleri
* Veri kaynakları
* Teknik açıklamaları

gibi bilgiler bulunmaktadır.

Bu dosya özellikle gösterge seçimi ve veri sözlüğü oluşturulması sırasında kullanılabilir.

---

## 4. Nihai Veri Seti – Excel

**`P_Data_Extract_From_World_Development_Indicators.xlsx`**

Projenin kullanıma hazır nihai Excel dosyasıdır.

Dosya içerisinde iki çalışma sayfası bulunmaktadır:

```text
P_Data_Extract_From_World_Development_Indicators.xlsx

├── Data
└── Series - Metadata
```

### `Data`

Ülke/bölge, yıl ve 41 gelişmişlik göstergesini içerir.

### `Series - Metadata`

Veri setinde kullanılan göstergelerin metadata bilgilerini içerir.

---

# 🧹 Veri Ön İşleme

Veri analizi veya makine öğrenmesi çalışmalarından önce aşağıdaki ön işleme adımlarının uygulanması önerilmektedir.

## 1. Eksik Verilerin Dönüştürülmesi

Dünya Bankası verilerinde eksik değerler:

```text
..
```

şeklinde gösterilmektedir.

Analiz sırasında bu değerlerin `NaN` / `null` değerlerine dönüştürülmesi önerilir.

Python:

```python
df = df.replace("..", pd.NA)
```

Sayısal sütunlar için:

```python
numeric_columns = df.columns[4:]

df[numeric_columns] = df[numeric_columns].apply(
    pd.to_numeric,
    errors="coerce"
)
```

---

## 2. Dipnot ve Metadata Satırlarının Çıkarılması

Nihai veri dosyasının sonunda yer alan dipnot ve metadata satırları analiz matrisine dahil edilmemelidir.

Beklenen analiz veri yapısı:

```text
265 ülke/bölge × 5 yıl
= 1.325 gözlem
```

---

## 3. Ülke ve Bölge Ayrımı

Veri setinde yalnızca bağımsız ülkeler bulunmamaktadır.

Örneğin:

```text
World
Arab World
European Union
Sub-Saharan Africa
```

gibi bölgesel veya ekonomik topluluklar da bulunabilir.

Analizin amacına göre `Country Code` veya `Country Name` kullanılarak bu kayıtlar ayrıştırılmalıdır.

---

## 4. Veri Tiplerinin Düzenlenmesi

Gösterge sütunlarının sayısal veri tipine dönüştürülmesi önerilir.

Örneğin:

```python
df["GDP growth (annual %)"] = pd.to_numeric(
    df["GDP growth (annual %)"],
    errors="coerce"
)
```

Bu işlem, istatistiksel analiz ve makine öğrenmesi modellerinde veri tipinden kaynaklanabilecek hataların önüne geçer.

---

# 🔬 Kullanım Alanları

Bu veri seti aşağıdaki çalışmalar için kullanılabilir:

* 🌍 Ülkelerin gelişmişlik karşılaştırmaları
* 📈 Ekonomik büyüme analizi
* 💰 GSYH ve kişi başına gelir analizi
* 💻 Dijitalleşme ve internet kullanım analizi
* 🔬 Ar-Ge ve teknoloji göstergelerinin incelenmesi
* ⚡ Enerji ve elektrik erişimi analizi
* 🌱 Çevresel sürdürülebilirlik araştırmaları
* 🌡️ İklim ve sera gazı emisyon analizleri
* 👥 Nüfus ve demografik analizler
* 🎓 Eğitim göstergelerinin karşılaştırılması
* 👷 İşgücü ve işsizlik analizleri
* 🤖 Makine öğrenmesi ve tahmin modelleri
* 📊 Veri görselleştirme ve dashboard uygulamaları
* 🧮 Ülke gelişmişlik endeksi oluşturma
* 🔎 Korelasyon ve regresyon analizleri
* 📉 Çok değişkenli istatistiksel analizler

---

# 📌 Veri Kalitesi ve Dikkat Edilmesi Gerekenler

Veri analizi sırasında aşağıdaki noktalar dikkate alınmalıdır:

1. **Eksik değerler:** `..` değerleri gerçek sıfır anlamına gelmez.
2. **Bölgesel kayıtlar:** Tüm satırlar bağımsız ülkeleri temsil etmez.
3. **Ölçüm birimleri:** Göstergelerin birimleri birbirinden farklıdır.
4. **Zaman kapsamı:** Veri seti 2021–2025 dönemini kapsamaktadır.
5. **Gösterge bulunabilirliği:** Bazı göstergelerde belirli ülke veya yıllar için veri bulunmayabilir.
6. **Karşılaştırılabilirlik:** Farklı göstergeler farklı metodolojilerle hesaplandığından doğrudan karşılaştırma yapılmadan önce metadata incelenmelidir.

---
