# Projeye Özel Öğrenimler ve Mimari Hafıza (`PROJECT.md`)

> **Kapsam:** Katman 3 — AB Ayçam Sosyal Medya ve İçerik Yönetimi (`Kedihane` Yönetiminde)
> **Yönetici Ekosistem:** `c:\Users\dell\.gemini\antigravity\scratch\kedihane` (Tekir Şefliğinde 8 Ajan)
> **İşletme & Sosyal Medya Reposu:** `E:\ab ayçam\AB-Aycam-SosyalMedyaYonetimi` & `E:\ab ayçam\github-guncelleme`
> **Kayıt Tarihi:** 2026-11-07 · **Commit Politikası:** `kullanici-github-desktop` (`sor`)

---

## 1. Otomatik Çift Repo Çalışma Mimarisi (Kedihane -> AB Ayçam)

- **Varsayılan Otomatik Mod:** Bu projede (`Kedihane+AB_Ayçam_Sosyalmedya`) açılan **her yeni sohbette**, kullanıcının tekrar anlatmasına veya `"ekip:"` yazmasına gerek olmaksızın oturum **otomatik olarak `kedihane` reposu yönetiminde (Tekir şefliğinde)** başlar ve **`AB-Aycam-SosyalMedyaYonetimi` reposunu** kullanır.
- **Okuma Sırası (Her Yeni Sohbetin İlk İşi):**
  1. `antigravity_davran-sh` v2.0.0 model ve kota öneri kutusu sunulup `"devam et"` onayı alınır.
  2. Kedihane anayasası (`c:\Users\dell\.gemini\antigravity\scratch\kedihane\GEMINI.md`, `.agents/learnings/PROJECT.md`) ve görevle ilgili `bilgi/` rehberi (fihristten satır aralığıyla) okunur.
  3. AB Ayçam kalıcı hafızası (`E:\ab ayçam\github-guncelleme` ve `E:\ab ayçam\AB-Aycam-SosyalMedyaYonetimi` içindeki `AGENTS.md`, `.agents/learnings/PROJECT.md`, `AB_Aycam_Proje_Context_TAM.md`, `ilerleme.md`, `bekleyen-isler.md`, `ogrenilenler.md`, ilgili `is-akislari/*.md` ve `promptlar/*.md`) okunur.
- **Kayıt ve Gizlilik İzolasyonu:**
  - Yapılan her iş, rapor, ilerleme ve ders hem `E:\ab ayçam\github-guncelleme` hem `E:\ab ayçam\AB-Aycam-SosyalMedyaYonetimi` klasörlerine kaydedilir.
  - Müşteri adları ve mesaj içerikleri yalnızca `.gitignore`'da korunan `yerel-kayitlar/` klasörüne yazılır.
  - `kedihane` reposuna AB Ayçam'a ait hiçbir kişisel/kurumsal bilgi (marka adı, müşteri adı, telefon numarası, adres, `E:\` yolu) **asla yazılmaz**; yalnızca anonimleştirilmiş global teknik yöntemler Minnak Tekir aracılığıyla aktarılabilir.

---

## 2. Proje Kararları, Öğrenimler ve Tuzaklar Kayıt Tablosu

**Kategoriler:** `mimari` · `tuzak` · `komut` · `kutuphane` · `api` · `tercih`

| Tarih | Kategori | Öğrenim / Karar / Tuzak | Bağlam / İlgili Dosya | Durum |
| :--- | :--- | :--- | :--- | :--- |
| 2026-11-07 | mimari | Proje `project-link` ile `antigravity_davran-sh` sistemine bağlandı ve `Kedihane+AB_Ayçam_Sosyalmedya` proje yapılandırmasında `kedihane` + `AB-Aycam-SosyalMedyaYonetimi` git klasörleri kalıcı olarak birleştirildi. | `AGENTS.md`, `REGISTRY.md` | aktif |
| 2026-11-07 | tercih | Her yeni sohbette kullanıcı tekrar açıklamadan ve `"ekip:"` komutu beklemeden otomatik olarak `kedihane` (Tekir) yönetiminde `AB-Aycam-SosyalMedyaYonetimi` reposu kullanılır. | `AGENTS.md`, `GEMINI.md`, `PROJE_INSTRUCTIONS_GUNCEL.md` | aktif |
| 2026-11-07 | mimari | Çoklu sosyal medya yorum/mesajlarında "Paralel Beyin, Sıralı Parmak" mimarisi uygulanır: 5 sütunlu onay tablosu paralel geçici Flash alt ajanlarla hazırlanır; gönderim tek sekmede sıralı (3-5 sn jitter) ve DOM doğrulamalı yapılır. | `is-akislari/meta-mesaj-ve-yorum-cevaplama.md` | aktif |
| 2026-11-03 | tercih | Sosyal medya ön onay ve raporlamalarında 5 sütunlu tablo (`# \| Soru Arapça \| Soru Türkçe \| Hazırlanan Cevap Arapça \| Cevap Türkçe & Eklenti`) ve `{ISIM}` yerine gerçek profil adının canlı yazılması zorunludur. | `ogrenilenler.md`, `PROJE_INSTRUCTIONS_GUNCEL.md` | aktif |
| 2026-11-02 | kural | Messenger'da fiyat/model soranlara yalnızca güncel `E:\ab ayçam\kartela görüntüsü\kartelas 1 - fiyatlı.pdf` (8,01 MiB) gönderilir (`Temp` dizinine kopyalanarak `upload_file` yapılır) ve yalnız `https://wa.me/201066830373` linki kullanılır. Her gönderim DOM üzerinden 3 adımlı doğrulama kapısından geçmeden sonraki kişiye geçilmez. | `ogrenilenler.md`, `PROJE_INSTRUCTIONS_GUNCEL.md` | aktif |
| 2026-11-01 | tuzak | Dikey (`1080x1920`) taş/strass videolarında küçük PiP/split-screen ve FFmpeg tam-sayı `crop` kaydırma titremesi yasaktır; görseller `1:1` piksel oranıyla tam ekran sabit kadrajlanır ve `0.40 sn` yumuşak `fade` geçişi kullanılır. | `ogrenilenler.md` | aktif |
| 2026-11-09 | mimari | Taşlı şal kadın manken promptlarında Downloads örnekleri doğrulaması: 21 başa sarılan (tarha wrap) + 21 omuza dökümlü (shoulder drape açık dalgalı saç), mermer kafe terasları/porselen fincan ve nötr iç mekan kombini taş parıltısını ve mobil netliği maksimize eder. | promptlar/42_tasli_sal_kadin_manken_ozel_promptlari.md | aktif |
| 2026-11-09 | mimari | Premiere Pro Antigravity 8 Lüks Taş Baskı Paketi: Video merkezini (%85+ açık alan) ve kumaş dökümünü kapatmayan minimal yüzen cam kapsüller (üst rozet Y:220-350, lower-third Y:1420-1620); sıfır sim/glitter kuralı; 15 statik PNG, 5 hareketli ProRes 4444 MOV & MP4 animasyon ve Premiere FCP7 XML sekansı. | premiere pro/şablonlar premiere/antigravity 8/, is-akislari/video-tasarim-ve-yazilar.md | aktif |
| 2026-11-09 | mimari | Google Flow (Veo) taşlı şal I2V video prompt mimarisi: 35 görsel için 3 dengeli ağır çekim kamera modu (12 Push-In, 11 Pan, 12 Orbit), abartısız narin model mikro-hareketleri, %100 kumaş/bağlama/taş sadakat kilidi ve Low/Medium-Low hareket şiddeti standardı uygulandı. | promptlar/27_sal_google_flow_video_promptlari.md | aktif |
| 2026-11-10 | tuzak | Meta Business Suite sol listesinde `"Sen: Merhaba ..."` / `"Sen: أهلاً بيك في AB إسطنبول"` otomatik karşılama önizlemesi insan yanıtı değildir; reklam sorularını gizleyebildiği için cevapsız aday gibi açılıp kontrol edilmelidir. PDF yüklemesinde ise üst banner'daki ilgisiz `progressbar` yerine `[role="listitem"] [role="progressbar"]` ve siyah aktif `Gönder` (`rgb(0, 0, 0)`) kontrol edilir. | `is-akislari/meta-mesaj-ve-yorum.md`, `ogrenilenler.md` | aktif |
| 2026-11-10 | kural | `kartelas 1 - fiyatlı.pdf` dosyasının 39 sayfasının tamamında model adları ve EGP fiyatları (`38–75 EGP`) bulunduğu doğrulandığından Messenger cevaplarından *"fiyat sadece WhatsApp'ta verilir"* ibaresi kaldırıldı; artık hem modellerin hem fiyatların ekteki PDF'te olduğu belirtilip detay ve sipariş için `https://wa.me/201066830373` verilir. | `AGENTS.md`, `is-akislari/meta-mesaj-ve-yorum.md`, `ogrenilenler.md` | aktif |
| 2026-11-10 | kural | Premiere Pro şablonlarında (PNG, MOV/MP4, bitiş kartları) WhatsApp **link (`wa.me`) olarak konulmaz**, açık numara (`01066830373`) ve şirket fabrika adresi (`مصنع إيه بي أيشام — العبور – القليوبية – المنطقة الصناعية بي آند سي – قطعة 7 – بلوك 27003 – الدور الثالث`) zorunlu olarak eklenir; video şablonlarında *"الأسعار عبر واتساب فقط"* yazılmaz. | `AGENTS.md`, `is-akislari/video-tasarim-ve-yazilar.md`, `ogrenilenler.md` | aktif |
| 2026-11-10 | mimari | Telefon numarası ve şirket adresi yasağı **yalnızca `kedihane` reposu içindir**; AB Ayçam reposunda şirket numarası ve adresi yazılmasında hiçbir kısıt yoktur (yalnızca bireysel müşteri adları ve mesajları `.gitignore` altındaki `yerel-kayitlar/` klasöründe tutulur). | `AGENTS.md`, `GEMINI.md`, `AB_Aycam_Proje_Context_TAM.md` | aktif |
