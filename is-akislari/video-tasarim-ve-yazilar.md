# İş akışı: Video tasarımları, yazı katmanları ve Facebook açıklaması

Son güncelleme: 24.10.2026

## Amaç
Premiere'de hazırlanan dikey videolara (Facebook/Reels) şeffaf PNG tasarım katmanları, zamanlı Arapça yazılar, iletişim kartı ve 4 fotoğraflı bitiş sahnesi eklemek.

## Teknik ayarlar
- Kullanıcının sequence'i: 2160x3840 (9:16), 59,94 fps, ProRes 422 LT önizleme. Klip kaynakları 1080x1920 olabilir.
- Export: tek yüksek kaliteli master, H.264 MP4, VBR 2 geçiş 60-80 Mbps (max 100), High profile Level 5.2, AAC 320 kbps 48 kHz. Facebook zaten yeniden sıkıştırır; ayrı Facebook export'u şart değil. Dosya 4 GB'ı aşarsa bitrate 50 Mbps'ye indirilir.
- Facebook Reels (Meta API): min 540x960, 24-60 fps, 3-90 sn, H.264/H.265, AAC 48 kHz stereo.

## Üretilen tasarımlar (kaynak: `video-tasarimlari/_kaynak/design4k.py <ölçek>`)
`E:\ab ayçam\video-tasarimlari\2160x3840\` (1080x1920 klasörü eski sürüm): 01 iletişim kartı (şeffaf), 02 koyu zeminli kart, 03 alt başlık bandı, 04 köşe çerçeve + gradyan, 05 WhatsApp butonu, 06 rozetler (جودة تركية, أكثر من 37 رسمة, بدون استيراد, تنفيذ سريع), 07 4 foto ızgara şablonu, 08-09 parıltı, 10 yuvarlak köşeli foto üst katmanı.
- Palet: siyah, kırmızı #D7141D, gümüş, beyaz. Font: Cairo (npm @fontsource/cairo woff'tan ttf'ye çevrilir; sunucu geçici klasörü sıfırlanırsa `_kaynak` yedeğinden alınır).
- Arapça metin: Pillow + raqm, kelime kelime sağdan sola dizilim; Arapça font Arapça kelimeler için, Latin font sayı/Latin için. `…` karakteri fontta yok, Arapça virgül (،) kullanılır.

## 4 fotoğraflı bitiş
Üst katman PNG (10) en üst kanala, 4 fotoğraf altındaki kanallara. Yuva merkezleri (2160x3840): (560,1360) (1600,1360) (560,2720) (1600,2720); yuva 960x1280 (3:4). Fotoğraf yuvayı doldurmalı (Scale). Yuvarlak köşeyi katman delikleri sağlar, Premiere'de köşe yuvarlatma efekti yok.

## Yazı katmanları
`E:\ab ayçam\video-yazilari\2160x3840` ve `1080x1920`: 15 şeffaf PNG, ad = sıra + saniye aralığı (örn. `03_8s5-12s5sn.png`). Tam ekran boyutlu, konum ayarı gerekmez. Yazılar alt-orta (y≈1330), 14 numara ızgara altında, 15 numara kart altında.
Metinler: طباعة الاستراس بالمتر / على التوب كامل، مش قطع / لمعة مختلفة في كل متر / أكتر من 37 رسمة تختار منها / ثبات وجودة تركية / بنطبع على القماش اللي تختاره / تنفيذ سريع من غير استيراد / إنت اختار القماش، وإحنا علينا الباقي / كل الألوان وكل الأقمشة / تفاصيل دقيقة تلفت الأنظار / مناسب للمصانع وورش الملابس / عبايات · لانجيري · سواريه · ملابس حريمي / شوف شغلنا / كل قطعة بلمسة استراس / كلمنا على واتساب.

## Video 17T (örnek)
"17T video Reklam - Facebook - mini.mp4" (1080x1920, 80,5 sn, sadece müzik): 0-36 sn kırmızı kumaş, 36-60 sn yeşil kumaş (kesimler 36,0 ve 40,5), ~61-73 sn dört fotoğraflı ızgara (fotoğraflar ~65, 67, 69, 71'de değişir), ~74-80 sn iletişim kartı. Zamanlar `17T_yazilar.srt` içinde; yazı sırası/zamanı yukarıdaki PNG adlarıyla aynı.

## Bayraklı bitiş (14.10.2026)
**Kural: bayrakları Claude çizmez; kullanıcı kendi bayrak görsellerini koyar.** (Claude'un çizdiği Mısır kartalı kötü göründü, kullanıcı reddetti; dosyalar silindi.)
`E:\ab ayçam\video-tasarimlari\bayrak-sablon\2160x3840` ve `1080x1920`: 01 şeffaf (koyu vinyet), 02 koyu zeminli. İki daire deliği olan üst katman: altın çerçeveli, hafif parlama; Türk bayrağı solda, Mısır sağda; ortada kırmızı elmas, altında "جودة تركية داخل مصر" ve AB AYÇAM. Bayrak görselleri altındaki kanala konur. Delik merkezleri (2160x3840): sol (570,1760), sağ (1590,1760); çap 760 px (1080x1920'de 285,880 / 795,880, çap 380). Bayrak görseli deliği tamamen kaplayacak kadar büyütülür. Betik `_kaynak\bayrak.py <ölçek>` (design4k.py'ye bağlı).

## Facebook açıklama kuralları
Arapça (Mısır lehçesi), fiyat yok, WhatsApp için sadece `https://wa.me/201066830373` linki (yazılı numara yok), adres satırı ve etiketler dahil (#طباعة_استراس #استراس #طباعة_بالمتر #هوت_فيكس #لانجيري #عبايات #فساتين_سهرة #العبور #مصر #ABAYÇAM). Metin: başlıkta "طباعة الاستراس بالمتر… على التوب كامل، مش قطع", ✔️ listesi (37 رسمة, ثبات وجودة تركية, القماش اللي تختاره, تنفيذ سريع من غير استيراد, مناسب للمصانع وورش الملابس), "الأسعار والموديلات بنشاركها على واتساب بس".

## Video 18 - reklam (19.10.2026)
- Yöntem: `.prproj` dosyası gzip'li XML; python ile okunup sequence'teki klip adları, başlangıç/bitiş (tick/254016000000 = sn) ve in-point'ler çıkarıldı. Her klibin ortasından ffmpeg ile kare alınıp kontak sayfası yapıldı; yazılar görüntüye göre zamanlandı. Premiere projesi kullanıcıda açıkken de okunabiliyor, değiştirilmiyor.
- Çıktı klasörü: `premiere pro\18 - reklam video\yazi-ve-bitis-sablonlari\` (2160x3840, 1080x1920, SRT, OKU-BENI.md, `_kaynak` betik+font+logo yedeği). Yazılar sequence zamanıyla adlandırıldı.
- Yeni kural (kullanıcı): bitiş kartında SADECE 0373 ile biten WhatsApp numarası olur, diğer numaralar konmaz. Yeni şablon: ücretsiz numune ("getireceğiniz numuneye ücretsiz taş baskı yapılır") — metin: عرض خاص / أي عينة تجيبها بنطبع لك عليها استراس مجاناً.
- Teknik ders: Arapça cümlede Latin/rakam kelimeleri (AB AYÇAM, +20 106 683 0373) kelime kelime sağdan sola dizilince ters çıkıyor; ardışık Latin/rakam kelimeleri tek soldan-sağa blok olarak yazılmalı. `video-tasarimlari`/`video-yazilari` klasörleri ve eski betik bu tarihte bulunamadı; betik yeniden yazıldı ve artık `_kaynak` içinde.

- Video 18'de eklenenler: açılış kartı (`00_baslangic_*`) ve 2 fotoğraflı bitiş katmanı (`16_ikili_foto_ust_katman.png`): yuvalar 960x1280, merkezler (560,1900) ve (1600,1900) (2160x3840), kırmızı çerçeveli, üstte شوف شغلنا. 4'lü şablonun 2'li uyarlaması; yöntem aynı (üst katman delikli, fotoğraflar altta).

- Video 18: 2'li yerine 4'lü seçildi (`17_dortlu_foto_ust_katman.png`, merkezler (560,1360) (1600,1360) (560,2720) (1600,2720), yuva 960x1280); 2'li (`16_...`) yedekte. Kullanıcı bitiş fotoğraf sahnesinde 4'lüyü tercih ediyor.

## Denenenler
- Sunucuda ses→metin modeli indirilemedi (ağ 403); bu videoda gerek olmadı (sadece müzik).

## Video 19 - sim (glitter) numune kurgusu (19.10.2026)
- Kaynak: `premiere pro\19 - sim\sim numuneleri\` 9 video (dikey 4K HEVC, 60 fps, toplam ~5 dk). `VID_20261019_031416` tamamen siyah → kullanılmadı. Kumaşlar: kırmızı (172716), ahududu (172840, 172917, 172938 yakın çekim, yeşil yıldız), gri-bej (173153, 83 sn), zeytin (173352, 173432), siyah (173534).
- Üretim (`_calisma\`): `cut.sh` (kesit → 1080x1920/30 fps, eq contrast 1.04 sat 1.08), `sim_gen.py` (Video 18 `gen.py` yardımcılarını exec ederek başlık/etiket/logo/bitiş kartı PNG'leri), `passA.py` (9 kesit + bitiş kartı xfade 0,35 sn / fadeblack 0,5 sn, 916 kare), `passB.py 0|1|2` (yazılar 3 parçada; parça sınırları 360 ve 608. kare), concat + sessiz AAC.
- Akış (sn): 0-3,5 siyah açılış (yavaş çekim 0,5x) → kırmızı → ahududu → yakın yıldız → zeytin (2) → gri → siyah (2) → bitiş kartı 25,7-30,5. Etiket: أحمر / عنابي / زيتي / رمادي فاتح / أسود; alt yazılar ve zamanları `sim_kurgu_v1_yazilar.srt`.
- Bitiş kartı: logo, AB AYÇAM, "طباعة الجليتر بالمتر", sadece +20 106 683 0373, adres, "ابعت لنا القماش بتاعك" (Video 18 kuralı).
- Ses yok (müzik sonra); Facebook açıklaması: `premiere pro\19 - sim\sim_kurgu_v1_facebook_aciklama.txt`.
- Gemini referans kareleri `premiere pro\19 - sim\gemini-referans-kareler\`; promptlar `promptlar\GEMINI PROMPTLARI v15 - ...md`.


## Video 19 (sim) — şablonlar ve v15 notu (19.10.2026)
- Şablon klasörü: `premiere pro\19 - sim\sablonlar-video-19\` (2160x3840 + 1080x1920). Üst katman PNG'leri tam kadraj, fotoğraf yuvaları şeffaf; fotoğraflar alt kata konur. Üreten betik: `_kaynak\tmpl_gen.py` (gen18.py üzerine).
- **Reddedilen:** v15 şal promptları — simler öbek/desen gibi çıktı (serpme olmalı). Yerine v16.

## Video 19 (sim) v2 — devam (20.10.2026)
- Bitiş bölümü kalıbı: 5 dörtlü (2,6 sn, 0,35 sn arayla sırayla belirme) + 3 tek (yuvarlak çerçeve/tam kadraj, hafif zoom, 1,6-1,8 sn) + 4,5 sn bitiş kartı. Renge göre gruplama: kırmızı, ahududu/bordo, gri-bej, siyah/koyu, akşam sıcak tonlar.
- Yazı zamanları klip sınırlarına göre: 0,4-4,4 başlık; renk etiketi klibin ilk 0,3 sn'sinden; ikinci yazı klipten ~0,4 sn sonra.

## Video 21 - geniş kumaş (24.10.2026)
- Kaynak proje: `premiere pro\21 - geniş kumaş\video 21 video.prproj` (sekans: `VID_20261015_152528`, 2160x3840, ~81,1 sn görüntü + 84,6 sn müzik). Açık projeye dokunulmadı, sadece okundu.
- Sekans yapısı: 0–56,32 sn arası 12 geniş kumaş taş/strass baskı klibi (0–2,74 sn V2'de açılış logosu, 2,74–56,32 sn V3'te sağ üst yarı şeffaf logo), 56,32–68,91 sn 4'lü fotoğraf ızgarası (3 grup x 4 foto + `10_foto_ust_katman_yuvarlak_kose.png`), 68,91–75,57 sn bayrak şablonu (`Nested Sequence 01`), 75,57–81,09+ sn bitiş alanı.
- Çıktı klasörü: `premiere pro\21 - geniş kumaş\yazi-ve-bitis-sablonlari\` (`2160x3840\`, `1080x1920\`, `21_genis_kumas_yazilar.srt`, `OKU-BENI.md`, `_kaynak\gen21.py` + `fontlar\` + `logo.png`).
- **3.20 mt en vurgusu (kullanıcı isteği):** 02 (`5,7–9,3 sn`), 04 (`14,8–18,2 sn`) ve 09 (`35,5–40,1 sn`) numaralı kliplerin şablonları ile açılış/bitiş kartlarına **"3.20 mt eninde kumaşlara da baskı yapılabildiği"** (`بنطبع على القماش العريض لحد عرض 3.20 متر`, `حتى الأقمشة بعرض 3.20 متر بنطبع عليها`, `طباعة لحد عرض 3.20 متر بالمتر / مناسب للمصانع وورش الملابس والمفروشات`) eklendi; ayrıca istenen her yere konabilecek 2 bağımsız şablon (`21_ek_320_metre_en_alt_bant_seffaf.png`, `22_ek_320_metre_en_rozetli_alt_bant_seffaf.png`) üretildi.
- Videonun sonu için (`75,6–81,1+ sn`) Mısır Amme Arapçası ile "numuneler ücretsiz baskısı yapılır" (`عرض خاص / طباعة العينات مجاناً / أي عينة تجيبها بنطبع لك عليها استراس مجاناً / جرّب شغلنا على قماشك من غير أي تكلفة`) şablonunun 5 varyantı üretildi: şeffaf orta kart (`14`), koyu zeminli tam ekran kart (`15`), alt yazı bandı (`16`), ücretsiz numune + iletişim (sadece 0373) birleşik bitiş kartı şeffaf/koyu (`17`/`18`), standart iletişim kartı şeffaf/koyu (`19`/`20`).
- Ayrıca V2'deki açılış logosu `19 - sim` klasöründen (`طباعة الجليتر بالمتر`) kalmış olduğu için taş baskı karşılığı (`00_acilis_0s0-2s7sn_logo_strass_seffaf.png`: `طباعة الاستراس بالمتر / على القماش العريض لحد عرض 3.20 متر`) eklendi.

## Video 22 - desenler (24.10.2026)
- Kaynak: `E:\ab ayçam\premiere pro\22 - desenler\videolar` içindeki 35 WhatsApp desen videosu incelendi; tekrar edenler elenip en net ve farklı 14 desen/üretim klibi seçildi.
- Müzik ve ritim senkronu: `Amr Diab & Orange - Lola El Banat` (`48,50 sn`'den başlatıldı; `5,70 sn`'de nakarat ritim patlaması ile ana desen geçişleri başlıyor; tüm kesimler `122.5 BPM` — 8 vuruş `3,92 sn` ve 6 vuruş `3,00 sn` — müzik ritmine kilitlendi).
- Görsel iyileştirme ve efektler: WhatsApp videolarına LANCZOS ölçekleme, taş parlamasını belirginleştiren `unsharp` filtreleme, kontrast/doygunluk (`contrast=1.06, saturation=1.12`), dinamik yumuşak kamera pan/zoom hareketi, her vuruş kesiminde hafif parlama (beat-flash) ve ritmik geçişler (`fadewhite`, `slideleft`, `slideright`, `circleopen`, `wipeleft`, `slidedown`, `fadeblack`) uygulandı.
- 4 Ana Vurgu (Mısır Amme Arapçası):
  1. **40 farklı model:** `عندنا أكتر من 40 موديل ورسمة` / `40 موديل مختلف على أي خامة وأي لون` (üst rozet: `40+ موديل`).
  2. **3.20 mt eninde baskı:** `بنطبع لحد عرض 3.20 متر` / `حتى الأقمشة العريضة بنطبع عليها بفرش كامل` (üst rozet: `عرض 3.20 متر`).
  3. **Mısır'da bir Türk fabrikası:** `إحنا مصنع تركي في مصر` / `إحنا أتراك في مصر · جودة وخبرة تركية` / `مصنع تركي على أرض مصر` (üst rozet: `جودة تركية في مصر` + kullanıcının `images.png` ve `images (1).png` bayrak görselleriyle hazırlanan Türk-Mısır bayrak sahnesi).
  4. **Ücretsiz numune baskısı:** `طباعة العينات مجاناً قبل ما تبدأ شغلك` / `أي عينة تجيبها بنطبع لك عليها استراس ببلاش` (üst rozet: `العينات مجاناً` + özel ücretsiz numune kartı + birleşik bitiş iletişim kartı).
- Çıktılar:
  - Hazır kurgu videosu: `E:\ab ayçam\premiere pro\22 - desenler\video 22 - 1.mp4` (`1080x1920`, 30 fps, `75,5 sn`, H.264 + AAC 256 kbps).
  - Premiere Pro 4K XML sekansı: `E:\ab ayçam\premiere pro\22 - desenler\video22_premiere_sekans.xml` (`2160x3840`).
  - Şablonlar ve kaynak betikler: `E:\ab ayçam\premiere pro\22 - desenler\yazi-ve-bitis-sablonlari\` (`2160x3840\`, `1080x1920\`, `22_desenler_yazilar.srt`, `OKU-BENI.md`, `_kaynak\gen22.py`) ve `_calisma\build_video22.py`, `_calisma\mkxml22.py`.
