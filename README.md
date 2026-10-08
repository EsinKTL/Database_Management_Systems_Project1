# Database_Management_Systems_Project1

# Dünya Gelişmişlik Göstergeleri Veri Seti (2021–2025)

Bu depo, **Dünya Bankası Dünya Gelişmişlik Göstergeleri (World Development Indicators - WDI)** veritabanından alınan kapsamlı sosyo-ekonomik, çevresel ve teknolojik verileri içermektedir.

## 📂 Veri Setine Genel Bakış

| Özellik                  | Açıklama                                                   |
| ------------------------ | ---------------------------------------------------------- |
| **Dosya Adı**            | `21ff240d-8d5c-41c9-99c8-754be6895522_Data.csv`            |
| **Satır Sayısı**         | 1.330 satır (1.325 veri satırı + 5 dipnot/metadata satırı) |
| **Sütun Sayısı**         | 41 nitelik (özellik)                                       |
| **Zaman Aralığı**        | 2021–2025                                                  |
| **Kapsam**               | 265 ülke, bölge ve ekonomik topluluk                       |
| **Eksik Veri Gösterimi** | `..`                                                       |

Veri seti; ülkelerin ekonomik performansını, teknolojik ve dijital altyapısını, enerji ve çevre göstergelerini, demografik yapısını, iş gücü ve eğitim durumunu incelemek amacıyla kullanılabilir.

> **Not:** Veri setindeki `..` sembolü, ilgili gözlemin eksik veya ölçülememiş olduğunu ifade etmektedir.

---

## 📊 Veri Seti Sütunları

Veri setinde yer alan 41 sütun, 6 ana tematik grupta toplanmıştır.

### 1. Kimlik ve Zaman Bilgileri

| Sütun          | Açıklama                                                 |
| -------------- | -------------------------------------------------------- |
| `Time`         | Verinin ait olduğu yıl (ör. 2021).                       |
| `Time Code`    | Standart yıl kodu (ör. `YR2021`).                        |
| `Country Name` | Ülke, bölge veya ekonomik topluluğun tam adı.            |
| `Country Code` | Ülke/bölgeye ait 3 harfli kod (ör. `AFG`, `TUR`, `WLD`). |

### 2. Ekonomik Göstergeler

| Sütun                                               | Açıklama                                                          |
| --------------------------------------------------- | ----------------------------------------------------------------- |
| `GDP (constant 2015 US$)`                           | 2015 sabit ABD doları cinsinden Gayrisafi Yurt İçi Hasıla (GSYH). |
| `GDP growth (annual %)`                             | Yıllık GSYH büyüme oranı (%).                                     |
| `GDP per capita (constant 2015 US$)`                | Kişi başına düşen GSYH (2015 sabit USD).                          |
| `Inflation, consumer prices (annual %)`             | Tüketici fiyatlarına dayalı yıllık enflasyon oranı (%).           |
| `Foreign direct investment, net inflows (% of GDP)` | Doğrudan yabancı yatırım net girişlerinin GSYH'ye oranı (%).      |
| `Exports of goods and services (% of GDP)`          | Mal ve hizmet ihracatının GSYH'ye oranı (%).                      |
| `Imports of goods and services (% of GDP)`          | Mal ve hizmet ithalatının GSYH'ye oranı (%).                      |
| `Total natural resources rents (% of GDP)`          | Doğal kaynak gelirlerinin/rantlarının GSYH içindeki payı (%).     |

### 3. Teknoloji, İnovasyon ve Altyapı

| Sütun                                                 | Açıklama                                                                    |
| ----------------------------------------------------- | --------------------------------------------------------------------------- |
| `Individuals using the Internet (% of population)`    | İnternet kullanan nüfusun toplam nüfusa oranı (%).                          |
| `Fixed broadband subscriptions (per 100 people)`      | 100 kişi başına düşen sabit geniş bant internet aboneliği sayısı.           |
| `Mobile cellular subscriptions (per 100 people)`      | 100 kişi başına düşen mobil cep telefonu aboneliği sayısı.                  |
| `Secure Internet servers (per 1 million people)`      | 1 milyon kişi başına düşen güvenli internet sunucusu sayısı.                |
| `High-technology exports (% of manufactured exports)` | Yüksek teknoloji ürünleri ihracatının toplam imalat ihracatındaki payı (%). |
| `Research and development expenditure (% of GDP)`     | Araştırma ve Geliştirme (Ar-Ge) harcamalarının GSYH'ye oranı (%).           |
| `Technicians in R&D (per million people)`             | 1 milyon kişi başına düşen Ar-Ge teknik personeli sayısı.                   |

### 4. Enerji, Çevre ve Sürdürülebilirlik

| Sütun                                                                  | Açıklama                                                                                 |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `Access to electricity (% of population)`                              | Elektriğe erişimi olan nüfus oranı (%).                                                  |
| `Renewable energy consumption (% of total final energy consumption)`   | Toplam nihai enerji tüketimindeki yenilenebilir enerji payı (%).                         |
| `Forest area (% of land area)`                                         | Ormanlık alanın toplam kara alanına oranı (%).                                           |
| `PM2.5 air pollution, mean annual exposure`                            | Yıllık ortalama PM2.5 ince parçacıklı madde hava kirliliği maruziyeti (μg/m³).           |
| `Energy use (kg of oil equivalent per capita)`                         | Kişi başına düşen enerji kullanımı (kg petrol eşdeğeri).                                 |
| `Electricity production from coal sources (% of total)`                | Kömürden üretilen elektriğin toplam elektrik üretimine oranı (%).                        |
| `Energy intensity level of primary energy (MJ/$2021 PPP GDP)`          | Birincil enerji yoğunluk düzeyi (2021 SAGP GSYH başına megajul).                         |
| `Renewable electricity output (% of total electricity output)`         | Yenilenebilir kaynaklardan elde edilen elektriğin toplam elektrik üretimindeki payı (%). |
| `Total greenhouse gas emissions excluding LULUCF (% change from 1990)` | Toplam sera gazı emisyonlarının 1990 yılına göre yüzde değişimi.                         |
| `Total greenhouse gas emissions excluding LULUCF (Mt CO2e)`            | Toplam sera gazı emisyonu miktarı (Mt CO₂ eşdeğeri).                                     |
| `Nitrous oxide (N2O) emissions (total) excluding LULUCF (Mt CO2e)`     | Azot oksit (N₂O) emisyon miktarı (Mt CO₂e).                                              |
| `Total fisheries production (metric tons)`                             | Toplam su ürünleri/balıkçılık üretimi (metrik ton).                                      |

### 5. Demografi ve Nüfus

| Sütun                                      | Açıklama                                                   |
| ------------------------------------------ | ---------------------------------------------------------- |
| `Population, total`                        | Toplam nüfus.                                              |
| `Population, female`                       | Toplam kadın nüfusu.                                       |
| `Population, male`                         | Toplam erkek nüfusu.                                       |
| `Population growth (annual %)`             | Yıllık nüfus artış oranı (%).                              |
| `Urban population (% of total population)` | Kentsel alanlarda yaşayan nüfusun toplam nüfusa oranı (%). |
| `Life expectancy at birth, total (years)`  | Doğumda beklenen ortalama yaşam süresi (yıl).              |

### 6. İşgücü ve Eğitim

| Sütun                                          | Açıklama                                              |
| ---------------------------------------------- | ----------------------------------------------------- |
| `Unemployment, total (% of total labor force)` | Toplam işsizlik oranı (ILO tahmini, %).               |
| `Labor force, total`                           | Toplam işgücü sayısı.                                 |
| `Compulsory education, duration (years)`       | Zorunlu eğitim süresi (yıl).                          |
| `School enrollment, tertiary (% gross)`        | Yükseköğretime (üniversite) brüt okullaşma oranı (%). |

---

## 🌍 Kapsam

Veri seti toplam **265 ülke, bölge ve ekonomik topluluğu** kapsamaktadır.

Veri içerisinde yalnızca bağımsız ülkeler değil, Dünya Bankası tarafından tanımlanan çeşitli bölgesel ve ekonomik gruplar da bulunmaktadır.

Örnekler:

* World
* Arab World
* Africa Eastern and Southern
* Afghanistan (`AFG`)
* Türkiye (`TUR`)
* ve diğer ülke/bölge grupları

---

## 🗓️ Zaman Aralığı

Veriler **2021–2025** dönemini kapsamaktadır:

* **2021**
* **2022**
* **2023**
* **2024**
* **2025**

Bazı göstergelerde ilgili yıl için veri bulunmayabilir. Bu durumda değer `..` olarak gösterilmektedir.

---

## ⚠️ Eksik Veriler

Veri setinde eksik veya ölçülemeyen değerler:

```text
..
```

şeklinde gösterilmiştir.

Veri analizi veya makine öğrenmesi çalışmalarında bu değerlerin sayısal veri olarak kullanılmadan önce uygun bir yöntemle ele alınması gerekir.

Örneğin:

* Eksik gözlemlerin kaldırılması
* Ortalama veya medyan ile doldurma
* Zaman serilerinde ileri/geri doldurma
* İstatistiksel imputasyon yöntemleri

kullanılabilir.

---

## 🔎 Kullanım Alanları

Bu veri seti aşağıdaki çalışmalar için kullanılabilir:

* Ülkelerin gelişmişlik düzeylerinin karşılaştırılması
* Ekonomik kalkınma analizi
* Dijitalleşme ve teknoloji göstergelerinin incelenmesi
* Ar-Ge ve inovasyon performansının analizi
* Çevresel sürdürülebilirlik çalışmaları
* Enerji tüketimi ve yenilenebilir enerji analizi
* Nüfus ve demografik yapı analizi
* Eğitim ve işgücü karşılaştırmaları
* Ülkelerin ekonomik ve teknolojik kümelenmesi
* İstatistiksel analiz ve veri görselleştirme
* Makine öğrenmesi ve tahmin modelleri

---

## 🧹 Veri Ön İşleme Önerileri

Analiz öncesinde aşağıdaki ön işleme adımlarının uygulanması önerilir:

1. `..` değerlerinin `NaN` / eksik değer olarak dönüştürülmesi.
2. Sayısal sütunların uygun veri tipine dönüştürülmesi.
3. `Time` sütununun sayısal veya tarihsel değişken olarak ele alınması.
4. Ülke, bölge ve ekonomik toplulukların analiz amacına göre ayrıştırılması.
5. Eksik veri oranlarının incelenmesi.
6. Aykırı değerlerin kontrol edilmesi.
7. Makine öğrenmesi uygulanacaksa özelliklerin uygun şekilde ölçeklendirilmesi.
8. Zaman boyutu dikkate alınarak eğitim ve test verilerinin ayrıştırılması.

---

## 📁 Dosya Yapısı

```text
.
├── 21ff240d-8d5c-41c9-99c8-754be6895522_Data.csv
└── README.md
```

---

## 📌 Veri Kaynağı

Veri setinin temel kaynağı **Dünya Bankası – World Development Indicators (WDI)** veritabanıdır.

WDI, ülkeler ve ekonomiler hakkında ekonomik, sosyal, çevresel, teknolojik ve demografik çok sayıda gösterge sunan kapsamlı bir uluslararası veri kaynağıdır.

---

## 📄 Lisans ve Kullanım

Veri setinin kullanım koşulları ve lisans bilgileri için verinin alındığı **Dünya Bankası World Development Indicators** kaynak ve lisans koşullarının incelenmesi önerilir.

---

## 📈 Özet

| Metrik                       |     Değer |
| ---------------------------- | --------: |
| Veri yılı                    | 2021–2025 |
| Ülke/bölge/ekonomik topluluk |       265 |
| Toplam satır                 |     1.330 |
| Veri satırı                  |     1.325 |
| Metadata/dipnot satırı       |         5 |
| Özellik sayısı               |        41 |
| Ana tema sayısı              |         6 |
| Eksik veri gösterimi         |      `..` |


# World Development Indicators (WDI) Dataset (2021–2025)

Bu veri seti, **Dünya Bankası (World Bank - World Development Indicators - WDI)** veritabanından derlenmiş olup, 2021–2025 yılları arasında dünya genelindeki ülkelerin ve bölgesel/ekonomik grupların sosyo-ekonomik, teknolojik, çevresel ve demografik göstergelerini içermektedir.

Veri seti; makroekonomik analizler, iklim değişikliği çalışmaları, dijitalleşme oranlarının incelenmesi, sürdürülebilirlik araştırmaları ve kamu politikalarının değerlendirilmesi gibi çeşitli veri analizi çalışmalarında kullanılabilir.

---

## 📂 Dataset Genel Bakış

| Özellik            |                                                        Değer | Açıklama                                       |
| ------------------ | -----------------------------------------------------------: | ---------------------------------------------- |
| **Dosya Adı**      | `21ff240d-8d5c-41c9-99c8-754be6895522_Series - Metadata.csv` | Ham verinin yer aldığı CSV dosyası             |
| **Toplam Satır**   |                                                      `1,397` | 1.325 veri satırı + 72 metadata satırı         |
| **Veri Satırı**    |                                                      `1,325` | 265 ülke/bölge × 5 yıl                         |
| **Sütun Sayısı**   |                                                         `41` | 4 kimlik bilgisi + 37 kalkınma göstergesi      |
| **Kapsanan Dönem** |                                                  `2021–2025` | Yıllık veriler                                 |
| **Coğrafi Kapsam** |                                                 `265 Entity` | Bağımsız ülkeler + bölgesel/ekonomik birlikler |
| **Veri Kaynağı**   |                                               World Bank WDI | World Development Indicators                   |

> **Not:** Dosyanın sonundaki 72 satır; kullanılan veri kaynakları, metodolojik dipnotlar ve lisans bilgileri gibi metadata açıklamalarını içermektedir.

---

# 📊 Dataset Yapısı

Veri setindeki 41 sütun, aşağıdaki **6 ana kategori** altında gruplandırılmıştır:

1. 🆔 Kimlik ve Zaman Bilgileri
2. 📈 Ekonomi, Dış Ticaret ve Doğal Kaynaklar
3. 💻 Teknoloji, Dijitalleşme ve Ar-Ge
4. 🌿 Enerji, Çevre ve İklim Değişikliği
5. 👥 Nüfus, Demografi ve Sağlık
6. 🎓 İşgücü ve Eğitim

---

## 1. 🆔 Kimlik ve Zaman Bilgileri

| Sütun Adı      | Kod / Format | Açıklama                                                                    |
| -------------- | ------------ | --------------------------------------------------------------------------- |
| `Time`         | `YYYY`       | Verinin ait olduğu yıl (2021, 2022, 2023, 2024, 2025).                      |
| `Time Code`    | `YRYYYY`     | Yılın kodlanmış hali. Örneğin `YR2021`.                                     |
| `Country Name` | `Metin`      | Ülke veya coğrafi/ekonomik bölge adı. Örneğin *Turkey*, *Germany*, *World*. |
| `Country Code` | `ISO-3`      | 3 harfli standart ülke/bölge kodu. Örneğin `TUR`, `DEU`, `WLD`.             |

---

## 2. 📈 Ekonomi, Dış Ticaret ve Doğal Kaynaklar

| Sütun Adı                                           | Gösterge Kodu          | Birim / Açıklama                                                                              |
| --------------------------------------------------- | ---------------------- | --------------------------------------------------------------------------------------------- |
| `GDP (constant 2015 US$)`                           | `NY.GDP.MKTP.KD`       | Sabit 2015 ABD Doları cinsinden Gayrisafi Yurtiçi Hasıla (reel GSYH).                         |
| `GDP growth (annual %)`                             | `NY.GDP.MKTP.KD.ZG`    | Yıllık reel GSYH büyüme oranı (%).                                                            |
| `GDP per capita (constant 2015 US$)`                | `NY.GDP.PCAP.KD`       | Kişi başına düşen reel GSYH (sabit 2015 ABD Doları).                                          |
| `Inflation, consumer prices (annual %)`             | `FP.CPI.TOTL.ZG`       | Tüketici Fiyat Endeksi (TÜFE) üzerinden hesaplanan yıllık enflasyon oranı (%).                |
| `Foreign direct investment, net inflows (% of GDP)` | `BX.KLT.DINV.WD.GD.ZS` | Net doğrudan yabancı yatırım girişlerinin GSYH'ye oranı (%).                                  |
| `Exports of goods and services (% of GDP)`          | `NE.EXP.GNFS.ZS`       | Mal ve hizmet ihracatının GSYH içindeki payı (%).                                             |
| `Imports of goods and services (% of GDP)`          | `NE.IMP.GNFS.ZS`       | Mal ve hizmet ithalatının GSYH içindeki payı (%).                                             |
| `Total natural resources rents (% of GDP)`          | `NY.GDP.TOTL.RT.ZS`    | Petrol, gaz, kömür, maden ve orman kaynaklarından elde edilen gelirin GSYH içindeki payı (%). |

---

## 3. 💻 Teknoloji, Dijitalleşme ve Ar-Ge

| Sütun Adı                                             | Gösterge Kodu       | Birim / Açıklama                                                        |
| ----------------------------------------------------- | ------------------- | ----------------------------------------------------------------------- |
| `Individuals using the Internet (% of population)`    | `IT.NET.USER.ZS`    | Toplam nüfus içinde internet kullanan bireylerin oranı (%).             |
| `Fixed broadband subscriptions (per 100 people)`      | `IT.NET.BBND.P2`    | Her 100 kişiye düşen sabit genişbant internet aboneliği sayısı.         |
| `Mobile cellular subscriptions (per 100 people)`      | `IT.CEL.SETS.P2`    | Her 100 kişiye düşen mobil telefon aboneliği sayısı.                    |
| `Secure Internet servers (per 1 million people)`      | `IT.NET.SECR.P6`    | Her 1 milyon kişiye düşen güvenli internet sunucusu (HTTPS/SSL) sayısı. |
| `High-technology exports (% of manufactured exports)` | `TX.VAL.TECH.MF.ZS` | Yüksek teknoloji ürünlerinin imalat sanayi ihracatındaki payı (%).      |
| `Research and development expenditure (% of GDP)`     | `GB.XPD.RSDV.GD.ZS` | Araştırma ve Geliştirme (Ar-Ge) harcamalarının GSYH içindeki payı (%).  |
| `Technicians in R&D (per million people)`             | `SP.POP.TECH.RD.P6` | Her 1 milyon kişiye düşen Ar-Ge alanında çalışan teknisyen sayısı.      |

---

## 4. 🌿 Enerji, Çevre ve İklim Değişikliği

| Sütun Adı                                                              | Gösterge Kodu          | Birim / Açıklama                                                                                            |
| ---------------------------------------------------------------------- | ---------------------- | ----------------------------------------------------------------------------------------------------------- |
| `Access to electricity (% of population)`                              | `EG.ELC.ACCS.ZS`       | Elektrik enerjisine erişimi olan nüfus oranı (%).                                                           |
| `Renewable energy consumption (% of total final energy consumption)`   | `EG.FEC.RNEW.ZS`       | Toplam nihai enerji tüketiminde yenilenebilir enerji kaynaklarının oranı (%).                               |
| `Forest area (% of land area)`                                         | `AG.LND.FRST.ZS`       | Toplam kara alanı içerisindeki ormanlık alan oranı (%).                                                     |
| `PM2.5 air pollution, mean annual exposure`                            | `EN.ATM.PM25.MC.M3`    | PM2.5 parçacıkları için yıllık ortalama maruz kalma düzeyi (μg/m³).                                         |
| `Energy use (kg of oil equivalent per capita)`                         | `EG.USE.PCAP.KG.OE`    | Kişi başına düşen birincil enerji kullanımı (kg petrol eşdeğeri).                                           |
| `Electricity production from coal sources (% of total)`                | `EG.ELC.COAL.ZS`       | Toplam elektrik üretiminde kömür kaynaklarının payı (%).                                                    |
| `Total greenhouse gas emissions excluding LULUCF (% change from 1990)` | `EN.GHG.TOT.ZG.AR5`    | Arazi kullanımı ve ormancılık hariç toplam sera gazı emisyonlarının 1990 yılına kıyasla yüzde değişimi (%). |
| `Total greenhouse gas emissions excluding LULUCF (Mt CO2e)`            | `EN.GHG.ALL.MT.CE.AR5` | Toplam sera gazı emisyon miktarı (Milyon Metrik Ton CO₂ Eşdeğeri).                                          |
| `Energy intensity level of primary energy (MJ/$2021 PPP GDP)`          | `EG.EGY.PRIM.PP.KD`    | Bir birim ekonomik çıktı üretmek için kullanılan enerji yoğunluğu (MJ).                                     |
| `Renewable electricity output (% of total electricity output)`         | `EG.ELC.RNEW.ZS`       | Toplam elektrik üretiminde yenilenebilir enerji kaynaklarının payı (%).                                     |
| `Nitrous oxide (N2O) emissions (total) excluding LULUCF (Mt CO2e)`     | `EN.GHG.N2O.MT.CE.AR5` | Toplam diazot monoksit (N₂O) emisyon miktarı (Mt CO₂e).                                                     |
| `Total fisheries production (metric tons)`                             | `ER.FSH.PROD.MT`       | Deniz ve iç su avcılığı ile su ürünleri yetiştiriciliğini kapsayan toplam balıkçılık üretimi (metrik ton).  |

---

## 5. 👥 Nüfus, Demografi ve Sağlık

| Sütun Adı                                  | Gösterge Kodu       | Birim / Açıklama                                            |
| ------------------------------------------ | ------------------- | ----------------------------------------------------------- |
| `Population, total`                        | `SP.POP.TOTL`       | Toplam nüfus sayısı.                                        |
| `Population, female`                       | `SP.POP.TOTL.FE.IN` | Toplam kadın nüfusu.                                        |
| `Population, male`                         | `SP.POP.TOTL.MA.IN` | Toplam erkek nüfusu.                                        |
| `Population growth (annual %)`             | `SP.POP.GROW`       | Yıllık nüfus artış oranı (%).                               |
| `Urban population (% of total population)` | `SP.URB.TOTL.IN.ZS` | Kent merkezlerinde yaşayan nüfusun toplam nüfusa oranı (%). |
| `Life expectancy at birth, total (years)`  | `SP.DYN.LE00.IN`    | Doğuşta beklenen ortalama yaşam süresi (yıl).               |

---

## 6. 🎓 İşgücü ve Eğitim

| Sütun Adı                                      | Gösterge Kodu    | Birim / Açıklama                                                   |
| ---------------------------------------------- | ---------------- | ------------------------------------------------------------------ |
| `Unemployment, total (% of total labor force)` | `SL.UEM.TOTL.ZS` | Toplam işgücü içerisindeki işsizlik oranı (ILO modeli tahmini, %). |
| `Labor force, total`                           | `SL.TLF.TOTL.IN` | Ekonomik olarak aktif olan toplam işgücü nüfusu.                   |
| `Compulsory education, duration (years)`       | `SE.COM.DURS`    | Yasal olarak zorunlu tutulan eğitim süresi (yıl).                  |
| `School enrollment, tertiary (% gross)`        | `SE.TER.ENRR`    | Yükseköğretime (üniversite/yüksekokul) brüt okullaşma oranı (%).   |

---

# 🔍 Kullanım Alanları ve Veri Analizi Fikirleri

### 1. Makroekonomik Analizler

GSYH büyümesi ile enflasyon, doğrudan yabancı yatırımlar ve dış ticaret oranları arasındaki ilişkiler incelenebilir.

### 2. Sürdürülebilirlik ve Yeşil Dönüşüm

Ülkelerin yenilenebilir enerji kullanımı, sera gazı emisyonları ve ormanlaşma oranları üzerinden çevresel performans skorları oluşturulabilir.

### 3. Dijital Dönüşüm Analizleri

İnternet kullanımı, sabit/mobil genişbant yaygınlığı ve güvenli internet sunucusu sayıları karşılaştırılarak ülkelerin dijital gelişmişlik düzeyleri analiz edilebilir.

### 4. Sosyal Kalkınma Göstergeleri

Doğuşta beklenen yaşam süresi, yükseköğretim okullaşma oranı ve işsizlik verileri kullanılarak sosyal ve insani gelişmişlik analizleri gerçekleştirilebilir.

### 5. Ülke Karşılaştırmaları

Ülkeler ekonomik, teknolojik, çevresel, demografik ve eğitim göstergeleri açısından karşılaştırılabilir.

### 6. Zaman Serisi Analizi

2021–2025 dönemindeki değişimler incelenerek ülkelerin ekonomik ve sosyal göstergelerindeki gelişim veya gerileme eğilimleri analiz edilebilir.

---

# 🧹 Veri Ön İşleme

Veri analizi öncesinde aşağıdaki işlemlerin uygulanması önerilir:

1. Metadata satırlarının veri analizinden ayrılması.
2. Sayısal değişkenlerin uygun veri tipine dönüştürülmesi.
3. Eksik değerlerin tespit edilmesi ve uygun şekilde ele alınması.
4. Ülke ve bölgesel/ekonomik grupların analiz amacına göre ayrıştırılması.
5. Aykırı değerlerin kontrol edilmesi.
6. Gerekli durumlarda değişkenlerin normalize veya standardize edilmesi.
7. Zaman serisi analizlerinde yıllara göre sıralamanın korunması.
8. Makine öğrenmesi çalışmalarında eğitim ve test verilerinin zaman boyutu dikkate alınarak ayrılması.

---

# 🌍 Coğrafi Kapsam

Veri seti toplam **265 entity** kapsamaktadır.

Bunlar:

* Bağımsız ülkeler
* Bölgesel gruplar
* Ekonomik birlikler
* Dünya toplamı
* Diğer Dünya Bankası tarafından tanımlanan ekonomik/coğrafi gruplar

gibi farklı entity türlerini içermektedir.

Örnekler:

```text
Turkey
Germany
United States
World
Arab World
Africa Eastern and Southern
```

---

# 📅 Zaman Aralığı

Veri setindeki gözlemler:

```text
2021
2022
2023
2024
2025
```

yıllarını kapsamaktadır.

Toplam veri yapısı:

```text
265 Entity × 5 Years = 1,325 Data Rows
```

şeklindedir.

---

# 📌 Veri Kaynağı

**World Development Indicators (WDI)**

**Kaynak:** Dünya Bankası (World Bank)

World Development Indicators; ekonomik, sosyal, çevresel, teknolojik, demografik ve eğitim alanlarında ülkeler ve ekonomiler hakkında çok sayıda uluslararası karşılaştırılabilir gösterge sağlayan kapsamlı bir veri kaynağıdır.

---

# 📄 Dosya Yapısı

```text
.
├── 21ff240d-8d5c-41c9-99c8-754be6895522_Series - Metadata.csv
└── README.md
```

---

# 📊 Dataset Özeti

| Metrik              |                 Değer |
| ------------------- | --------------------: |
| **Kaynak**          |      World Bank – WDI |
| **Dönem**           |             2021–2025 |
| **Entity Sayısı**   |                   265 |
| **Veri Satırı**     |                 1,325 |
| **Toplam Satır**    |                 1,397 |
| **Metadata Satırı** |                    72 |
| **Sütun Sayısı**    |                    41 |
| **Ana Kategori**    |                     6 |
| **Veri Türü**       | Yıllık / Zaman Serisi |

---

## 📜 Lisans ve Kullanım

Veri setinin kullanım koşulları, kaynak gösterimi ve lisans bilgileri için verinin alındığı **Dünya Bankası World Development Indicators** kaynak ve lisans koşullarının incelenmesi önerilir.


# World Development Indicators (WDI) Dataset (2021–2025)

Bu veri seti, **Dünya Bankası (World Bank)** tarafından yayınlanan **World Development Indicators (WDI)** veri tabanından aktarılmış küresel kalkınma göstergelerini içermektedir.

Veri seti; dünya üzerindeki bağımsız ülkelerin, bölgesel toplulukların ve ekonomik grupların **2021–2025** yılları arasındaki ekonomik, sosyo-demografik, teknolojik, çevresel ve enerji göstergelerini karşılaştırmalı olarak incelemek amacıyla kullanılabilir.

---

## 📁 1. Dosya Bilgileri

### Dosya Adı

```text
Data_Extract_FromWorld Development Indicators (1).xlsx
```

---

## 📊 2. Satır ve Sütun Sayıları

| Özellik                 |     Değer |
| ----------------------- | --------: |
| **Toplam Satır Sayısı** |     1.331 |
| **Toplam Sütun Sayısı** |        40 |
| **Veri Satırı**         |     1.325 |
| **Ülke/Bölge Sayısı**   |       265 |
| **Yıl Sayısı**          |         5 |
| **Dönem**               | 2021–2025 |

### Veri Yapısı

Veri tablosunda **5 ana yıl bloğu** bulunmaktadır:

* 2021
* 2022
* 2023
* 2024
* 2025

Her yıl bloğunda **265 ülke/bölge** verisi bulunmaktadır.

```text
5 Yıl × 265 Ülke/Bölge = 1.325 Veri Satırı
```

Geriye kalan **6 satır** ise yıl başlıkları ve dosyanın en alt kısmında bulunan World Bank kaynak/dipnot bilgisinden oluşmaktadır.

---

# 🌍 3. Veri Setinin Amacı

Bu veri seti, **World Bank – World Development Indicators (WDI)** veri tabanından alınan küresel kalkınma göstergelerini kapsamaktadır.

Veri setinde ülkelerin ve bölgesel/ekonomik grupların aşağıdaki alanlardaki gelişim seviyeleri incelenebilir:

* Ekonomik gelişmişlik
* Dış ticaret
* Doğrudan yabancı yatırımlar
* Nüfus ve demografi
* İşgücü
* Dijitalleşme
* Teknoloji
* Ar-Ge ve inovasyon
* Enerji
* Yenilenebilir enerji
* Çevre
* İklim değişikliği
* Eğitim
* Sağlık ve yaşam beklentisi

Veri setinde bağımsız ülkelerin yanı sıra **Arab World**, **Africa Eastern and Southern**, **World** gibi bölgesel ve ekonomik topluluklar da bulunmaktadır.

---

# 📑 4. Veri Setindeki Sütunlar

Veri setinde toplam **40 sütun** bulunmaktadır.

Bunlardan:

* 1 sütun yıl bloğu ayırıcısıdır.
* 1 sütun ülke/bölge adını içerir.
* 1 sütun boş yardımcı sütundur (`Unnamed: 4`).
* Geriye kalan sütunlar kalkınma göstergelerini içermektedir.

## A. 🗓️ Ülke ve Zaman Bilgileri

### 1. İlk Sütun

Yıl bloğu başlıklarını içerir:

```text
2021
2022
2023
2024
2025
```

### 2. `Unnamed: 1`

Ülke veya bölgesel küme adını içerir.

Örnek:

```text
Afghanistan
Albania
Turkey
World
```

---

# B. 📈 Ekonomik ve Ticari Göstergeler

### 3. `GDP (constant 2015 US$)`

Sabit 2015 ABD doları cinsinden Gayrisafi Yurt İçi Hasıla (GSYH).

### 4. `GDP growth (annual %)`

Yıllık reel GSYH büyüme oranı (%).

### 5. `GDP per capita (constant 2015 US$)`

Kişi başına düşen GSYH (2015 sabit ABD doları).

### 6. `Inflation, consumer prices (annual %)`

Tüketici fiyatları endeksine göre yıllık enflasyon oranı (%).

### 7. `Foreign direct investment, net inflows (% of GDP)`

Doğrudan yabancı yatırımların GSYH'ye oranı (%).

### 8. `Exports of goods and services (% of GDP)`

Mal ve hizmet ihracatının GSYH içindeki payı (%).

### 9. `Imports of goods and services (% of GDP)`

Mal ve hizmet ithalatının GSYH içindeki payı (%).

### 10. `Total natural resources rents (% of GDP)`

Toplam doğal kaynak gelirlerinin GSYH'ye oranı (%).

---

# C. 👥 Demografik ve İşgücü Göstergeleri

### 11. `Population, total`

Toplam ülke nüfusu.

### 12. `Population, female`

Toplam kadın nüfusu.

### 13. `Population, male`

Toplam erkek nüfusu.

### 14. `Population growth (annual %)`

Yıllık nüfus artış hızı (%).

### 15. `Urban population (% of total population)`

Kentsel alanlarda yaşayan nüfusun toplam nüfusa oranı (%).

### 16. `Life expectancy at birth, total (years)`

Doğumda beklenen ortalama yaşam süresi (yıl).

### 17. `Labor force, total`

Toplam işgücü sayısı.

### 18. `Unemployment, total (% of total labor force)`

Toplam işsizlik oranı (ILO tahmini, %).

---

# D. 💻 Teknoloji, Dijitalleşme ve Ar-Ge

### 19. `Individuals using the Internet (% of population)`

İnternet kullanan nüfusun toplam nüfusa oranı (%).

### 20. `Fixed broadband subscriptions (per 100 people)`

100 kişi başına düşen sabit geniş bant internet aboneliği.

### 21. `Mobile cellular subscriptions (per 100 people)`

100 kişi başına düşen mobil telefon aboneliği.

### 22. `Secure Internet servers (per 1 million people)`

1 milyon kişi başına düşen güvenli internet sunucusu sayısı.

### 23. `High-technology exports (% of manufactured exports)`

İmalat sanayi ihracatı içinde yüksek teknoloji ürünlerinin payı (%).

### 24. `Research and development expenditure (% of GDP)`

Ar-Ge harcamalarının GSYH'ye oranı (%).

### 25. `Technicians in R&D (per million people)`

Ar-Ge alanında çalışan milyon kişi başına düşen teknisyen sayısı.

---

# E. 🌿 Çevre, Enerji ve Doğal Kaynaklar

### 26. `Access to electricity (% of population)`

Elektriğe erişimi olan nüfus oranı (%).

### 27. `Renewable energy consumption (% of total final energy consumption)`

Yenilenebilir enerji tüketiminin toplam nihai enerji tüketimine oranı (%).

### 28. `Renewable electricity output (% of total electricity output)`

Toplam elektrik üretiminde yenilenebilir enerji kaynaklarının payı (%).

### 29. `Electricity production from coal sources (% of total)`

Kömür kaynaklarından elde edilen elektrik üretiminin toplam elektrik üretimindeki oranı (%).

### 30. `Energy use (kg of oil equivalent per capita)`

Kişi başına enerji kullanımı (kg petrol eşdeğeri).

### 31. `Energy intensity level of primary energy`

Birincil enerji yoğunluk seviyesi (MJ/$2021 PPP GSYH).

### 32. `Forest area (% of land area)`

Ormanlık alanların toplam kara alanına oranı (%).

### 33. `PM2.5 air pollution, mean annual exposure`

PM2.5 hava kirliliğine yıllık ortalama maruz kalma düzeyi (μg/m³).

### 34. `Total greenhouse gas emissions excluding LULUCF (% change from 1990)`

Toplam sera gazı emisyonlarının 1990 yılına göre değişim oranı (%).

### 35. `Total greenhouse gas emissions excluding LULUCF (Mt CO2e)`

Toplam sera gazı emisyonu (Mt CO₂ eşdeğeri).

### 36. `Nitrous oxide (N2O) emissions (total) excluding LULUCF (Mt CO2e)`

Azot oksit (N₂O) emisyonu (Mt CO₂ eşdeğeri).

### 37. `Total fisheries production (metric tons)`

Toplam su ürünleri/balıkçılık üretimi (metrik ton).

---

# F. 🎓 Eğitim

### 38. `Compulsory education, duration (years)`

Zorunlu eğitim süresi (yıl).

### 39. `School enrollment, tertiary (% gross)`

Yükseköğretim/üniversite brüt okullaşma oranı (%).

---

# 📌 5. Veri Seti Kategorileri

| Kategori                          |             Gösterge Sayısı |
| --------------------------------- | --------------------------: |
| Ülke ve Zaman Bilgileri           |                           2 |
| Ekonomik ve Ticari Göstergeler    |                           8 |
| Demografik ve İşgücü Göstergeleri |                           8 |
| Teknoloji, Dijitalleşme ve Ar-Ge  |                           7 |
| Çevre, Enerji ve Doğal Kaynaklar  |                          12 |
| Eğitim                            |                           2 |
| **Toplam**                        | **39 gösterge/bilgi alanı** |

---

# 🔍 6. Kullanım Alanları

Bu veri seti aşağıdaki analiz ve araştırmalarda kullanılabilir:

### Ekonomik Analiz

* GSYH karşılaştırmaları
* GSYH büyüme analizi
* Kişi başına GSYH karşılaştırmaları
* Enflasyon analizi
* Doğrudan yabancı yatırım analizi
* İthalat ve ihracat karşılaştırmaları

### 🌐 Dijitalleşme ve Teknoloji

* İnternet kullanım oranlarının karşılaştırılması
* Geniş bant internet yaygınlığının analizi
* Mobil iletişim altyapısının incelenmesi
* Güvenli internet sunucularının karşılaştırılması
* Yüksek teknoloji ihracatının incelenmesi
* Ar-Ge yatırımlarının analiz edilmesi

### 🌱 Çevre ve Sürdürülebilirlik

* Yenilenebilir enerji kullanımının karşılaştırılması
* Kömür kaynaklı elektrik üretiminin analizi
* Sera gazı emisyonlarının incelenmesi
* PM2.5 hava kirliliği analizi
* Orman alanlarının karşılaştırılması
* Enerji yoğunluğu analizi

### 👥 Demografi ve Sosyal Gelişmişlik

* Nüfus değişimi
* Kentleşme oranları
* Kadın/erkek nüfus karşılaştırmaları
* Yaşam beklentisi analizi
* İşsizlik analizi
* İşgücü büyüklüğü karşılaştırmaları

### 🎓 Eğitim

* Zorunlu eğitim sürelerinin karşılaştırılması
* Yükseköğretim okullaşma oranlarının analizi
* Eğitim ve ekonomik gelişmişlik arasındaki ilişkilerin incelenmesi

---

# 📊 7. Veri Analizi Önerileri

Bu veri seti kullanılarak aşağıdaki çalışmalar gerçekleştirilebilir:

1. Ülkelerin ekonomik gelişmişliklerinin karşılaştırılması.
2. Dijitalleşme ve ekonomik büyüme arasındaki ilişkinin incelenmesi.
3. Ar-Ge yatırımları ile yüksek teknoloji ihracatı arasındaki ilişkinin analiz edilmesi.
4. Yenilenebilir enerji kullanımı ile sera gazı emisyonlarının karşılaştırılması.
5. Eğitim seviyesi ile ekonomik gelişmişlik arasındaki ilişkinin incelenmesi.
6. İşsizlik ve GSYH büyümesi arasındaki ilişkinin araştırılması.
7. Ülkelerin çok boyutlu gelişmişlik skorlarının oluşturulması.
8. 2021–2025 dönemindeki değişimlerin zaman serisi olarak incelenmesi.
9. Ülkelerin benzer özelliklerine göre kümelenmesi.
10. Makine öğrenmesi yöntemleriyle kalkınma göstergelerinin tahmin edilmesi.

---

# 🧹 8. Veri Ön İşleme

Veri analizi gerçekleştirilmeden önce aşağıdaki işlemlerin uygulanması önerilir:

* Yıl başlığı satırlarının ayrıştırılması.
* Boş yardımcı sütunların kontrol edilmesi.
* Ülke/bölge adlarının standartlaştırılması.
* Sayısal sütunların uygun veri tiplerine dönüştürülmesi.
* Eksik verilerin tespit edilmesi.
* Aykırı değerlerin kontrol edilmesi.
* Gerekli durumlarda değişkenlerin normalize edilmesi.
* Zaman serisi analizlerinde yılların doğru sırada tutulması.
* Makine öğrenmesi modellerinde eğitim ve test verilerinin uygun şekilde ayrılması.

---

# 📁 9. Dosya Yapısı

```text
.
├── Data_Extract_FromWorld Development Indicators (1).xlsx
└── README.md
```

---

# 🌍 10. Veri Kaynağı

**World Bank – World Development Indicators (WDI)**

Veri seti, Dünya Bankası tarafından yayımlanan World Development Indicators veri tabanından aktarılmıştır.

WDI; ülkeler ve ekonomiler hakkında ekonomik, sosyal, çevresel, teknolojik, demografik ve eğitim alanlarında çok sayıda gösterge sağlayan uluslararası bir veri kaynağıdır.

---

# 📈 11. Dataset Özeti

| Özellik                |            Değer |
| ---------------------- | ---------------: |
| **Veri Kaynağı**       | World Bank – WDI |
| **Dönem**              |        2021–2025 |
| **Ülke/Bölge**         |              265 |
| **Veri Satırı**        |            1.325 |
| **Toplam Satır**       |            1.331 |
| **Toplam Sütun**       |               40 |
| **Ana Gösterge Alanı** |               38 |
| **Yıl**                |                5 |
| **Dosya Formatı**      |             XLSX |

---

## 📄 Lisans ve Kullanım

Veri setinin kullanım koşulları ve lisans bilgileri için verinin alındığı **World Bank – World Development Indicators (WDI)** kaynak ve lisans koşullarının incelenmesi önerilir.

---

## ⭐ Kaynak

**World Bank – World Development Indicators (WDI)**

Bu veri seti, Dünya Bankası'nın küresel kalkınma göstergelerinden yararlanılarak oluşturulmuştur.

# World Development Indicators (WDI) Dataset

## 1. Dataset Hakkında

Bu veri seti, **Dünya Bankası (World Bank) – World Development Indicators (WDI)** veritabanından elde edilen, ülkelerin ve bölgesel/ekonomik grupların 2021–2025 yılları arasındaki sosyo-ekonomik, çevresel ve teknolojik gelişim göstergelerini içeren bir Excel veri setidir.

Dataset; ekonomi, nüfus, işgücü, teknoloji, dijitalleşme, enerji, çevre, AR-GE, eğitim ve doğal kaynaklar gibi farklı alanlardaki göstergelerin ülkeler ve bölgeler arasında karşılaştırılmasına olanak sağlar.

---

## 2. Dosya Bilgileri

| Özellik                    | Bilgi                                                   |
| -------------------------- | ------------------------------------------------------- |
| **Dosya Adı**              | `P_Data_Extract_From_World_Development_Indicators.xlsx` |
| **Veri Kaynağı**           | World Bank – World Development Indicators (WDI)         |
| **Çalışma Sayfası Sayısı** | 2                                                       |
| **Ana Veri Sayfası**       | `Data`                                                  |
| **Meta Veri Sayfası**      | `Series - Metadata`                                     |
| **Yıl Aralığı**            | 2021–2025                                               |
| **Yıl Sayısı**             | 5                                                       |
| **Ülke/Bölge Sayısı**      | 265                                                     |
| **Ana Veri Sütun Sayısı**  | 41                                                      |

---

## 3. Çalışma Sayfaları

### `Data`

Ana veri tablosudur. Ülkeler ve bölgesel/ekonomik gruplar için 2021–2025 dönemine ait göstergeleri içerir.

* **Toplam satır sayısı:** 1.330
* **Net veri satırı:** 1.325
* **Sütun sayısı:** 41
* **Ülke/Bölge sayısı:** 265
* **Yıl aralığı:** 2021–2025

Son 5 satır veri dipnotu ve boşluk içerdiğinden net veri satırı sayısı **1.325** olarak değerlendirilmiştir.

### `Series - Metadata`

Veri setinde kullanılan göstergelerin teknik açıklamalarını içeren meta veri tablosudur.

* **Gösterge tanımı:** 37
* **Meta veri sütunu:** 16

Bu sayfa; gösterge kodları, lisans, kaynak, metodoloji ve göstergelere ilişkin diğer teknik bilgileri içerir.

---

## 4. Dataset Temaları

Dataset beş ana tema altında değerlendirilebilir:

### 1. Ekonomi ve Finans

Ülkelerin ekonomik büyüklüklerini ve ekonomik performanslarını incelemek için kullanılan göstergeleri içerir.

* Gayrisafi Yurtiçi Hasıla (GDP)
* GDP büyüme oranı
* Kişi başına GDP
* Enflasyon
* Doğrudan Yabancı Yatırım (FDI)
* İhracat
* İthalat

### 2. Nüfus ve İşgücü

Nüfus yapısını, demografik değişimleri ve işgücü piyasasını açıklayan göstergeleri içerir.

* Toplam nüfus
* Kadın nüfusu
* Erkek nüfusu
* Nüfus artış oranı
* Kentsel nüfus
* Yaşam beklentisi
* İşsizlik
* Toplam işgücü

### 3. Çevre, Enerji ve İklim

Enerji kullanımı, yenilenebilir enerji, çevresel koşullar ve sera gazı emisyonlarına ilişkin göstergeleri kapsar.

* Elektriğe erişim
* Yenilenebilir enerji tüketimi
* Yenilenebilir elektrik üretimi
* Kömür kaynaklı elektrik üretimi
* Enerji kullanımı
* Enerji yoğunluğu
* Ormanlık alan
* PM2.5 hava kirliliği
* Sera gazı emisyonları
* Nitroz oksit emisyonları
* Doğal kaynak rantları

### 4. Teknoloji, AR-GE ve Altyapı

Dijitalleşme, teknoloji kullanımı ve araştırma-geliştirme kapasitesini ölçen göstergeleri içerir.

* İnternet kullanım oranı
* Sabit geniş bant abonelikleri
* Mobil hücresel abonelikler
* Güvenli internet sunucuları
* Yüksek teknoloji ihracatı
* AR-GE harcamaları
* AR-GE teknisyenleri

### 5. Eğitim ve Üretim

Eğitim sisteminin kapsamını ve balıkçılık üretimini gösteren değişkenleri içerir.

* Zorunlu eğitim süresi
* Yükseköğretim brüt okullaşma oranı
* Toplam balıkçılık üretimi

---

## 5. Sütunların Detaylı Açıklaması

### A. Kimlik ve Zaman Bilgileri

| # | Sütun          | Açıklama                                |
| - | -------------- | --------------------------------------- |
| 1 | `Time`         | Verinin ait olduğu yıl: 2021–2025       |
| 2 | `Time Code`    | Yılın kodlanmış hali, ör. `YR2021`      |
| 3 | `Country Name` | Ülke veya bölgesel grubun adı           |
| 4 | `Country Code` | Ülkenin 3 harfli ISO/Dünya Bankası kodu |

---

### B. Makroekonomik Göstergeler

| #  | Sütun                                               | Açıklama                                                 |
| -- | --------------------------------------------------- | -------------------------------------------------------- |
| 5  | `GDP (constant 2015 US$)`                           | Sabit 2015 ABD Doları cinsinden Gayrisafi Yurtiçi Hasıla |
| 6  | `GDP growth (annual %)`                             | Yıllık GSYH büyüme oranı                                 |
| 7  | `GDP per capita (constant 2015 US$)`                | Kişi başına düşen sabit GSYH                             |
| 8  | `Inflation, consumer prices (annual %)`             | Tüketici Fiyat Endeksi bazlı yıllık enflasyon oranı      |
| 9  | `Foreign direct investment, net inflows (% of GDP)` | Net doğrudan yabancı yatırım girişlerinin GSYH'ye oranı  |
| 10 | `Exports of goods and services (% of GDP)`          | Mal ve hizmet ihracatının GSYH'ye oranı                  |
| 11 | `Imports of goods and services (% of GDP)`          | Mal ve hizmet ithalatının GSYH'ye oranı                  |

---

### C. Dijital Dönüşüm ve Teknoloji

| #  | Sütun                                                 | Açıklama                                                  |
| -- | ----------------------------------------------------- | --------------------------------------------------------- |
| 12 | `Individuals using the Internet (% of population)`    | İnternet kullanan bireylerin nüfusa oranı                 |
| 13 | `Fixed broadband subscriptions (per 100 people)`      | Her 100 kişiye düşen sabit geniş bant aboneliği           |
| 14 | `Mobile cellular subscriptions (per 100 people)`      | Her 100 kişiye düşen mobil hat aboneliği                  |
| 15 | `Secure Internet servers (per 1 million people)`      | 1 milyon kişiye düşen güvenli internet sunucusu           |
| 16 | `High-technology exports (% of manufactured exports)` | Yüksek teknoloji ürün ihracatının imalat ihracatına oranı |

---

### D. Enerji, AR-GE ve Çevre

| #  | Sütun                                                                | Açıklama                                                     |
| -- | -------------------------------------------------------------------- | ------------------------------------------------------------ |
| 17 | `Access to electricity (% of population)`                            | Elektriğe erişimi olan nüfusun oranı                         |
| 18 | `Research and development expenditure (% of GDP)`                    | AR-GE harcamalarının GSYH'ye oranı                           |
| 19 | `Technicians in R&D (per million people)`                            | 1 milyon kişiye düşen AR-GE teknisyeni sayısı                |
| 20 | `Renewable energy consumption (% of total final energy consumption)` | Yenilenebilir enerjinin toplam enerji tüketimindeki payı     |
| 21 | `Forest area (% of land area)`                                       | Ormanlık alanların toplam kara alanına oranı                 |
| 22 | `PM2.5 air pollution, mean annual exposure`                          | Yıllık ortalama PM2.5 hava kirliliği maruziyeti              |
| 23 | `Energy use (kg of oil equivalent per capita)`                       | Kişi başına düşen enerji kullanımı                           |
| 24 | `Electricity production from coal sources (% of total)`              | Kömürden üretilen elektriğin toplam elektrik üretimine oranı |

---

### E. Demografi ve İşgücü

| #  | Sütun                                          | Açıklama                            |
| -- | ---------------------------------------------- | ----------------------------------- |
| 25 | `Population, total`                            | Toplam nüfus                        |
| 26 | `Population, female`                           | Toplam kadın nüfusu                 |
| 27 | `Population, male`                             | Toplam erkek nüfusu                 |
| 28 | `Population growth (annual %)`                 | Yıllık nüfus artış oranı            |
| 29 | `Urban population (% of total population)`     | Kentsel nüfusun toplam nüfusa oranı |
| 30 | `Life expectancy at birth, total (years)`      | Doğumda beklenen yaşam süresi       |
| 31 | `Unemployment, total (% of total labor force)` | Toplam işsizlik oranı               |
| 32 | `Labor force, total`                           | Toplam işgücü sayısı                |

---

### F. Eğitim, Emisyon ve Kaynaklar

| #  | Sütun                                                                  | Açıklama                                               |
| -- | ---------------------------------------------------------------------- | ------------------------------------------------------ |
| 33 | `Compulsory education, duration (years)`                               | Zorunlu eğitimin süresi                                |
| 34 | `School enrollment, tertiary (% gross)`                                | Yükseköğretim brüt okullaşma oranı                     |
| 35 | `Total greenhouse gas emissions excluding LULUCF (% change from 1990)` | Toplam sera gazı emisyonlarının 1990'a göre değişimi   |
| 36 | `Total greenhouse gas emissions excluding LULUCF (Mt CO2e)`            | Toplam sera gazı emisyonu, milyon ton CO₂ eşdeğeri     |
| 37 | `Total natural resources rents (% of GDP)`                             | Doğal kaynak rantlarının GSYH içindeki payı            |
| 38 | `Energy intensity level of primary energy (MJ/$2021 PPP GDP)`          | Birincil enerjinin enerji yoğunluğu düzeyi             |
| 39 | `Renewable electricity output (% of total electricity output)`         | Yenilenebilir elektrik üretiminin toplam üretime oranı |
| 40 | `Nitrous oxide (N2O) emissions (total) excluding LULUCF (Mt CO2e)`     | Toplam Nitroz Oksit (N₂O) emisyonu                     |
| 41 | `Total fisheries production (metric tons)`                             | Toplam balıkçılık üretimi                              |

---

## 6. Veri Kapsamı

Dataset toplam **265 ülke/bölge** ve **5 yıllık dönem** kapsamaktadır.

### Yıllar

* 2021
* 2022
* 2023
* 2024
* 2025

### Ülke ve Bölgesel Gruplar

Dataset yalnızca bağımsız ülkeleri değil, aynı zamanda çeşitli bölgesel ve ekonomik grupları da kapsamaktadır.

Örnekler:

* Afghanistan
* Albania
* Türkiye
* Arab World
* Africa Eastern and Southern
* World

Bu yapı, ülkeler ile bölgesel/ekonomik grupların aynı göstergeler üzerinden karşılaştırılmasına olanak sağlar.

---

## 7. Kullanım Alanları

Dataset aşağıdaki analiz ve araştırma alanlarında kullanılabilir:

* Ülkelerin ekonomik gelişmişliklerinin karşılaştırılması
* GDP ve GDP büyüme analizi
* Kişi başına gelir karşılaştırmaları
* Enflasyon ve ekonomik performans analizi
* Nüfus ve demografik trend analizi
* İşsizlik ve işgücü piyasası analizi
* Dijitalleşme ve internet kullanım analizi
* Teknolojik altyapı karşılaştırmaları
* AR-GE kapasitesi ve harcama analizi
* Enerji tüketimi ve enerji yoğunluğu analizi
* Yenilenebilir enerji karşılaştırmaları
* Çevresel performans analizi
* Sera gazı ve N₂O emisyonlarının incelenmesi
* PM2.5 hava kirliliği karşılaştırmaları
* Eğitim göstergelerinin karşılaştırılması
* Ülkeler ve bölgeler arasında çok değişkenli gelişmişlik analizleri
* Veri görselleştirme ve istatistiksel analiz
* Makine öğrenmesi ve tahmin modelleri

---

## 8. Örnek Analiz Soruları

Bu veri seti kullanılarak aşağıdaki sorular incelenebilir:

1. 2021–2025 döneminde hangi ülkelerde GDP büyümesi daha yüksektir?
2. Kişi başına GDP ile internet kullanım oranı arasında bir ilişki var mıdır?
3. AR-GE harcamaları ile yüksek teknoloji ihracatı arasında ilişki bulunuyor mu?
4. Yenilenebilir enerji kullanımı ile sera gazı emisyonları arasında nasıl bir ilişki vardır?
5. Ülkelerin kentleşme oranları ile kişi başına GDP arasında ilişki var mıdır?
6. İnternet kullanım oranı ve sabit geniş bant abonelikleri yıllar içinde nasıl değişmiştir?
7. Enerji yoğunluğu ile ekonomik gelişmişlik arasında nasıl bir ilişki vardır?
8. PM2.5 hava kirliliği ülkeler arasında nasıl farklılaşmaktadır?
9. Eğitim süresi ve yükseköğretim okullaşma oranı hangi ülkelerde daha yüksektir?
10. Ülkelerin ekonomik, teknolojik ve çevresel göstergeleri birlikte değerlendirildiğinde nasıl bir gelişmişlik profili ortaya çıkmaktadır?

---

## 9. Veri Yapısı

Ana `Data` sayfasındaki her kayıt, bir ülke/bölge ve belirli bir yıl için göstergelerin değerlerini temsil eder.

Temel yapı:

```text
Time
Time Code
Country Name
Country Code
        ↓
Economic Indicators
Technology Indicators
Energy & Environmental Indicators
Demographic & Labor Indicators
Education & Resource Indicators
```

Bu yapı sayesinde veri, ülke ve yıl bazında filtrelenebilir ve karşılaştırmalı analizlerde kullanılabilir.

---

## 10. Veri Kaynağı

**Kaynak:** World Bank – World Development Indicators (WDI)

WDI, dünya ülkeleri ve bölgelerine ilişkin ekonomik, sosyal, çevresel, teknolojik ve demografik göstergeleri sağlayan Dünya Bankası veri kaynağıdır.

Dataset içerisindeki `Series - Metadata` sayfası, kullanılan göstergelerin teknik tanımları, kaynakları ve metodolojik bilgileri için referans olarak kullanılabilir.

---

## 11. Dosya Yapısı

```text
P_Data_Extract_From_World_Development_Indicators.xlsx
│
├── Data
│   ├── Time
│   ├── Time Code
│   ├── Country Name
│   ├── Country Code
│   ├── Economic Indicators
│   ├── Technology Indicators
│   ├── Energy & Environmental Indicators
│   ├── Demographic & Labor Indicators
│   └── Education & Resource Indicators
│
└── Series - Metadata
    ├── Indicator Definitions
    ├── Indicator Codes
    ├── Sources
    ├── Methodology
    └── License / Metadata Information
```

---

## 12. Özet

`P_Data_Extract_From_World_Development_Indicators.xlsx`, Dünya Bankası'nın **World Development Indicators (WDI)** veri kaynağından alınan ve **2021–2025** dönemini kapsayan çok boyutlu bir ülke ve bölge veri setidir.

Dataset:

* **265 ülke/bölge**
* **5 yıl**
* **41 veri sütunu**
* **1.325 net veri satırı**
* **37 gösterge tanımı**
* **16 meta veri sütunu**

içermektedir.

Veri seti; **ekonomi, nüfus ve işgücü, teknoloji ve dijitalleşme, enerji, çevre, AR-GE, eğitim ve doğal kaynaklar** gibi farklı alanları birlikte incelemeye olanak sağlamaktadır.

Bu nedenle dataset; keşifsel veri analizi (EDA), istatistiksel analiz, veri görselleştirme, karşılaştırmalı ülke analizi ve makine öğrenmesi çalışmalarında kullanılabilecek çok boyutlu bir veri kaynağıdır.

---

## 13. Lisans ve Kullanım

Veri, **World Bank – World Development Indicators (WDI)** kaynağından alınmıştır.

Verinin yeniden kullanımı, dağıtımı ve atıf koşulları için Dünya Bankası'nın ilgili veri kullanım ve lisans koşulları ile `Series - Metadata` sayfasındaki lisans bilgileri dikkate alınmalıdır.


