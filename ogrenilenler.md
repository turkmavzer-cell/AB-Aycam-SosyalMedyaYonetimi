# Öğrenilenler ve hatalardan çıkan dersler

Her işte yapılan hata, sebebi ve bundan sonraki kural burada tutulur. En yeni üstte.

## 21 Ekim 2026 — Messenger turu (dosya yükleme)
- **Ders (teknik):** Ataç butonu yerel dosya penceresi açar, DOM'da `input[type=file]` yoktur. Çözüm: sayfada `HTMLInputElement.prototype.click`'i yamala (file input'a `id=ab_upload_input` verip DOM'a ekle, açma), sonra `find` ile ref al, `file_upload` kullan. Yama sayfa yenilenene kadar yaşar; her kullanımdan önce eski `input#ab_upload_input`'ları sil.
- **Ders:** `file_upload` Windows yolunu kabul etmez ("izin verilen dosyalar"); PDF önce `device_stage_files` ile hazırlanır, container yolu (`/mnt/user-data/uploads/ab ayçam/tüm kalıplar tek renk.pdf`) verilir.
- **Ders:** Gönderim sonrası konuşmayı aç ve doğrula. Messenger "Bu hesap, herkesten gelen yeni mesaj isteklerine izin vermediği için mesajını alamıyor" yazabilir; o kişiye iletilemez, kullanıcıya bildir (WhatsApp/yazarsa tekrar).
- **Ders:** Konuşmada PDF zaten varsa tekrar gönderme; sadece metin + "اللي اتبعتلك فوق". Listedeki "Sen:" önizlemesi yanıltıcı olabilir, konuşmayı aç.
- **Ders:** Arama kutusundan isim açınca önce yorum konuşması çıkabilir; Messenger konuşma satırını seç, başlık adını doğrula. Sayfa kayarsa (ataç görünmez) ana sayfayı yukarı kaydır.

## 20 Ekim 2026 — Video 19 devam
- **Ders (onaylı yöntem):** Sim, kumaşın kadrajı doldurduğu kompozisyonlarda (başa sarılı şal, portre, yakın çekim) ve yan/arka ışıkta belirgin çıkar; uzak yarım boy çekimde kaybolur. Başlıca sim promptu bloğu her promptun içine gömülür (ayrı blok yapıştırma hatası azalır).
- **Ders (sim görünürlüğü):** Gerçek sim küçük çubuk parçalar; Gemini'de yarım boy çekimde kaybolur. Çözüm: yoğunluk/boyut sözel olarak artırılır ("clearly visible at first glance", yaklaşık 1-2 cm'de bir parça), yakın çekim kadrajı eklenir, koyu kumaş ve yan ışık kullanılır, referans olarak gerçek şal fotoğraflarının kırpımı verilir. Öbek yasağı korunur.
- **Ders (yazı şablonları):** Uzun Arapça satırlar kutudan/çerçeveden taşar (draw_line otomatik küçültmez); tmpl_gen3.py'ye genişliğe göre font küçülten sarmalayıcı eklendi. Yeni metin üretince kontrol kâğıdı (gri zeminde) bak.
- **Ders (Premiere XML):** Açık Premiere'e sekans eklemek için FCP7 xmeml üret, Ctrl+I ile içe aktar. Basic Motion `center` değeri sekansa değil klibin KENDİ piksel boyutuna göre normalize edilir: horiz=(hedefX-kareMerkezX)/klipGenişlik, vert=(hedefY-kareMerkezY)/klipYükseklik; scale % olarak doğrudan. Opacity keyframe'leri çalışır. İçe aktarmadan sonra monitörde doğrula.
- **Hata:** `computer_open_application` ile "Premiere 2026" açtım, oysa açık proje 2025'teydi; 2026 uyumluluk penceresi arkada kaldı. **Ders:** önce hangi sürümün açık olduğuna bak (görev çubuğu önizlemesi), onu aç.
- **Ders:** Yapay zekâ (Gemini) görselleri "işlerimiz" gibi sunulmaz; başlık "إطلالات" + "صور توضيحية" notu. Ürün kumaşlarında olmayan renk veya öbek sim görünen görsel videoya konmaz.
- **Ders:** Premiere dizisi kullanıcı tarafında değişir (klip süreleri 29,8 → 32,6 sn oldu); şablon yazı zamanlarını sabit varsayma, her devam işinde `.prproj` (gzip XML, VideoClipTrackItem Start/End ve Clip InPoint/OutPoint, /254016000000) yeniden okunup yazılar yeniden zamanlanır.
- **Ders:** Açık Premiere projesi yazılmaz; çıktı önizleme mp4 + zamanlama tablosu + tam kadraj PNG'ler olarak verilir.
- **Ders:** Foto beat'leri (dörtlü/ikili/tek) ayrı mp4 parçaları olarak üretilip `concat -c copy` ile birleştirilir; hepsi aynı kodlama/timescale ile.

## 19 Ekim 2026 — Sim serpme dağılımı (v15 → v16)
- **Hata:** v15 promptlarında sim öbek/desen çıktı. **Sebep:** referans karelerinde ışık parlaması lekeleri vardı (sim kümesi sanıldı) ve prompt "yoğunluk" tarif ediyordu. **Ders:** sim üfleme makinesiyle serpme uygulanır; prompta "rastgele, eşit, tek tek ayrı toz, aralarında boş kumaş, öbek/desen yok" olumlu biçimde yaz; referans karesini parlaması/yoğun lekesi olmayan kırpımdan seç ve görsele bakarak doğrula.
- **Ders:** Loş ortam görselleri için ayrı blok kullan (flaş/küçük lamba, kumaş rengi koyulaşmasın, ışık efekti yok).

## 19 Ekim 2026 — Sim numune kurgusu ve şal promptları
- **Ders (araç):** Cihan'ın bilgisayarındaki Linux VM (device_bash) 2 çekirdek; çağrı başı en çok 180 sn, arka plan işlemi çağrı bitince ölüyor (setsid/nohup işe yaramıyor) ve `rm` yasak. Uzun render'ı parçala: ana kurgu (xfade) + 3 yazı parçası (frame sınırlarında) + `concat -c copy`. Hatalı denemeleri silme, `mv` ile `_calisma\eski_denemeler`'e taşı.
- **Hata:** xfade zincirinde fotoğraf/döngü girişi ile video girişinin timebase'i uyuşmadı ("First input link main timebase ... do not match"). **Ders:** tüm girişleri `setpts=PTS-STARTPTS,fps=30,settb=1/30,format=yuv420p` ile normalize et.
- **Hata:** Renk etiketinde yazı nokta ile çakıştı; uzun alt yazı satırı (4 kelimelik liste) ekran dışına taştı. **Ders:** üretimden sonra bindirme PNG'lerini gri zeminde ön izleyip bak; uzun satırda font küçült.
- **Ders:** Telefon videoları dikey 4K HEVC (rotate=90); ffmpeg otomatik döndürür. Önce kontak sayfasıyla incele; bir video tamamen siyah çıktı (kullanılmadı).
- **Ders (Gemini referansı):** Referans karede zemin/duvar kenarı görünüyorsa kırp; Gemini onu da şala/sahneye taşıyabilir.
- **Ders (ekip):** Ankara'ya verilen görev metninde bozuk/anlamsız kelimeler (yazım hatası) vardı; ajan toparladı ama görev tanımı gönderilmeden önce okunmalı.
- **Ders (ekip):** Ankara yalnız metin üretir (Write yok); dosyaya Tekir yazar. Kaliko işi sürekli device_bash gerektirdiği için ana oturumda yapıldı.

## 20 Ekim 2026 — Messenger/yorum turu
- **Ders:** `file_upload` (4,7 MB PDF) sırasında Chrome eklentisi bağlantısı kopabiliyor; dosya yine de yüklenebiliyor ama her zaman değil. Bağlantı kopunca önce ekran görüntüsü/`tabs_context_mcp` ile durumu kontrol et, kutuda PDF çipi yoksa yeniden yükle; körlemesine tekrar gönderme. Bu turda 1 konuşmada metin gitti, PDF ayrıca yeniden yüklenip gönderildi.
- **Ders:** Konuşma listesinde satırlar `role=presentation` div'idir (427x92); isim araması için tam isim yerine kısa parça kullan (ى/ي farkı, "Mahmoud Salah" gibi). Başlık doğrulamasında `includes` kullan.
- **Ders:** Facebook yorumlarında fiyat/adres/telefon soruları Meta otomasyonu tarafından zaten cevaplanıyor ("1 yanıtı gör" + 2 sn önceki yanıt). Önce "1 yanıtı gör" açıp içerik ve wa.me linki kontrol edilir; elle cevap sadece otomatiğin karşılamadığı sorularda (örn. "kumaşı siz mi veriyorsunuz?") yazılır.
- **Ders:** Spam/reklam yorumları "Gizle" ile gizlenir (silinmez); ilk seferde çıkan "Gizleme Özelliği" bilgi penceresinde Tamam'a basılır.
- **Ders:** Messenger'daki Meta otomatik cevabı bazı konuşmalarda yazılı telefon numarası taşıyor; bu bizim cevabımız sayılmaz, kişiye isimli metin + PDF yine gider.
- **Ders:** Gönder düğmesi ikiden fazla olabilir; son `Gönder` role=button ele alınır ve rengi `rgb(0,0,0)` olunca (yükleme bitince) tıklanır. PDF çipi dönen halka gösteriyorsa 10-20 sn daha beklenir.
- **Ders:** Yorum cevabında Meta'nın otomatik özel mesaj popup'ı yazılan metni yutabilir; İptal'e basıp tekrar Yanıtla → yaz (Kaydet'e basma).

## 19 Ekim 2026 — Video 18 yazı/bitiş şablonları
- **Hata:** İlk üretimde "AB AYÇAM" ve telefon numarası ters dizildi (0373 683 106 +20). **Ders:** Arapça satırda ardışık Latin/rakam kelimeler tek LTR blok olmalı. Üretimden sonra mutlaka ön izleme görüntüsüne bak.
- **Ders:** Premiere `.prproj` gzip'li XML; klip süreleri/in-point'ler okunup görüntüye uygun yazı zamanlaması çıkarılabilir.
- **Ders:** Eski tasarım klasörleri/betik silinmiş olabilir; betik, font ve logo üretilen şablon klasöründe `_kaynak` olarak yedeklenir.
- **Kural:** Video bitiş kartında sadece 0373 ile biten numara.

## 18 Ekim 2026 — Messenger toplu cevap + PDF turu
- **Hata:** Bir cevapta wa.me linkinin son hanesi eksik gitti (…20106683037). **Ders:** Her mesajdan önce linkin tam `https://wa.me/201066830373` olduğunu kontrol et; hata olursa düzeltme mesajı at ve kullanıcıya söyle.
- **Hata:** "PDF gitti" kontrolü, kutudaki dosya çipini sayınca yanlış pozitif verdi. **Ders:** Başarıyı sadece sohbet listesindeki "Bir dosya eki gönderdin" önizlemesiyle doğrula.
- **Hata:** PDF yüklenmeden Gönder'e basılınca dosya gitmedi (3 konuşma). **Ders:** PDF ~4,7 MB, yükleme 10+ sn sürüyor; Gönder yazısı siyah olunca tıkla.
- **Hata:** Aynı konuşmada PDF çipi iki kez eklendi. **Ders:** Göndermeden önce çip sayısına bak, fazlayı kaldır.
- **Hata:** Önceki turda ~23 konuşma yanlış satıra denk gelip atlandı. **Ders:** Konuşmayı açtıktan sonra başlık adını doğrula, sonra yaz.
- **Hata:** "Önerilen yanıt" çubuğu kutuya yazılı numara taşıyabiliyor. **Ders:** Kullanma; kutuya girerse temizle.
- **Ders:** Liste önizlemesi gecikebilir; "CHECK" çıkanları tek tek açıp bak, tekrar gönderme.
- **Ders:** Tek seferde çok konuşma gezen JS komutu 45 sn'de zaman aşımına uğruyor; konuşmaları tek tek işle.
- **Ders:** Müşteri adı içeren listeler repoya değil `yerel-kayitlar/` klasörüne (gitignore'da) yazılır.
- **Ders:** İsimsiz/anlamsız mesaj (çıkartma, cevapsız arama bildirimi) atanlara da, önceden soru sormuşlarsa, standart metin+PDF gider.
- **Ders:** Kullanıcıya sunulan bir dosya (liste vb.) kök klasörde kaybolabiliyor; kalıcı olması gerekenler `github-guncelleme\` altına, kök klasöre değil.
- **Ders (kullanıcı kararı):** Her yapılan işi klasöre koymak gerekmez. Klasöre sadece istenen promptlar/benzer kalıcı kaynaklar ve iş akışı öğrenilenleri girer.
- **Ders:** Kullanıcı bir sohbette tek tek "tamam mı, tekrar kontrol et" derse tüm metni baştan okuyup eksik madde ara; bu turda son güncelleme listesinde `ogrenilenler.md` eksikti.
- **Ders:** Hesap/portföy doğrulaması eski numaraya gidiyorsa Meta destek asistanı talep açamıyor; kimlik yükleme yolu telefon uygulamasında aranmalı.
- **Instagram:** AB sayfası portföyde değil; portföye eklemek eski numaraya kod istiyor. Meta destek asistanı talep açamıyor. Denenecek: telefon/başka tarayıcıdan "Kimlik Yükle", Meta kurtarma süreci.
