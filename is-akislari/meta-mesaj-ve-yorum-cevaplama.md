# İş akışı: Meta Business Suite mesaj ve yorum cevaplama

Son güncelleme: 11.11.2026

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
2. Okunmamış sayıları ve "Okunmamış" filtresini kullan. Listeyi aşağı kaydırıp daha eski konuşmaları yükle. Son mesajın "Sen:" ile başlaması genellikle bizim cevap verdiğimiz anlamına gelir; **ancak `"Sen: Merhaba ..."` veya `"Sen: أهلاً بيك في AB إسطنبول"` önizlemesi Meta'nın otomatik karşılama mesajıdır (insan yanıtı değildir) — müşteri sorusu arkasında kalmış olabileceği için cevapsız aday olarak mutlaka açılıp doğrulanmalıdır.** Müşterinin yazdığı son mesajlar cevap bekleyenlerdir.
3. Yorumlarda her gönderiyi aç; altında "1 yanıtı gör" yazan yorumların cevabı var mı genişleterek doğrula (tıklama yeri yorum altındaki bu yazı). Sayfa adı üzerine gelince açılan profil kartını X ile kapat.
4. **Listeyi 5 Sütunlu Türkçe Tablo Olarak Çıkar (İki Aşamalı Onay & Gerçek Zamanlı İsim Hitabı):**
   - Kullanıcı sormasa dahi veya gelen yorum/mesajlar incelendiğinde her zaman şu 5 sütunlu tam tablo formatında sunulur:
     `| # | Mesajdan/Yorumdan Gelen Soru (Arapça) | Sorunun Türkçe Anlamı | Hazırlanan Cevap (Arapça) | Cevabın Türkçe Anlamı & Eklenti |`
   - **Gerçek Zamanlı İsim Hitabı:** Hazırlanan cevabın hem Arapça metninde hem de Türkçe açıklamasında `{ISIM}` şablon değişkeni yerine doğrudan **mesajı atan veya yorumu yapan müşterinin gerçek profil adı** yazılır.
   - **Katalog Eki Belirteci:** Türkçe sütununda `📎 Ek: kartelas 1 - fiyatlı.pdf` açıkça gösterilir.
   - Müşteri adı sadece sohbette onay için gösterilir, git reposuna yazılmaz (`yerel-kayitlar/` altında tutulur).
5. **Kullanıcı Onayı Olmadan Asla Başlama:** Kullanıcı açıkça *"onayla / gönder / başla"* demeden tek bir mesaj dahi gönderilmez.
6. **Messenger gönderirken (Kişi Başına Tekil Doğrulama Kapısı):**
   - Konuşmayı aç ve sağ paneldeki başlık adının hedef müşteriyle birebir eşleştiğini doğrula.
   - Yanıt kutusuna Arapça metni yaz.
   - PDF gerekiyorsa ataç/dosya yükleme ile `kartelas 1 - fiyatlı.pdf` dosyasını ekle.
   - Yükleme ilerleme çubuğu (progressbar) bitmeden ve Gönder butonu aktif siyah renge (`rgb(0, 0, 0)`) dönmeden tıklama yapma.
   - Gönder'e tıkla.
   - **Tekil Doğrulama Şartı:** Sağ paneldeki mesaj listesinde PDF ekini ve metni gör; sol konuşma listesinde *"Bir dosya eki gönderdin."* (veya iletilen metin) önizlemesini DOM üzerinden kesin olarak doğrula. **Doğrulanmayan hiçbir konuşma geçilemez, başarılı sayılamaz ve bir sonraki müşteriye geçilmez.**
7. Yorum yanıtı: yorumun altındaki "Yanıtla"ya tıkla, yaz, Enter. Gönderildiğini DOM üzerinden doğrula.
8. **Meta'nın "otomatik özel mesaj" penceresi** çıkarsa her zaman **İptal**'e bas, Kaydet'e basma.
9. Kendi yorum cevabını düzeltmek için: üzerine gel → "..." → Düzenle → ctrl+a → yeni metin → Return. (Gönderilmiş Messenger mesajı düzenlenemez.)
10. **Tur Sonu Doğrulama Raporu:** Toplu tur bittiğinde kullanıcıya her müşterinin onay doğrulaması durumunu (`Doğrulandı / Başarılı`) içeren kesin sonuç tablosu sunulur.

## Kurallar
- Cevaplar Arapça (Mısır lehçesi), kişinin adıyla hitap (Arapça yazan için Arapça isim, Latin yazanın adı olduğu gibi).
- WhatsApp'a yönlendirirken Messenger/Facebook metinlerinde **sadece `https://wa.me/201066830373` linki** kullanılır (Arapça metinde sıra ters görünmesini önlemek ve tek tıkla açılması için). *(Not: Şirket numarası ve adresi yazma yasağı yalnızca `kedihane` reposu içindir; AB Ayçam reposunda ve Premiere Pro video şablonlarında `01066830373` ve fabrika adresi açıkça yazılır.)*
- **Açık Adres (sorulursa paylaşılabilir):** `العبور – القليوبية – المنطقة الصناعية B&C – قطعة 7 – بلوك 27003 – الدور الثالث`
- **Messenger'da fiyat ve modeller ekteki fiyatlı katalog PDF'inde (`kartelas 1 - fiyatlı.pdf`) paylaşılır (10.11.2026 güncellemesi):** Messenger yanıtlarında *"fiyat sadece WhatsApp'ta verilir"* ibaresi kullanılmaz; fiyat ve modellerin PDF'te olduğu belirtilir, detay ve sipariş için WhatsApp'a (`https://wa.me/201066830373`) yönlendirilir. (Yorumlarda dosya eklenemediği için yorum yanıtları WhatsApp'a yönlendirilmeye devam edilir.)
- Yorumda otomatik özel mesaj numarayı zaten gönderiyorsa ayrıca cevap yazma.
- Spam ve ilgisiz reklamlar atlanır.
- Reklam seti ve otomasyon değişiklikleri sadece onayla.
- Şifre/doğrulama kodu girilmez.

## Cevap şablonları ({ISIM} yerine kişinin adı)
**Facebook Gönderi Yorumu — Fiyat sorusu (Yorumlara PDF eklenemediği için):**
أهلاً {ISIM} 👋 سعر المتر بيختلف حسب الرسمة ونوع القماش. ابعتلنا رسالة على الصفحة أو كلمنا على واتساب عشان نبعتلك ملف الموديلات والأسعار (PDF) فوراً: https://wa.me/201066830373

**Facebook Gönderi Yorumu — Şekiller/modeller sorusu (Yorumlara PDF eklenemediği için):**
أهلاً {ISIM} 👋 عندنا أكتر من 39 رسمة وموديل للطباعة بالمتر. ابعتلنا رسالة على الصفحة أو كلمنا على واتساب عشان نبعتلك ملف الموديلات والأسعار (PDF) فوراً: https://wa.me/201066830373

**Messenger Ücretsiz Numune Şartları Sorusu (`kartelas 1 - fiyatlı.pdf` Ekli):**
أهلاً بحضرتك يا {ISIM} 👋 مفيش أي شروط خالص! حضرتك تشرفنا في مصنعنا بمدينة العبور بقماشك ونعمل لحضرتك عينة مجانية وتشوف جودة الطباعة بنفسك. وكل موديلاتنا وأسعارها موجودة في الملف المرفق (PDF) 📎 اختار اللي يعجبك، وللتفاصيل أو الحجز كلمنا على واتساب وهنرد على حضرتك فوراً: https://wa.me/201066830373

**Messenger Fabrika Dışından Kumaş Kabulü (`kartelas 1 - fiyatlı.pdf` Ekli):**
أهلاً {ISIM} 👋 أيوة طبعاً بنستلم القماش من عند حضرتك وبنطبعه بأعلى جودة تركي فصوص واستراس 💎 كل موديلاتنا وأسعارها موجودة في الملف المرفق (PDF) 📎 اختار اللي يعجبك، وللتفاصيل أو الحجز كلمنا على واتساب وهنرد عليك فوراً: https://wa.me/201066830373

**Standart Messenger Yanıtı (Modeller ve Fiyatlar PDF'te — 10.11.2026):**
أهلاً {ISIM} 👋 كل موديلاتنا وأسعارها موجودة في الملف المرفق (PDF) 📎 اختار اللي يعجبك، وللتفاصيل أو الحجز كلمنا على واتساب وهنرد عليك فوراً: https://wa.me/201066830373

**Sipariş isteği:**
أهلاً {ISIM} 👋 كل موديلاتنا وأسعارها موجودة في الملف المرفق (PDF) 📎 اختار الموديل اللي يعجبك، وتقدر تطلب طباعة على قماشك وتتابع التفاصيل على واتساب وهنرد عليك فوراً: https://wa.me/201066830373

**Kargo / teslimat sorusu (Messenger'da PDF ekiyle; gerçek kargo politikası kullanıcı teyidinde güncellenecek):**
أهلاً {ISIM} 👋 كل موديلاتنا وأسعارها موجودة في الملف المرفق (PDF) 📎 وبالنسبة لتفاصيل الشحن والتوصيل كلمنا على واتساب وهنرد عليك فوراً: https://wa.me/201066830373

**Teşekkür (olumlu yorum):**
شكراً لذوقك! لطلب كتالوج الموديلات والأسعار (PDF) أو أي تفاصيل كلمنا على واتساب: https://wa.me/201066830373

## Denenen ve olmayanlar
- Cevaba telefon numarasını yazı olarak koymak: kullanıcının ekranında numara sırası ters göründü. Sadece link bırakıldı. Eski cevaplarda yazılı numaralar vardı; yorumlarda Düzenle ile düzeltildi, Messenger mesajları düzenlenemediği için bekliyor.
- Meta'nın otomatik karşılama mesajı sadece "nasıl yardım edebiliriz" der; fiyat/link içermez, bu yüzden ayrıca cevap gerekir.

## Mevcut durum
11 Kasım: Son 36 saatlik turda 7 Messenger mesajı (`kartelas 1 - fiyatlı.pdf` ekli) ve 2 Facebook gönderi yorumu (`reel/1792770955308605`) tek sekmede sıralı gönderilip DOM üzerinden 9/9 doğrulandı.
13 Ekim: 7 yeni Messenger mesajı cevaplandı (sadece ismini yazıp beğeni atan bir kişi atlandı). Yorumlarda Meta otomatik yanıtı çalışıyor. Messenger'da yanıt kutusu konumu pencere boyutuna göre değişir (y≈677 veya 722); yazmadan önce ekran görüntüsüyle kutuyu doğrula. Gönderilen konuşma listenin en üstüne çıkar, alttakiler kaymaz.
12 Ekim: bekleyen tüm Messenger mesajları cevaplandı; tekrar soran yoktu. Eski mesajlar ve bazı yorumlar için `bekleyen-isler.md` dosyasına bak.
