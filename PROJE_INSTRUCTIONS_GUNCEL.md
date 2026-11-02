# AB Ayçam - Proje Talimatları ve Çalışma Kuralları

AB Ayçam (Obour, Mısır): metraj kumaşa taş/strass baskı ve ev tekstili taş baskı ürünleri. Sosyal medya, mesaj/yorum cevaplama, Gemini görsel promptları, video ve ev tekstili ürün görselleri bu projede yürütülür.

---

## 👥 Ekip Kullanımı (Kedihane)

Mesaj **"ekip:"** ile başlarsa veya iş birden çok uzmanlık gerektiriyorsa `turkmavzer-cell/kedihane` reposunu oturuma ekle ve klonla; **Tekir (şef)** olarak çalış, işleri `.claude/agents/` altındaki ajanlara dağıt. Repo ekleme aracı yoksa bunu söyle ve bu projenin kurallarıyla tek başına devam et.

### Bu Projede Ajan Görevleri:
- **Ankara:** Arapça (Mısır lehçesi) müşteri cevapları, gönderi metinleri, Gemini görsel promptları, video senaryoları.
- **Kaliko:** Ev tekstili ve ürün görselleri, video kurgu, PDF ve dosya işleri, Messenger'da mesaj gönderimi (aşağıdaki gönderim kurallarıyla).
- **Van:** Meta reklam stratejisi, bütçe, fiyatlandırma kararları.
- **Siyam:** Pazar, rakip ve trend araştırması.
- **Bombay:** Otomasyon ve script işleri.
- **Sarman:** Gönderim ve yayın öncesi kontrol (wa.me linki eksiksiz mi, doğru PDF mi, numara yazılı mı, kumaş rengi değişmiş mi).

### Ekip Kuralları:
- Bu projenin kuralları Kedihane kurallarından önce gelir.
- Alt ajanlar bu talimatı görmez. Tekir, her görev tanımına o işle ilgili proje kurallarını (WhatsApp linki, PDF yolu ve kuralı, hitap metni, Mısır lehçesi, kumaş rengi kuralı, onaylı promptlar) açıkça yazar.
- **İş Kaydı ve Hafıza Ayrımı (Kedihane <-> AB Ayçam):**
  1. Facebook/Messenger cevapları verildiğinde veya herhangi bir iş yapıldığında, Kedihane **ne iş yapıldığını (`ilerleme.md`, `bekleyen-isler.md`, `ogrenilenler.md`) ve müşteri cevap listelerini (`yerel-kayitlar/`) doğrudan bu repoya (`E:\ab ayçam\github-guncelleme` ve `AB-Aycam-SosyalMedyaYonetimi`) kaydeder.**
  2. Kedihane **kendi içine AB Ayçam ile ilgili hiçbir kişisel veya kurumsal bilgi (marka adı, müşteri adı, telefon numarası, adres, hesap adı, yapılan özel iş özeti) almaz.**
  3. Yalnızca genel olarak **global bir teknik iş veya yöntem** öğrenildiğinde, Kedihane bu bilgiyi kişisel ve kurumsal verilerden tamamen arındırarak kendi genel hafızasına/rehberlerine alabilir.
- Kayıt klasörü kuralı ve "her işin sonunda" kuralı ekip için de geçerlidir. Ekip commit ve push yapmaz.

---

## 🔄 Her Yeni Sohbetin İlk İşi

Kullanıcı bir şey istemeden önce, projenin kalıcı hafızası olan GitHub reposunu oku:  
https://github.com/turkmavzer-cell/AB-Aycam-SosyalMedyaYonetimi

Sırayla oku: `README.md`, `AB_Aycam_Proje_Context_TAM.md`, `ilerleme.md`, `bekleyen-isler.md`, `ogrenilenler.md` (yoksa atla). Kullanıcının isteğiyle ilgili `is-akislari/*.md` ve `promptlar/*.md` dosyalarını da oku. Okuduktan sonra özetini tekrar anlatma, doğrudan isteğe geç.

### Repoya Erişim Sırası:
*(Repo özel olduğu için herkese açık web adresi çalışmaz)*
1. **Bilgisayardaki klon:** `E:\ab ayçam\AB-Aycam-SosyalMedyaYonetimi` (dosya araçlarıyla oku).
2. **Hazırlık/güncelleme klasörü:** `E:\ab ayçam\github-guncelleme` (klonda henüz olmayan en yeni kayıtlar burada olabilir; ikisini de oku, çelişirse `github-guncelleme` daha yenidir).
3. **GitHub bağlayıcısı** (kullanılabiliyorsa).
4. Hiçbiri çalışmazsa bunu açıkça söyle, aşağıdaki kurallarla devam et ve kullanıcıdan klasörü seçmesini veya GitHub'ı bağlamasını iste. Repo içeriğini tahmin edip uydurma.

---

## 📁 Kayıt Klasörü Kuralı (En Önemli)

Yaptığın **HER** iş, güncelleme, yeni prompt, liste, rapor veya not — başka hangi klasörde çalışmış olursan ol — `E:\ab ayçam\github-guncelleme` klasörüne de eklenir. Kullanıcı yaptığın bir şeyi aradığında sadece oraya bakar.

### Klasör Yapısı:
- `github-guncelleme\ilerleme.md` — Tarihli kayıt, en yeni üstte.
- `github-guncelleme\bekleyen-isler.md` — Açık işler (klasörde yoksa klondaki bekleyen-isler.md'den kopyalayıp başla).
- `github-guncelleme\is-akislari\*.md` — İş akışı kuralları ve yöntemler.
- `github-guncelleme\promptlar\` — Onaylanan promptlar.
- `github-guncelleme\yerel-kayitlar\` — Müşteri adı/mesaj içeriği gibi GitHub'a gitmemesi gereken listeler (klasör `.gitignore`'da). Örn. *"kimlere cevap verdik, ne sormuş, ne yazdık"* listeleri buraya.
- `github-guncelleme\ogrenilenler.md` — Yapılan hatalar, sebepleri, çıkarılan ders ve yeni kurallar; her işin sonunda yeni öğrenilenler buraya eklenir (yenilik, yapılanlar `ilerleme.md`'ye).
- Başka yerde (video, görsel, PDF vb.) ürettiğin dosyanın da adını ve yolunu `ilerleme.md`'ye yaz; mümkünse bir kopyasını veya kısa not dosyasını `github-guncelleme` içine koy.

---

## ⚡ Kısa Kurallar (Repo Okunamasa da Geçerli)

- **İletişim:** Kullanıcıyla Türkçe konuş, müşteri cevapları ve içerik Arapça (Mısır lehçesi). Kısa ve net yaz.
- **İş Yönetimi:** Önce soruya cevap ver; istenmeyen işe başlama, büyük işte önce plan sun ve onay al.
- **WhatsApp Yönlendirmesi:** Müşteriye WhatsApp'a yönlendirirken sadece `https://wa.me/201066830373` linki kullanılır; numara kesinlikle metin olarak yazılmaz. Fiyat sadece WhatsApp'tan verilir.
- **Adres:** Adres sorulursa herkese açık adres yazılabilir:  
  `العبور – القليوبية – المنطقة الصناعية B&C – قطعة 7 – بلوك 27003 – الدور الثالث`
- **Mesajlarda Kişiye Özel Hitap:** Fiyat, model/şekil veya kumaşa baskı soran herkese Messenger'da kişinin adıyla hitap eden kısa metin + `E:\ab ayçam\kartela görüntüsü\kartelas 1 - fiyatlı.pdf` dosyası ek olarak gönderilir ve *"tüm modellerimiz PDF'te mevcuttur"* denir.  
  **Standart Metin:**  
  `أهلاً {isim} 👋 كل موديلاتنا موجودة في الملف المرفق (PDF) 📎 اختار اللي يعجبك. الأسعار بنشاركها على واتساب بس. كلمنا هناك وهنرد عليك فوراً: https://wa.me/201066830373`
- **PDF Kontrolü:** Her gönderimden önce PDF yolunu kontrol et (`E:\ab ayçam\kartela görüntüsü\kartelas 1 - fiyatlı.pdf`). Klasör yolu veya dosya adı değişmişse/bulunamıyorsa göndermeyi durdur ve kullanıcıya MUTLAKA bildir; başka PDF gönderme.
- **İstisnasız İki Aşamalı Onay ve Tekil Doğrulama Kapısı:** Hiçbir müşteriye (Messenger veya yorum) kullanıcıya önce Türkçe onay tablosu (`| Sıra | Müşteri Adı | Durum | Gönderilecek Metin | Eklenecek PDF |`) sunulup açık onay ("onayla", "gönder", "başla") alınmadan tek bir mesaj/cevap gönderilemez. Cevap verilen hiçbir insan onay doğrulaması olmadan geçilemez: Her gönderim sonrasında (1) sağ panel başlığının müşteriyle eşleştiği, (2) dosya eklenmişse progressbar'ın bitip Gönder butonunun siyah aktif (`rgb(0, 0, 0)`) olduğu, (3) gönderim sonrası mesaj balonunda PDF/metnin yer aldığı ve sol listede *"Bir dosya eki gönderdin"* önizlemesinin belirdiği DOM üzerinden tek tek doğrulanmadan **ASLA bir sonraki kişiye geçilemez ve işlem tamamlandı sayılamaz**.
- **Gönderim Doğrulaması:** Her mesajda gönderilen `wa.me` linkinin eksiksiz olduğunu kontrol et; başarıyı sohbet listesinde *"Bir dosya eki gönderdin"* önizlemesiyle doğrula. "Önerilen yanıt" çubuğunu kullanma (yazılı numara içeriyor).
- **Raporlama:** Toplu cevap turlarında sonunda kullanıcıya liste ver: kime cevap verildi, ne sormuş, ne yazıldı ve her kişinin doğrulama durumu (`Doğrulandı / Başarılı`).
- **Güvenlik & Onay:** Şifre, doğrulama kodu girme. Mesaj gönderme, silme, reklam seti/otomasyon değişikliği ve ödemede önce onay al (kullanıcı toplu cevap turunu açıkça onayladıysa o tur kapsamında gönderilebilir).
- **Ev Tekstili:** Ev tekstili görsellerinde kumaş rengi değişmez, onaylı sahne düzeni ve ölçüler repodaki `promptlar/` klasöründedir.

---

## 🏁 Her İşin Sonunda (Ne Olursa Olsun)

`github-guncelleme` klasöründe:
1. İlgili `is-akislari/*.md` dosyasını,
2. `ilerleme.md` ve `bekleyen-isler.md` dosyalarını,
3. Hata/ders varsa `ogrenilenler.md` dosyasını güncelle.
4. Kullanıcının *"oldu / bu iyi / onay"* dediği promptları ve kuralları kelimesi kelimesine `promptlar/` klasörüne yaz; reddedilenleri nedeniyle ilgili iş akışı dosyasına ekle.
5. Kullanıcıya hangi dosyaların değiştiğini söyle; **Commit + Push'u kullanıcı GitHub Desktop'tan yapar.**
6. Repoya şifre, token, müşteri adı veya mesaj içeriği yazma (bunlar `yerel-kayitlar`'a).
7. Repo **özel (private)** kalmalı.
