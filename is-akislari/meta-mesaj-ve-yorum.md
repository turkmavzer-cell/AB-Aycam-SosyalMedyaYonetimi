# Meta mesaj ve yorum iş akışı

## İstisnasız İki Aşamalı Onay ve Tekil Doğrulama Kapısı (02.11.2026, Kullanıcı Kararı)
- **Ön Onay Şartı:** Hiçbir müşteriye (Messenger veya yorum) doğrudan cevap verilemez. Önce yöneticiye Türkçe onay tablosu (`| Sıra | Müşteri Adı | Durum | Gönderilecek Metin | Eklenecek PDF |`) sunulur. Kullanıcı açıkça onaylamadan ("onay / gönder / başla") tek bir mesaj bile tetiklenemez.
- **Tekil Doğrulama Kapısı (Hiçbir İnsan Doğrulanmadan Geçilemez):**
  1. Sağ paneldeki başlık adının hedef müşteriyle birebir eşleştiği teyit edilir.
  2. Dosya eklenmişse (`kartelas 1 - fiyatlı.pdf`) progressbar kapanmadan ve Gönder butonu aktif siyah renge (`rgb(0, 0, 0)`) dönmeden tıklama yapılmaz.
  3. Gönderim sonrası sağ panel mesaj balonunda PDF eki ve sol konuşma listesinde *"Bir dosya eki gönderdin."* önizlemesi DOM üzerinden kesin olarak doğrulanır.
  4. **Doğrulanmayan hiçbir konuşma geçilemez, başarılı sayılamaz ve bir sonraki müşteriye geçilmez.**
  5. Tur bitiminde tüm listenin onay doğrulaması durumu (`Doğrulandı / Başarılı`) kullanıcıya raporlanır.

## Mesaj cevap kuralı (Güncelleme: 10.11.2026, kullanıcı kararı)
- Fiyat soran ve model/şekil isteyen herkese Messenger'da: kişinin adıyla hitap eden kısa metin + `E:\ab ayçam\kartela görüntüsü\kartelas 1 - fiyatlı.pdf` dosyası ek olarak gönderilir (24.10.2026'ya kadar `tüm kalıplar tek renk.pdf` kullanılıyordu, bu tarihte fiyatlı kartela PDF'ine geçildi).
- Metin (Mısır lehçesi, her mesajda kişinin adı kullanılır): `أهلاً {isim} 👋 كل موديلاتنا وأسعارها موجودة في الملف المرفق (PDF) 📎 اختار اللي يعجبك، وللتفاصيل أو الحجز كلمنا على واتساب وهنرد عليك فوراً: https://wa.me/201066830373`
- **Önemli Güncelleme (10.11.2026):** `kartelas 1 - fiyatlı.pdf` içinde 39 modelin adları ve EGP fiyatları (`38 EGP`–`75 EGP`) yer aldığı için artık mesajlarda *"fiyat sadece WhatsApp'ta verilir"* ibaresi kullanılmaz; fiyat ve modellerin PDF'te olduğu belirtilir, detay ve sipariş için WhatsApp'a yönlendirilir.
- Her gönderimden önce PDF yolu kontrol edilir (`E:\ab ayçam\kartela görüntüsü\kartelas 1 - fiyatlı.pdf`). Dosya yoksa ya da adı değiştiyse gönderim durdurulur, kullanıcıya bildirilir; başka dosya gönderilmez.
- Her mesajda gönderilen linkin sonunda eksik hane olmadığı kontrol edilir (17.10'da bir mesajda son hane eksik çıktı, düzeltme mesajı gönderildi).
- Eski kural (model/fiyat sadece WhatsApp) tamamen güncellendi: Messenger'da hem modeller hem fiyatlar `kartelas 1 - fiyatlı.pdf` ile paylaşılır; WhatsApp detay, sipariş ve randevu içindir.
- **Ücretsiz Numune Şartı Kalıbı (Messenger PDF Ekli):** `أهلاً بحضرتك يا {isim} 👋 مفيش أي شروط خالص! حضرتك تشرفنا في مصنعنا بمدينة العبور بقماشك ونعمل لحضرتك عينة مجانية وتشوف جودة الطباعة بنفسك. وكل موديلاتنا وأسعارها موجودة في الملف المرفق (PDF) 📎 اختار اللي يعجبك، وللتفاصيل أو الحجز كلمنا على واتساب وهنرد على حضرتك فوراً: https://wa.me/201066830373`
- **Fabrika Dışından Kumaş Kabulü Kalıbı (Messenger PDF Ekli):** `أهلاً {isim} 👋 أيوة طبعاً بنستلم القماش من عند حضرتك وبنطبعه بأعلى جودة تركي فصوص واستراس 💎 كل موديلاتنا وأسعارها موجودة في الملف المرفق (PDF) 📎 اختار اللي يعجبك، وللتفاصيل أو الحجز كلمنا على واتساب وهنرد عليك فوراً: https://wa.me/201066830373`
- **Facebook Yorum Yanıtı (PDF eklenemediği için):** `أهلاً {isim} 👋 ابعتلنا رسالة على الصفحة أو كلمنا على واتساب عشان نبعتلك ملف الموديلات والأسعار (PDF) فوراً: https://wa.me/201066830373`
- **Gizlilik Ayrımı:** Şirket telefon numarası (`01066830373`) ve açık adres (`العبور – القليوبية – المنطقة الصناعية B&C – قطعة 7 – بلوك 27003 – الدور الثالث`) yasağı yalnızca `kedihane` reposu içindir; AB Ayçam reposunda kısıt yoktur.

- Yöntem (18.10 turunda işledi): metni yaz+Enter, ardından ataç ikonu → dosya yükle, yükleme bitince (Gönder yazısı siyah) Gönder; başarı ölçütü listede "Bir dosya eki gönderdin" önizlemesi. Adres soran kişiye herkese açık adres yazılabilir. Cevapsız arama bildirimi olup önceden soru sormuş kişiye de standart metin+PDF gider.

## Yorum kuralı (19.10.2026)
- Yorumlarda fiyat/adres/telefon soranlara Meta otomatik cevap veriyor (isimli, wa.me linkli). Önce "1 yanıtı gör" açıp doğrula; eksik/yanlışsa elle cevap yaz.
- Otomatiğin karşılamadığı sorulara elle kısa Mısır lehçesi cevap + wa.me (örn. kumaşı müşteri seçer, biz toptan metre/top boyunca strass yapıştırırız).
- Spam/reklam yorum (site linki, "platform" reklamı) cevaplanmaz, "Gizle" ile gizlenir.
- Yorum cevabı yöntemi: Yanıtla → End (etiket kalır) → metni yaz → Enter. Çıkan Meta popup'ı yazdığını yutarsa İptal, tekrar Yanıtla.
- Adres soran Messenger kişisine metne adres satırı eklenir (PDF yine gider).

## Teknik (20.10.2026)
- Sıra: metin → Enter → ataç (`Bir dosya ekle`) → `input type=file` → `file_upload` → çip yüklenince son Gönder'e tıkla → listede "Bir dosya eki gönderdin" kontrolü. `file_upload` bağlantıyı koparabilir; kopunca ekran görüntüsüyle çip durumuna bak, yoksa yeniden yükle.

## Dosya yükleme yöntemi (21.10.2026, işledi)
1. PDF'i `device_stage_files` ile hazırla. 2. Sayfada `HTMLInputElement.prototype.click` yamasını uygula (file input'u `id=ab_upload_input` yapıp DOM'a bırakır). 3. Metni yaz, ataç → `find` ile input ref → `file_upload` (container yolu). 4. Çip yüklenince Gönder. 5. Konuşmada tam wa.me linki ve PDF'i doğrula.
- Konuşmada PDF varsa sadece metin gönder. Yeni mesaj isteklerine kapalı hesaba mesaj iletilemez (uyarı çıkar), kullanıcıya bildir.

## Notlar
- Meta "Önerilen yanıt" çubuğu yazılı telefon numarası içerir, kullanılmaz. Kutuya girerse temizlenir.
- Sol sohbet listesinde `"Sen: Merhaba ..."` veya `"Sen: أهلاً بيك في AB إسطنبول"` önizlemesi Meta otomatik karşılama mesajıdır; gerçek insan yanıtı sayılmaz. Tarama sırasında bu konuşmalar cevapsız aday olarak açılıp kontrol edilmelidir.
- Yükleme kontrolünde üst banner'daki ilgisiz `progressbar` yerine `[role="listitem"] [role="progressbar"]` ve `[aria-busy="true"]` yokluğu kontrol edilir; metin girişinde yalnızca `type_text` kullanılır (`paste` + `type_text` birlikte uygulanmaz).
- Hesaplar Merkezi ve portföy işlemleri eski telefon numarasına doğrulama kodu istiyor; Instagram bağlama (ab_aycam) bu yüzden beklemede. Ayrıntı: ilerleme.md 17 Ekim.
