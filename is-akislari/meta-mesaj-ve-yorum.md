# Meta mesaj ve yorum iş akışı

## Mesaj cevap kuralı (Güncelleme: 24.10.2026, kullanıcı kararı)
- Fiyat soran ve model/şekil isteyen herkese Messenger'da: kişinin adıyla hitap eden kısa metin + `E:\ab ayçam\kartela görüntüsü\kartelas 1 - fiyatlı.pdf` dosyası ek olarak gönderilir (24.10.2026'ya kadar `tüm kalıplar tek renk.pdf` kullanılıyordu, bu tarihte fiyatlı kartela PDF'ine geçildi).
- Metin (Mısır lehçesi, her mesajda kişinin adı kullanılır): `أهلاً {isim} 👋 كل موديلاتنا موجودة في الملف المرفق (PDF) 📎 اختار اللي يعجبك. الأسعار بنشاركها على واتساب بس. كلمنا هناك وهنرد عليك فوراً: https://wa.me/201066830373`
- Fiyat mesajda yazılmaz, detaylar ve sipariş için WhatsApp'a yönlendirilir.
- Her gönderimden önce PDF yolu kontrol edilir (`E:\ab ayçam\kartela görüntüsü\kartelas 1 - fiyatlı.pdf`). Dosya yoksa ya da adı değiştiyse gönderim durdurulur, kullanıcıya bildirilir; başka dosya gönderilmez.
- Her mesajda gönderilen linkin sonunda eksik hane olmadığı kontrol edilir (17.10'da bir mesajda son hane eksik çıktı, düzeltme mesajı gönderildi).
- Eski kural (model/fiyat sadece WhatsApp) güncellendi: model bilgisi PDF ile verilebilir, fiyat hâlâ sadece WhatsApp.

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
- Hesaplar Merkezi ve portföy işlemleri eski telefon numarasına doğrulama kodu istiyor; Instagram bağlama (ab_aycam) bu yüzden beklemede. Ayrıntı: ilerleme.md 17 Ekim.
