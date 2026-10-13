# İş akışı: Meta Business Suite mesaj ve yorum cevaplama

Son güncelleme: 13.10.2026

## Amaç
Facebook sayfası "AB İstanbul dijital & Taş baskı" için Messenger mesajlarını ve gönderi yorumlarını takip etmek, müşterilere Arapça (Mısır lehçesi) cevap yazmak ve WhatsApp'a yönlendirmek.

## Ne zaman
Kullanıcı "yeni mesaj ve yorumları kontrol et" dediğinde.

## Adım adım
1. Claude in Chrome ile Meta Business Suite gelen kutusunu aç (kullanıcının giriş yaptığı Chrome; yeni sekmede çalış).
   - Tüm mesajlar: `https://business.facebook.com/latest/inbox/all?asset_id=<sayfa asset id>`
   - Messenger: `.../latest/inbox/messenger?asset_id=...`
   - Facebook yorumları: `.../latest/inbox/facebook?asset_id=...`; bir gönderi için `&selected_item_id=<gönderi id>&thread_type=FB_PAGE_POST`
   - Sayfa yüklenirken boş görünebilir, 5-8 sn bekle.
2. Okunmamış sayıları ve "Okunmamış" filtresini kullan. Listeyi aşağı kaydırıp daha eski konuşmaları yükle. Son mesajın "Sen:" ile başlaması bizim cevap verdiğimiz anlamına gelir; müşterinin yazdığı son mesajlar cevap bekleyenlerdir.
3. Yorumlarda her gönderiyi aç; altında "1 yanıtı gör" yazan yorumların cevabı var mı genişleterek doğrula (tıklama yeri yorum altındaki bu yazı). Sayfa adı üzerine gelince açılan profil kartını X ile kapat.
4. **Listeyi Türkçe tablo olarak çıkar:** kim yazmış, ne yazmış, yazılacak cevap. Müşteri adı sadece sohbette gösterilir, repoya yazılmaz.
5. Kullanıcı onayı sonrası cevapları yaz (kullanıcı "hepsine cevap ver" demeden gönderme).
6. Messenger gönderirken: konuşmayı aç, yanıt kutusuna tıkla (konumu sayfaya göre değişir; yazı yazmadan önce ekran görüntüsüyle doğrula), Arapça metni yaz, Enter. Önerilen yanıt kutusu bazen yanıt alanına metin yazabilir; gerekirse ctrl+a + Delete ile temizle.
7. Yorum yanıtı: yorumun altındaki "Yanıtla"ya tıkla, yaz, Enter.
8. **Meta'nın "otomatik özel mesaj" penceresi** çıkarsa her zaman **İptal**'e bas, Kaydet'e basma.
9. Kendi yorum cevabını düzeltmek için: üzerine gel → "..." → Düzenle → ctrl+a → yeni metin → Return. (Gönderilmiş Messenger mesajı düzenlenemez.)
10. Her gönderimden sonra ekran görüntüsüyle gönderildiğini doğrula.

## Kurallar
- Cevaplar Arapça (Mısır lehçesi), kişinin adıyla hitap (Arapça yazan için Arapça isim, Latin yazanın adı olduğu gibi).
- WhatsApp'a yönlendirirken **sadece `https://wa.me/201066830373` linki**. Telefon numarası yazı olarak yazılmaz (Arapça metinde sıra ters görünür).
- **Fiyat ve model çeşitliliği sadece WhatsApp'tan verilir.** Cevapta açıkça söylenir. İnsanlar Messenger'dan cevap aldıktan sonra da fiyat/model sorduğu için bu vurgu eklendi.
- Yorumda otomatik özel mesaj numarayı zaten gönderiyorsa ayrıca cevap yazma.
- Spam ve ilgisiz reklamlar atlanır.
- Reklam seti ve otomasyon değişiklikleri sadece onayla.
- Şifre/doğrulama kodu girilmez.

## Cevap şablonları ({ISIM} yerine kişinin adı)
**Fiyat sorusu:**
أهلاً {ISIM} 👋 سعر المتر بيختلف حسب الرسمة والقماش. للسعر والتفاصيل كلمنا على واتساب: https://wa.me/201066830373

**Şekiller/modeller sorusu:**
أهلاً {ISIM} 👋 عندنا أكتر من 37 رسمة مختلفة للطباعة. لمشاهدة الأشكال المتاحة وإرسال قماشك كلمنا على واتساب: https://wa.me/201066830373

**Fiyat ve model yalnızca WhatsApp'ta (tekrar soranlara; güncel kural):**
أهلاً {ISIM} 👋 الأسعار والموديلات بنشاركها على واتساب بس. كلمنا هناك وهنرد عليك فوراً: https://wa.me/201066830373

**Sipariş isteği:**
أهلاً {ISIM} 👋 الأسعار والموديلات بنشاركها على واتساب بس، وتقدر تطلب طباعة على قماشك من هناك. كلمنا وهنرد عليك فوراً: https://wa.me/201066830373

**Kargo / teslimat sorusu (13.10.2026'da kullanıldı; gerçek politika kayıtta yok, kullanıcı teyit edince güncellenecek):**
أهلاً {ISIM} 👋 تفاصيل الشحن والتوصيل بنشاركها على واتساب بس. كلمنا هناك وهنرد عليك فوراً: https://wa.me/201066830373

**Teşekkür (olumlu yorum):**
شكراً لذوقك! للتفاصيل والسعر كلمنا على واتساب: https://wa.me/201066830373

## Denenen ve olmayanlar
- Cevaba telefon numarasını yazı olarak koymak: kullanıcının ekranında numara sırası ters göründü. Sadece link bırakıldı. Eski cevaplarda yazılı numaralar vardı; yorumlarda Düzenle ile düzeltildi, Messenger mesajları düzenlenemediği için bekliyor.
- Meta'nın otomatik karşılama mesajı sadece "nasıl yardım edebiliriz" der; fiyat/link içermez, bu yüzden ayrıca cevap gerekir.

## Mevcut durum
13 Ekim: 7 yeni Messenger mesajı cevaplandı (sadece ismini yazıp beğeni atan bir kişi atlandı). Yorumlarda Meta otomatik yanıtı çalışıyor. Messenger'da yanıt kutusu konumu pencere boyutuna göre değişir (y≈677 veya 722); yazmadan önce ekran görüntüsüyle kutuyu doğrula. Gönderilen konuşma listenin en üstüne çıkar, alttakiler kaymaz.
12 Ekim: bekleyen tüm Messenger mesajları cevaplandı; tekrar soran yoktu. Eski mesajlar ve bazı yorumlar için `bekleyen-isler.md` dosyasına bak.
