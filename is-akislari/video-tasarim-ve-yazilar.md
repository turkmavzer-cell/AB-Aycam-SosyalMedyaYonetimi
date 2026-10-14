# İş akışı: Video tasarımları, yazı katmanları ve Facebook açıklaması

Son güncelleme: 13.10.2026

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

## Denenenler
- Sunucuda ses→metin modeli indirilemedi (ağ 403); bu videoda gerek olmadı (sadece müzik).
