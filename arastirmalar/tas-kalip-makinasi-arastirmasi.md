# Metraj Taş Baskı Kalıp Yapım Makinası Araştırma Raporu

**Tarih:** 10 Kasım 2026  
**Hazırlayan Ekip:** Tekir (Koordinasyon) · Siyam (Pazar & Teknik Araştırma) · Van (Finans & Yatırım Analizi)  
**Hedef:** Müşteriden gelen özel desen/kalıp taleplerini bekletmeden, Obour fabrikası bünyesinde kendi kalıplarını üretip anında yanıt ve numune verebilmek.

---

## 1. Mevcut Makine ve Kalıp Tespiti (Fabrika Videolarından)

Fabrika klipleri (`E:\ab ayçam\premiere pro\21 - geniş kumaş\videolar 17T\` içindeki `VID_20261010_165315.mp4`, `VID20260430182123.mp4`, `VID20260915192152.mp4`) incelenerek mevcut üretim hattının yapısı doğrulandı:

- **Kullanılan Makine Tipi:** Rulo/metraj kumaş üzerine kesintisiz hotfix strass taş basan **konveyör/kalıp bantlı metraj taş baskı makinası** (proje kayıtlarına göre **3,20 metre** ene kadar baskı kapasiteli).
- **Mevcut Kalıp (Şablon) Yapısı:** Makine sert metal tambur veya tekil tişört şablonu değil, rulolar üzerinde dönen **delikli esnek sonsuz kalıp bandı** kullanmaktadır:
  - Alt yüzü dokuma takviyeli **yeşil delikli bant** (üzerinde birleştirme/ek izi görülmektedir),
  - Pürüzsüz yüzeyli **siyah delikli esnek bant/levha**.
- **Anlamı:** Alınacak kalıp makinasının **küçük masaüstü A3/A4 tişört şablonu** değil, **geniş enli (160–320 cm arası) rulo veya düz şerit bantları** yüksek hızda ve binlerce delik için hassas delebilecek kapasitede olması gerekir.

### Alım Öncesi Fabrikada Teyit Edilmesi Gereken 3 Kritik Ölçü
1. **Bant Hammaddesi:** Mevcut yeşil ve siyah kalıp bantları **PVC** mi, yoksa **PU (Poliüretan) / PET (Mylar) / kauçuk** mu? *(Lazer mi CNC mi kararını tek başına bu belirler.)*
2. **Net Bant Eni ve Çevresi:** 3,20 m baskı eni tek parça **320 cm** bantla mı, yoksa daha dar (ör. **160–180 cm**) bir bantla mı sağlanıyor? Çevre uzunluğu kaç metre?
3. **Delik Tipi ve Ekleme:** Delikler düz silindirik mi yoksa konik/havşalı mı? Delinen bant düz açılıp sonradan sıcak presle mi sonsuz banda dönüştürülüyor?

---

## 2. Kritik Teknik Uyarı: PVC Bantta Lazer Kullanılamaz

Araştırmada doğrulanmış en kritik tuzak **malzeme–makine uyumudur** (`gwklaser.com`, `xometry.com`, `darklylabs.com`):

| Kalıp Bandı Malzemesi | CO2 / Galvo Lazer | Mekanik CNC (Router / Zımba) | Neden? |
| :--- | :--- | :--- | :--- |
| **PVC (Polivinil Klorür)** | **KESİNLİKLE YASAK** | **GÜVENLİ / UYGUN** | PVC ağırlığının ~%57'si klordur. Lazerle yandığında **hidrojen klorür (HCl) asit gazı** çıkarır; bu gaz nemle birleşip **hidroklorik aside** dönüşerek lazer lenslerini, aynaları, rayları ve elektroniği haftalar içinde çürütür, operatör sağlığını tehdit eder. |
| **PU (Poliüretan) / PET (Mylar) / Silikon / Kauçuk** | **EN HIZLI & UYGUN** | **UYGUN** | Klor içermez. Özellikle Galvo CO2 lazerde çok temiz, çapaksız delikler açar. |

**Pratik Kural:** Mevcut bantlarınız **PVC** ise ya **CNC Router / CNC Bant Delme** almalı ya da kalıp hammaddenizi lazer uyumlu **PU / PET** banda geçirmelisiniz.

---

## 3. Makine Seçenekleri Karşılaştırma Tablosu

| Makine Türü | Çalışma Prensibi & En | Delme Hızı & Çap | Avantajları | Dezavantajları / Riskleri | Tahmini Fiyat (Kasım 2026) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **1. Konveyörlü Galvo / Hibrit Gantry-Galvo CO2 Lazer** | Rulo beslemeli konveyör + ayna taramalı (Galvo) veya hibrit kafa (~160 cm en) | **1.000 – 3.000+ delik/dk** · SS6 (~2 mm) – SS20 tüm çaplar yazılımla değişir | **En hızlı çözüm.** 20.000 delikli bir deseni dakikalar/saat içinde bitirir; uç kırılması yok. | **PVC yasak** (sadece PU/PET/kauçuk/akrilik). Cam tüp yerine uzun ömürlü **RF metal tüp** önerilir. | **Çin FOB:** Giriş cam tüplü $8.000–$15.000 · Endüstriyel RF metal tüplü / hibrit **$18.000 – $35.000+** *(+Mısır nakliye/gümrük)* |
| **2. Konveyörlü Flatbed (Gantry) CO2 Lazer** (`1610` / `1810` / `1820`) | 160x100 veya 180x100/200 cm konveyör yataklı klasik hareketli köprü lazer | **150 – 400 delik/dk** · SS6–SS20 yazılımla değişir | Geniş en (160–180 cm) rulo sürme özelliği ve düşük bütçeli başlangıç. | Kafa her delikte dur-kalk yaptığı için Galvo'ya kıyasla 5–10 kat yavaştır. **PVC yasak.** | **Çin FOB:** Tek kafa 80–130W $3.500–$7.000 · Çift kafa/servo/CCD $7.000–$14.000+ · **Mısır yerel (90x60–130x90):** 140.000–260.000 EGP |
| **3. Vakumlu Endüstriyel CNC Router** (`1325` / `1630` / `2030`) | 24.000 RPM yüksek devirli spindle ile matkap/freze delme | Gantry mekanik hız (Galvo'dan yavaş, zımbadan esnek) · 2 mm+ matkap/freze | **PVC, PU, akrilik, bakalit, alüminyum hepsini deler.** Asit gazı yok. Konik/havşalı delik açabilir. Mısır'da yerli üretim/servis güçlü. | Küçük 2 mm matkap uçlarında kırılma/ısınma olmaması için doğru devir ve vakum şart. 3,20 m tam en için özel 200x300+ tabla gerekir. | **Mısır yerel (Kahire, 130x250 cm):** Standart 80.000–260.000 EGP · ATC/çok kafalı 260.000–480.000+ EGP (~**$1.500–$8.900** karşılığı; taksit var) |
| **4. CNC Konveyör Bant Zımba Makinası** (Belt Perforator) | Servo kontrollü mekanik zımba pimi (1600 / 2000 / 3000+ mm) | **30 – 50 delik/dk** · Standart pimler genelde **3 mm+** | **PVC ve PU** bantları sıfır duman ve sıfır yanıkla temiz zımbalar. | **Taş kalıbı için hız ve çap riski:** 2 mm (SS6) ince pimler kolay kırılır; 30–50 delik/dk hızla 20.000 delikli tek bir kalıp **7–11 saat** sürer. | **Çin FOB:** 1600 mm $4.500–$9.000 · 2000 mm $7.000–$14.000 · 3000+ mm $12.000–$22.000+ |
| **Ek: PVC/PU Bant Sıcak Ekleme Presi** *(Gerekirse)* | Delinen düz şeridi sonsuz banda kaynaklayan sıcak pres | 1600 / 2000 / 3200 mm en | Kalıbı düz şerit olarak delip fabrikada kendi sonsuz bandınızı kapatmanızı sağlar. | Kalıpları hazır ekli satın almıyorsanız veya yerel bantçıda ekletmeyecekseniz ek bütçe gerektirir. | **Çin FOB:** 1600 mm $2.500–$5.500 · 2000 mm $3.500–$7.500 · 3200 mm $7.000–$15.000+ |

> **Not:** Küçük parça/tişört taş şablonu (kauçuk/flock/Mylar) kesilecekse 40x40 / 60x60 cm mini hassas CNC ($2.600–$4.900 FOB) veya küçük CO2 lazer ($1.500–$4.500 FOB) yeterlidir; ancak **metraj kumaş makinesinin kalıp bandı** için en az **160 cm ve üzeri** iş genişliği gerekir.

---

## 4. Tedarik Coğrafyası: Mısır Yerel vs Çin vs Türkiye

### Mısır Kur & İthalat Gerçeği (Kasım 2026)
- **Banka Kuru (CBE):** ~53,92 – 54,02 EGP / USD (`cbe.org.eg`)
- **Resmî Gümrük Kuru:** **54,31 EGP / USD** (`customs.gov.eg`, `nafeza.gov.eg`)
- **İthalat Yükü:** Çin veya Türkiye'den makine getirirken FOB fiyata deniz navlunu + **Nafeza / ACID** ön kayıt + gümrük vergisi + **%14 KDV (VAT)** + EOS uygunluk denetimi eklenir. Toplam maliyet tipik olarak FOB fiyatının **%20–35+ üzerine** çıkar ve 4–8+ haftalık lojistik/gümrük süresi alır.

### Öne Çıkan Tedarikçiler
- **Mısır (Kahire / Obour'a Yakın Yerel Tedarik & Taksit + 1 Yıl Garanti):**
  - **Simplex Arabia** (`simplexarabia.net`) — Mısır'ın önde gelen yerel CNC üreticilerinden (130x250 cm ve özel ölçü CNC Router & CO2 lazerler, taksit ve yerel servis).
  - **Top Laser Egypt** (`toplaser-eg.com`) — Kahire şubeleri, CO2 lazer & CNC router tedariki, yedek parça ve 1 yıl garanti.
  - **CNC Falcon** (`cncfalcon.com`) — Mısır yerel CNC router ve lazer üretimi/satışı, taksit imkânları.
  - **Miracle4Laser** (`miracle4laser.com`) — Büyük ebat CO2 lazerler.
- **Çin (Fabrika Çıkışı Özel Makinalar):**
  - *Galvo / Konveyörlü Lazer:* **Golden Laser**, **MimoWork**, **Han's Yueming Laser**, **Redshift Laser**, **Dowin Laser** (Guangdong / Shandong / Zhejiang).
  - *Bant Delme & Sıcak Ekleme Presi:* **Beltwin**, **Bayrich**, **Holo Belt**, **Loyicn**.
  - *Taş Baskı & Ekipman:* **Guangzhou Disen** (`disenprinter.com`), **Guangzhou Dashanming**.
- **Türkiye:** İstanbul (İkitelli / Güngören / Başakşehir / Merter) merkezli CNC, taş kalıbı lazer ve konveyör bant firmaları mevcuttur; ancak Türkiye stoklu ithal makinelerde genellikle Çin FOB üzerine **%20–40** bayi marjı bulunur, ayrıca Mısır'a tekrar ihracat gümrük maliyeti doğar. Yedek parça, uç ve taş dizim yazılımı/eğitim desteği için avantajlıdır.

---

## 5. Van Yatırım & Uygulama Senaryoları (Karar Desteği)

| Senaryo | Kime Uygun? | Tahmini Bütçe | Teslim Süresi | Kârlılık / Risk Özeti |
| :--- | :--- | :--- | :--- | :--- |
| **Kötü / Düşük Riskli Test (Ön Adım)** | Hemen satın alma yapmadan kalıp malzemesini ve kalitesini sınamak için | **~0 – 15.000 EGP** *(fason numune kesimi)* | **2 – 5 gün** | Mevcut banttan 1 m² parça Kahire'de yerel CNC atölyesinde (ve PVC değilse lazerde) deldirilir. Taşların oturma açısı ve hız görülür; **yanlış makine alma riskini sıfırlar.** |
| **Orta Senaryo (Mısır Yerel Vakumlu CNC Router)** | Mevcut bantlar **PVC** ise veya PVC + PU + sert şablon hepsini işlemek istenirse | **200.000 – 480.000+ EGP** *(~3.700–8.900 USD; taksit imkânı var)* | **1 – 3 hafta** *(yerel stok)* | Gümrük beklemesi yok, Obour'a yakın servis, taksit avantajı. Hızı Galvo lazerden düşüktür ama 24.000 RPM + çoklu kafa seçeneğiyle işi çözer; **konik havşa** açabilir. |
| **İyi / Yüksek Hız Senaryosu (160 cm Konveyörlü Galvo CO2 Lazer — RF Tüp)** | Müşteriye **aynı gün / saatler içinde** yeni metraj kalıp çıkarmak ve bant hammaddesini **PU/PET** yapmak istenirse | **$18.000 – $35.000 FOB** *(Mısır teslim tahmini $23.000 – $45.000+)* *(Cam tüplü giriş: $8.000–$15.000 FOB)* | **6 – 10 hafta** *(üretim + deniz yolu + Nafeza/ACID gümrük)* | Dakikada **1.000–3.000+ delik** hızıyla rakipsizdir. **Şart:** PVC bant kesinlikle kullanılmamalı, PU veya PET kalıp rulosu tedarik edilmelidir. |

### Yazılım İhtiyacı
Makine tek başına deseni taş noktalarına çeviremez. Müşteriden gelen görseli/logoyu SS6/SS10/SS16 taş koordinatlarına ve DXF/PLT kesim dosyasına dönüştürmek için **CorelDRAW taş dizim eklentileri (Rhinestone plugins)**, **WinDesign / Richpeace** veya uyumlu CAD-CAM yazılımı (LightBurn / EZCAD / ArtCAM) iş akışına eklenmelidir.

---

## 6. Önerilen Sonraki Adımlar (Sıralı Eylem Planı)

1. **Bant Analizi:** Makinenin üzerindeki yeşil ve siyah bantların **PVC mi yoksa PU/PET mi** olduğunu kesinleştirin; net bant enini (cm) ve toplam çevre uzunluğunu (cm) ölçün.
2. **Yerel Fason Test:** Kahire/Obour çevresinde vakumlu CNC Router (ve PVC değilse CO2 lazer) ile 50x50 cm deneme deliği açtırıp taş dökme/fırçalama testini makinenizde görün.
3. **Bant Ekleme Çözümü:** Delinen bantları kendi fabrikanızda mı ekleyeceksiniz, yoksa Kahire'deki konveyör bant firmalarında fason sıcak ekleme mi yaptıracaksınız netleştirin (kendi fabrikanızda yapacaksanız **Hot Splicing Press** bütçeye dahil edilmelidir).
4. **Teklif Toplama:** CNC yolu için *Simplex Arabia*, *Top Laser*, *CNC Falcon*; Galvo Lazer yolu için (yalnız PU/PET bantta) *Golden Laser*, *MimoWork*, *Han's Yueming* firmalarından proforma teklif alın.

---

## 7. Kaynakça (Kasım 2026)

- **Lazer & CNC Malzeme Güvenliği / PVC Klor Riski:** `gwklaser.com`, `xometry.com`, `darklylabs.com`
- **Galvo & Konveyörlü Geniş En Lazer Sistemleri:** `goldenlasercutter.com`, `mimowork.com`, `hansyueming.com`, `redshiftlaser.com`, `dowinlaser.com`, `ventechmachine.com`
- **Konveyör Bant Delme & Sıcak Ekleme Presleri:** `beltwin.com`, `bayrichbelt.com`, `holobelt.com`, `loyicn.com`, `utuobelt.com`, `machinebeltsdirect.com`
- **Taş Dizim & Kalıp Makinaları:** `disenprinter.com`, `disenmachinery.com`, `apimpex.com`, `made-in-china.com`, `alibaba.com`
- **Mısır Yerel Makine Tedarikçileri & Fiyat Aralıkları:** `simplexarabia.net`, `cncfalcon.com`, `toplaser-eg.com`, `miracle4laser.com`, `dubizzle.com.eg`, `sigmamachines.net`
- **Mısır Kur & Gümrük Mevzuatı (Kasım 2026):** `cbe.org.eg`, `customs.gov.eg`, `nafeza.gov.eg`, `hegazylaw.com`

---

## 8. Hammaddeye Göre Kullanılacak Makina Matrisi

| Kalıp / Bant Hammaddesi | Kullanılacak Doğru Makina | Yasak / Uygunsuz Makina & Sebebi |
| :--- | :--- | :--- |
| **PVC** *(klasik yeşil/siyah konveyör bant veya sert PVC levha)* | **Vakumlu CNC Router** veya **CNC Bant Zımba** | **CO2 / Galvo Lazer YASAK** — Klor / HCl asit gazı çıkarır, lensleri ve rayları çürütür. |
| **PU (Poliüretan) veya PET / Mylar** | **Galvo / Hibrit CO2 Lazer** (en hızlı) veya **Konveyörlü CO2 Lazer** | İnce esnek şeritte bıçaklı plotter zorlanır; CNC Router çalışır ama lazere göre yavaştır. |
| **Kauçuk / Lazer Şablon Kauçuğu / Flock** | **CO2 Lazer** (güçlü duman emişli) · İnce flock'ta **Bıçaklı Plotter** | Kalın kauçuk plotter bıçağını kırar; CNC uçları kauçukta çapak bırakabilir. |
| **Silikon / PTFE (Teflon) Kaplı Bant** | **Vakumlu CNC Router / Mekanik Delme** (PTFE için güvenli) | PTFE lazerde toksik florür dumanı çıkarabilir; saf silikonda güçlü egzostlu CO2 lazer gerekir. |
| **Akrilik / Pleksi / POM (Delrin)** | **CO2 Lazer** veya **Vakumlu CNC Router** (havşalı delik için CNC) | Fiber lazer şeffaf akriliği kesemez. |
| **Bakelit / FR4 Fiberglas / MDF** | **Vakumlu CNC Router** | CO2 lazer bakelit ve epoksiyi kömürleştirir, yoğun zehirli duman üretir. |
| **Alüminyum / Paslanmaz İnce Sac** | **Fiber Lazer Kesim** veya **Metal CNC Freze/Delme** | **CO2 lazer metali kesemez.** |

---

## 9. Doğrulanmış Doğrudan Satış & Ürün Linkleri (Kasım 2026)

### A. Mısır Yerel Satış Sayfaları (Kahire / Obour Yakını — Servis & Taksit)
- **Simplex Arabia — Vakumlu/Standart CNC Router (`SIM-R-S 1325 ES/EV` — PVC, PU, Bakelit, Akrilik):** https://simplexarabia.net/product/standard-router-sim-r-s-1325-es-ev/
- **Top Laser Egypt — CNC Router Modelleri (`TOP-1 1325B` vb.):** https://toplaser-eg.com/%D8%A3%D9%86%D9%88%D8%A7%D8%B9-%D9%85%D8%A7%D9%83%D9%8A%D9%86%D8%A7%D8%AA-%D8%B1%D8%A7%D9%88%D8%AA%D8%B1-%D8%B3%D9%8A-%D8%A3%D9%86-%D8%B3%D9%8A
- **CNC Falcon Egypt — CNC Router Makineleri:** https://cncfalcon.com/en/cnc-machines-cnc-routers-egypt-cnc/cnc/
- **Simplex Arabia — CO2 Lazer (`SIM-L 1325` — Sadece PU/PET/Kauçuk/Akrilik):** https://simplexarabia.net/product/laser-co2-sim-l-1325/
- **Simplex Arabia — Fiber Lazer (Metal Kalıp/Sac İçin):** https://simplexarabia.net/en/product-category/metal-machinery-en/

### B. Çin Üretici & B2B Satış Sayfaları (Geniş En Konveyörlü Sistemler)
- **Galvo + Gantry Hibrit Konveyörlü CO2 Lazer (PU/PET İçin En Hızlı):**
  - Golden Laser (`ZJJG-160100LD`): https://www.goldenlasercutter.com/gantry-galvo-integrated-laser-cutting-marking-machine.html
  - Redshift Laser (`1610G`): https://redshiftlaser.com/galvo-gantry-laser-machine/
- **Konveyörlü Flatbed CO2 Lazer (`1600mm` / `1610` — PU/PET/Kauçuk):**
  - Golden Laser Mars (`MJG-160100LD`): https://www.goldenlasercutter.com/single-double-head-laser-cutting-machine.html
  - Foster Laser (`1610` Çift Kafa): https://www.fosterlaser.com/high-quality-co2-laser-engraving-machine-1610-large-working-area-double-heads-60w-80w-100w-130w-150w-co2-laser-cutting-machines-foster-product/
  - MimoWork (`160` Flatbed/Konveyör): https://m.mimowork.com/our-laser-solutions/flatbed-laser-cutter-1
- **Vakumlu CNC Router & Taş Makinaları / Kalıp İşleme:**
  - AccTek (`1325` Vakumlu CNC Router): https://acctekcnc.com/ar/cnc-router/1325-cnc-router/
  - Disen Machinery (Hotfix Taş & Kalıp Makinaları): https://www.disenprinter.com/china-hotfix-rhinestones-machine/
  - Made-in-China (Taş Makinaları Üreticileri): https://www.made-in-china.com/manufacturers/rhinestone-making-machine.html
  - Made-in-China (CNC Kalıp İşleme Makineleri): https://www.made-in-china.com/manufacturers/cnc-mould-die-engraving-machine.html
  - Alibaba (Yiwu Aiba Taş Şablon & Lazer Mağazası): https://ywaiba.en.alibaba.com/productlist.html
- **CNC Konveyör Bant Delme & Sıcak Ekleme Presleri (PVC/PU Bant İçin):**
  - Beltwin Bant Delme (`1100–3200mm`): https://www.beltwin.com/belt-perforating-machine
  - Bayrich Bant Delme: https://www.bayrichbelt.com/product/belt-perforating-machine.html
  - HoloBelt CNC Bant Delme: https://www.holobelt.com/product/timing-belt-perforating-machine/
  - Beltwin Hava Soğutmalı PU/PVC Ekleme Presi: https://www.beltwin.com/for-pvc-pu-belts/homogeneous-pu-belt-positive-drive-belt-splice-press
  - Beltwin Su Soğutmalı Geniş Ekleme Presi (`PB600-2100`): https://www.beltwin.com/for-pvc-pu-belts/water-cooling-belt-splice-press-stainless-steel-body-pb600-2100

### C. Türkiye Satış & İlan Kanalları
- **Makinecim (Sıfır CNC Router / Makine İlanları):** https://makinecim.com/satilik-yeni-makine-sifir-makina
- **Kaya Grup Lazer (CO2 & Fiber Lazer):** http://www.kayagruplazer.com/tr

---

## 10. Gönderilen Kalıp Fotoğraflarının Teknik Analizi (`E:\ab ayçam\taşlı yapay zeka\kalıp\`)

İncelenen 6 yakın plan fotoğraf (`IMG_20261110_105052` – `105135`) üzerinden kalıp bandının fiziksel yapısı çıkarılmıştır:

- **Katman & Karkas Yapısı:** Tek kat (**1-ply**) beyaz polyester bez dokuma karkaslı, tahmini **~1,0–1,2 mm** kalınlığında ince yeşil endüstriyel konveyör bandıdır (`105123` ve `105135` kenar kesitinde tek kat beyaz polyester elyaf ve lif dokusu net görülmektedir).
- **Yüzey Dokusu:** Üst (taş) yüzü ince mat/kumlu kaplama; alt (rulo) yüzü ise ince elmas/kafes (`fabric-impression`) dokulu yeşil kaplamadır.
- **Ek Yeri Yöntemi:** `105102`, `105109` ve `105131` karelerinde ek yerinin ağır sıcak parmak presi yerine düz alın ek + takviye şerit bant ile kapatıldığı ve ek hattı üzerine de delik açıldığı görülmüştür. Bu durum ilk aşamada pahalı sıcak ekleme presi olmadan da ekleme yapılabildiğini göstermektedir.
- **Delik İçi (`105052` makro):** Delik çeperinde siyah yanık/karbonlaşma görülmemektedir.
- **PVC vs PU Ayrımı:** Hem 1-ply yeşil **PVC** hem 1-ply yeşil **PU** konveyör bantlar dış görünüş ve alt doku olarak birebir aynı şekilde üretildiği için sadece fotoğraftan %100 kesin ayrım yapılamaz. Elinizdeki artık parçadan 10 saniyelik bakır tel alev testiyle (yeşil alev = PVC, sarı alev = klorsuz PU) kesin teyit alınabilir.
- **Stratejik Sonuç:** Mevcut bant PVC çıksa bile yeni ham bant rulolarını **1,0–1,2 mm 1-ply PU (Poliüretan) + polyester bez** olarak temin ederseniz lazer kesime geçebilirsiniz; PVC ile devam edilecekse delik içi polyester ipliklerinin saçaklanmaması için yüksek devirli keskin uçlu **Vakumlu CNC Router** veya mekanik delme gerekir.

---

## 11. Lazer Yolu İçin Seçilen Makineler & Lazer Uyumlu Kalıp Malzemesi Satış Linkleri

### A. Alınabilecek Lazer Makineleri (Doğrulanmış `HTTP 200` Linkler)
- **3,20 Metre Tam En Konveyörlü CO2 Lazerler (Eğer bant eni 320 cm ise):**
  - MimoWork Contour 320 (`3200 mm` konveyörlü): https://www.mimowork.com/contour-laser-cutting-machine-products/
  - Golden Laser (`3200 mm` geniş konveyörlü): https://www.goldenlasercutter.com/product/vision-laser-cutting-machine/
- **En Hızlı Galvo + Gantry Hibrit Konveyörlü CO2 Lazerler (160 cm — 1.000–3.000+ delik/dk):**
  - Golden Laser (`ZJJG-160100LD`): https://www.goldenlasercutter.com/gantry-galvo-integrated-laser-cutting-marking-machine.html
  - Golden Laser CO2 Galvo/Gantry Serileri: https://www.goldenlasercutter.com/co2-laser-machine/
  - Redshift Laser (`1610G`): https://redshiftlaser.com/galvo-gantry-laser-machine/
- **160–180 cm Konveyörlü Flatbed CO2 Lazerler (Daha ekonomik Çin fabrika çözümleri):**
  - Golden Laser Mars (`MJG-160100LD` tek/çift kafa): https://www.goldenlasercutter.com/single-double-head-laser-cutting-machine.html
  - Foster Laser `1610` Çift Kafa: https://www.fosterlaser.com/high-quality-co2-laser-engraving-machine-1610-large-working-area-double-heads-60w-80w-100w-130w-150w-co2-laser-cutting-machines-foster-product/
  - MimoWork `160` Konveyörlü Lazer: https://m.mimowork.com/our-laser-solutions/flatbed-laser-cutter-1
- **Mısır Yerel CO2 Lazer Satıcıları (Kahire/Obour'a yakın servis & taksit):**
  - Simplex Arabia (`SIM-L 1325`): https://simplexarabia.net/product/laser-co2-sim-l-1325/
  - Miracle4Laser (Çift Kafalı CO2 Lazer): https://miracle4laser.com/%D9%85%D8%A7%D9%83%D9%8A%D9%86%D8%A9-%D8%A7%D9%84%D9%84%D9%8A%D8%B2%D8%B1-co2-%D8%AB%D9%86%D8%A7%D8%A6%D9%8A%D8%A9-%D8%A7%D9%84%D8%B1%D8%A3%D8%B3/
  - Top Laser Egypt (CO2 Lazer Kategorisi): https://toplaser-eg.com/en/%D9%85%D8%A7%D9%83%D9%8A%D9%86%D8%A7%D8%AA/non-metallic-sector
  - CNC Falcon Egypt (CO2 Lazer): https://cncfalcon.com/%D9%84%D9%8A%D8%B2%D8%B1-co2/

### B. Lazer Uyumlu Ham Kalıp Malzemeleri (PVC-Free PU Bant & PET/Mylar)
> Siparişte mutlaka **"%100 PVC-free PU (Polyurethane) + polyester bez, 1.0–1.2 mm 1-ply"** şartını yazdırın.
- **Mısır Yerel PU Konveyör Bant Tedarikçileri (Kahire El-Herafeyeen & 10th of Ramadan — Obour'a çok yakın):**
  - Golden Eagle Egypt (`PU Belt`): https://goldeneagle-egypt.com/pu-belt-%D8%B3%D9%8A%D9%88%D8%B1-%D9%86%D8%A7%D9%82%D9%84%D8%A9/
  - Star Belt Egypt (`PU / Teflon`): https://starbelt.com.eg/
  - Techno Belt Egypt (`PU Conveyor Belt`): https://technobelt-eg.com/2024/10/22/pu/
  - Sanam Egypt (`Belt Conveyor`): https://sanam-eg.com/material-handling/belt-conveyor/
- **Çin Üretici & B2B Ham PU Bant / PET-Mylar Rulo Linkleri:**
  - Jarulan Conveyor Belting (`0.8–1.5 mm` PU bant): https://www.jarulanconveyorbelting.com/supplier-4762530-pu-conveyor-belt
  - Xinbex Belting (`1–1.5 mm` yeşil mat PU bant): https://www.xinbexbelting.com/pu-conveyor-belt/weight-of-conveyor-belt.html
  - Made-in-China (`1.0 mm` PU konveyör bant): https://sa.made-in-china.com/video-channel/tgrbelt_bZdGQEjCZAVR_U-10am-S-1-0mm-PU-Conveyor-Belt-for-Food-Industry-Cake-Biscuit-Conveyor-System.html
  - Made-in-China PU Konveyör Bant Kataloğu: https://www.made-in-china.com/products-search/hot-china-products/Pu_Conveyor_Belt.html
  - Alibaba `1 mm` Yeşil PU Bant Arama: https://www.alibaba.com/trade/search?SearchText=1mm+PU+conveyor+belt+green
  - Made-in-China PET / Mylar Rulo Şablon Filmi: https://www.made-in-china.com/products-search/hot-china-products/Mylar_Sheet_Roll.html
  - The Rhinestone World (Parça Şablon İçin Magic Flock Rehberi): https://www.therhinestoneworld.com/what-is-magic-flock

---

## 12. Ölçü Revizyonu: `200 cm × 180 cm` Kalıp Bandına Göre Doğru Lazer Seçimi

Kullanıcının verdiği net kalıp ölçüsüne göre (**eni 200 cm / 2 metre, rulo açıldığında 180 cm** — açık alan **200 × 180 cm** veya biri 200, diğeri 180 cm):

- **KRİTİK ELEME (`1325` ve `1610` Almayın!):**
  - Standart `1325` (`130 × 250 cm`) veya `1610` (`160 × 100 cm`) CO2 lazerlerde kısa kenar **130–160 cm** ile sınırlıdır; iki kenarı da `180 cm` ve `200 cm` olan bant bu makinelere **sığmaz**.
  - Rulo sürmeli `1810` (`180 cm` genişlik) lazer ise ancak **180 cm** kenar rulo geçiş yönü ise ve bant kenar payı kurtarırsa çalışır; **200 cm** kenar içeri giremez.
- **DOĞRU ÖLÇÜ (`200 × 300 cm` / `250 × 400 cm` / `3200 mm`):**
  - **En Rahat Yerel Seçenek (Mısır — Tek Seferde Tam Yatırma):** `CNC Falcon` tarafından üretilen **`200 × 300 cm`** (veya `200 × 400` / `250 × 400 cm`) CO2 lazer: https://cncfalcon.com/%D9%84%D9%8A%D8%B2%D8%B1-co2/ *(alırken köprü iç net açıklığının en az 205–210 cm olduğundan emin olun).*
  - **Konveyörlü Tam Rulo Seçeneği (Çin Fabrika — 320 cm Genişlik):**
    - MimoWork Contour 320 (`3200 mm` konveyörlü): https://www.mimowork.com/contour-laser-cutting-machine-products/
    - Golden Laser (`3200 mm` geniş konveyörlü): https://www.goldenlasercutter.com/product/vision-laser-cutting-machine/
  - **200 cm+ Genişlikte `1,0–1,2 mm` PU Ham Bant Rulosu (Çin Üretici — PVC-Free):**
    - Xinbex Belting (`2000–4000 mm` master en, `0,85–1,5 mm` PU): https://www.xinbexbelting.com/pu-conveyor-belt/white-food-grade-pu-conveyor-belt.html
    - Jarulan Conveyor Belting (`2000–3000 mm` en, yeşil/beyaz PU): https://www.jarulanconveyorbelting.com/supplier-4762530-pu-conveyor-belt
    - Mısır Yerel (10th of Ramadan / El-Herafeyeen): Golden Eagle (`https://goldeneagle-egypt.com/pu-belt-%D8%B3%D9%8A%D9%88%D8%B1-%D9%86%D8%A7%D9%82%D9%84%D8%A9/`), Star Belt (`https://starbelt.com.eg/`), Techno Belt (`https://technobelt-eg.com/2024/10/22/pu/`) — *"200 cm eninde %100 PVC-free PU rulo stokta var mı"* diye teyit edilmelidir.

---

## 13. Birleşim Yeri Yapıştırma Yöntemi ve Malzemeleri

Fotoğraflarınızdaki ek yerinin (`IMG_20261110_105109` ve `105131` makro büyütmeleri) incelenmesi sonucu mevcut sistem ve yeni `PU` bantlar için uygun yöntemler çıkarıldı:

### A. Mevcut Kalıbınızdaki Yöntem
1. İki uç gönyeli kesilip **alın alına (butt joint)** birleştirilmiş.
2. Arkadan **ince beyaz dokuma takviye şeridi** ile bağlanmış.
3. Yan kenarlarda yük altında yırtılmayı önlemek için **cam elyaf takviyeli şeffaf filament bant (`Fiberglass Filament Tape`)** kullanılmış (`IMG_20261110_105131` kenarında dikey cam elyaf iplikleri görünmektedir).

### B. Yeni `PU` Kalıp Bandını Yapıştırmada 3 Yöntem
1. **En Sağlam (Sıcak Kaynak — `TPU Hot-Melt Film` + Sıcak Pres / Fason):**
   - İki uç parmak kesim veya alın/kademeli olarak araya **TPU eriyen film** ve koruyucu **PTFE (Teflon) kaplı bez** konup ~140–170 °C sıcaklık ve basınç altında kaynatılır (veya Mısır'da *Golden Eagle* / *Star Belt* / *El-Oseily*'de fason ekletilir). En yüksek ısı/buhar dayanımını verir.
2. **Atölye İçi Pratik Sıcak Ek (`TPU Film` + PTFE Bez + Kontrollü Sıcak Ütü/Tabanca + Filament Bant):**
   - 2 metrelik büyük pres almadan, arka yüzeye ince bez şerit + **TPU Hot-Melt Film** koyup üzerine PTFE Teflon bez örterek kontrollü ütü/ısı tabancasıyla birleştirme, kenarları da cam elyaf filament bantla kilitleme.
3. **Soğuk Kimyasal Yapıştırma (`2 Bileşenli PU Yapıştırıcı` + MEK/Aseton + Filament Bant):**
   - **Dikkat:** Klasik kauçuk solüsyonu (`SC 2000` vb.) PU bantta **tutmaz** (`lutze-group.com`). Mutlaka **PU/PVC için 2 bileşenli (yapıştırıcı + sertleştirici/hardener) poliüretan yapıştırıcı** kullanılmalı, yüzey öncesinde **MEK veya aseton** ile yağdan arındırılmalıdır.

### C. Doğrulanmış Malzeme & Tedarik Linkleri (`HTTP 200`)
- **Cam Elyaf Takviyeli Filament Bant (Mısır Yerel — Obour / 10th of Ramadan):**
  - Green Stars Tape (`Fiberglass Filament Tape`): https://www.greenstarstape.com/ar/pages/page/1495/%D8%A7%D9%82%D9%88%D9%8A-%D9%88%D8%A7%D9%81%D8%B6%D9%84-%D8%B3%D9%84%D9%88%D8%AA%D9%8A%D8%A8-%D9%85%D8%AF%D8%B9%D9%85-%D8%A8-%D8%A7%D9%84%D9%81%D8%A7%D9%8A%D8%A8%D8%B1-%D8%AC%D9%84%D8%A7%D8%B3-%D8%B3%D9%84%D9%88%D8%AA%D9%8A%D8%A8-%D9%85%D8%B3%D9%84%D8%AD-%D9%86%D8%B3%D9%8A%D8%AC%D9%8A-%D8%B4%D8%A8%D9%83%D9%8A-%D9%88-%D8%B7%D9%88%D9%84%D9%8A.html
  - Bta3Lasq Egypt (Endüstriyel bantlar): https://bta3lasq.com/
- **Mısır Bant Ekleme Hizmeti & Malzemesi:**
  - El-Oseily / Belt Egypt: https://beltegypt.com/ar/
  - Golden Eagle Egypt: https://goldeneagle-egypt.com/%D8%B3%D9%8A%D9%88%D8%B1-%D9%86%D8%A7%D9%82%D9%84%D8%A9-pvc-belt/
- **TPU Hot-Melt Kaynak Filmi & 2K Soğuk PU Yapıştırıcı:**
  - Beltwin Endüstriyel TPU Kaynak Filmi: https://www.beltwin.com/others/industrial-tpu-film-for-industrial-conveyor-belts-hot-splicing-press
  - Leo New Material TPU Hot-Melt Adhesive Film: https://www.leo-newmaterial.com/hot-melt-adhesive-film/tpu-hot-melt-adhesive-a/
  - Lutze 2K PU/PVC Soğuk Yapıştırıcı Çözümleri: https://www.lutze-group.com/conveyor-technology/repair-splicing-solutions
  - Made-in-China Konveyör Bant Yapıştırıcıları: https://www.made-in-china.com/products-search/hot-china-products/Conveyor_Belt_Adhesive.html
- **200 cm+ Bant İçin Sıcak Ekleme Presi (İleri Aşama):**
  - Beltwin `PB600-2100` (`2100 mm` su soğutmalı): https://www.beltwin.com/for-pvc-pu-belts/water-cooling-belt-splice-press-stainless-steel-body-pb600-2100
