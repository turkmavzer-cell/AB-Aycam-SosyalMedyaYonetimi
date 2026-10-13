# İlerleme kaydı

Son güncelleme: 13.10.2026. En yeni kayıt en üstte.

## 13 Ekim 2026
- Video yazı tasarımları: `E:\ab ayçam\video-yazilari\` (2160x3840 ve 1080x1920, 15 şeffaf PNG, ad = sıra + saniye aralığı). "17T video Reklam - Facebook - mini.mp4" için Arapça yazı planı, `17T_yazilar.srt` ve Facebook açıklaması (Arapça, fiyatsız, sadece wa.me linki) yazıldı. Ayrıntı: `is-akislari/video-tasarim-ve-yazilar.md`.
- Facebook kontrolü (öğleden sonra): 2 Messenger mesajı cevaplandı (fotoğraf isteği ve model sorusu; ikisi de wa.me linkiyle WhatsApp'a yönlendirildi). Sadece emoji atan bir kişi ve Meta otomatik yanıtı almış yorumlar cevapsız bırakıldı.
- Yuvarlak köşeli foto üst katmanı üretildi (`10_foto_ust_katman_yuvarlak_kose.png`): fotoğrafların üstüne konur, delikler köşeleri keser. Yuva merkezleri (2160x3840 sequence): (560,1360) (1600,1360) (560,2720) (1600,2720). Yuva 960x1280 px. (Önceki 1080 koordinatlı Position önerisi geçersiz.)
- Kullanıcının Premiere sequence ayarı: 2160x3840 (9:16), 59,94 fps, ProRes 422 LT önizleme. Tasarım PNG'leri 4K olarak yeniden üretildi (`video-tasarimlari\2160x3840\`, eskiler `1080x1920\`'de). Betik `_kaynak\design4k.py <ölçek>`. Export kararı: tek yüksek kaliteli H.264 master (VBR 2 geçiş 60-80 Mbps, AAC 320). Facebook Reels için Meta API: min 540x960, 24-60 fps, 3-90 sn, H.264/H.265, AAC 48 kHz stereo (4K Reels üst sınırı doğrulanamadı).
- Video bitiş/tasarım paketi: iletişim kartı (şeffaf + koyu zeminli; WhatsApp +20 106 683 0373, +20 106 895 6909, +90 532 058 8023, adres), alt başlık bandı, köşe çerçeve + gradyan, WhatsApp butonu, 4 rozet, 4 foto ızgara şablonu, parıltı katmanı. Palet: siyah, kırmızı #D7141D, gümüş, beyaz. Font Cairo (npm @fontsource/cairo'dan çevrildi).
- Facebook kontrolü (sabah): 7 Messenger mesajı (fiyat, model, kumaşa baskı, kargo sorusu) wa.me linkli cevaplarla yanıtlandı. Kargo sorusuna WhatsApp'a yönlendiren şablon kullanıldı (gerçek kargo politikası kayıtta yok). El Badry'nin strass satış ilanı yorumu cevapsız bırakıldı.
- GitHub'a ilk yükleme yapıldı: kök dosyalar, is-akislari, promptlar, promptlar/arsiv-gemini-giydirme (13). Repo özel. Eski video işleri aktarılmadı (kullanıcı kararı: bundan sonrası kayıt altına alınacak).
- GitHub kayıt sistemi kuruldu: her işte ilgili md güncellenir, onaylı promptlar `promptlar/` klasörüne yazılır.
- Proje Context dosyası güncellendi; Proje Instructions'a, yeni sohbetin repoyu okumasını söyleyen metin hazırlandı. `GITHUB AKTARIM TALIMATI.md` hazırlandı.
- Ses→metin: faster-whisper kurulu, model indirilemedi (ağ 403). Model dosyası kullanıcı koyarsa kullanılabilir.

## 12 Ekim 2026
- Ev tekstili çiçek seti: Mısır pazarı için 3 konsept denendi. Ramazan iftar sofrası (koyu) beğenildi, Nil terası beğenilmedi, **ev içi doğal Mısır konsepti onaylandı** (promptlar/ev-tekstili-cicek-sahne-dogal-misir-onayli.md). Küçük parçaların büyük çizilmesi sorunu orana vurguyla çözüldü.
- 3 detay çekimi promptu yazıldı (tabak altlığı, merkez desen, makro köşe).
- Facebook cevap kuralı güncellendi: fiyat ve model bilgisi sadece WhatsApp'tan verilir. Messenger'da 2 bekleyen müşteriye bu cevap gönderildi; tekrar soran yoktu.
- TikTok şirket hesabı tespit edildi (@toqa7808), erişim kurtarma adımları çıkarıldı. Giriş yapılmış hesap kişisel hesaptı; TikTok yorum akışı hesaba giriş sonrası konuşulacak.
- Facebook: 6 bekleyen Messenger mesajına ve fiyat soran yorumlara cevap verildi (wa.me linkiyle). Yorumlardaki cevaplar "1 yanıtı gör" açılarak doğrulandı.

## 11 Ekim 2026
- Ev tekstili kar seti için üstten kolaj denemeleri (v13 reddedildi, v14 aynı görseli üretti), kullanıcı konsept yerine model başına prompt istedi.
- Yerleşim netleşti: uzun masada büyük parça ortada çapraz, küçükler uçlarda düz, uzun parça boş alanda.
- Meta Business Suite: yeni mesaj/yorum listesi ve cevaplar; yorumlardaki yazılı numaralar düzeltilmeye başlandı (bkz. bekleyen-isler.md).

## 8 Ekim 2026 ve öncesi
- Taşlı yapay zeka giydirme promptları v2–v12, 6 seslendirmeli video, Premiere işleri, paisley vektör, Facebook metinleri. Ayrıntı: `AB_Aycam_Proje_Context_TAM.md`.
