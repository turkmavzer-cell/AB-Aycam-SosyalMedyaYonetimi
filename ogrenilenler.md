## 10 Kasım 2026 — Premiere Pro Şablonlarında Link Yerine Açık WhatsApp Numarası & Şirket Adresi Zorunluluğu ve Gizlilik Sınırı Ayrımı
- **Hata / Karışıklık:** Premiere Pro video şablonlarında (`antigravity 8` v1 ve `27 - şal` v1) WhatsApp numarası yerine `https://wa.me/201066830373` linki yazılmış ve bazı bitiş kartlarına şirket adresi eklenmemişti; ayrıca `kedihane` reposundaki telefon/adres gizliliği AB Ayçam reposuna da uygulanıyormuş gibi karışıklık doğmuştu.
- **Kesin Kural (10.11.2026):**
  1. **Premiere Pro & Video Şablonlarında Açık Numara + Adres:** Bundan sonra oluşturulacak tüm Premiere Pro şablonlarında (PNG, MOV/MP4, bitiş/CTA kartları ve XML) WhatsApp **kesinlikle `wa.me` linki olarak yazılmaz**; yerine WhatsApp ikonuyla doğrudan okunur **`01066830373`** numarası yazılır ve **şirket fabrika adresi mutlaka eklenir** (`مصنع إيه بي أيشام — العبور – القليوبية – المنطقة الصناعية بي آند سي – قطعة 7 – بلوك 27003 – الدور الثالث`). Videoda *"الأسعار عبر واتساب فقط"* yerine PDF katalog/fiyat çağrısı veya ücretsiz numune daveti kullanılır.
  2. **Kanal Ayrımı:** `https://wa.me/201066830373` linki yalnızca tıklanabilir Messenger/Facebook yazılı metin ve yorum yanıtlarında kullanılır.
  3. **Repo Gizlilik Sınırı:** Telefon numarası ve şirket adresi yasağı **yalnızca `kedihane` reposu içindir**. AB Ayçam reposunda şirket telefon numarası ve adresinin yazılmasında **hiçbir kısıtlama yoktur** (yalnızca bireysel müşteri adları ve mesaj içerikleri `yerel-kayitlar/` içinde saklanır).

## 10 Kasım 2026 — Fiyatlı Kartela PDF'i (`kartelas 1 - fiyatlı.pdf`) İçerik Doğrulaması ve Cevap Şablonu Güncellemesi
- **Bulgular / Ders:** `E:\ab ayçam\kartela görüntüsü\kartelas 1 - fiyatlı.pdf` içeriği incelendiğinde 39 sayfanın tamamında hem desen adlarının hem de metraj fiyatlarının (`38 EGP`–`75 EGP`) yer aldığı doğrulandı. Eski `tüm kalıplar tek renk.pdf` döneminden kalan *"fiyat sadece WhatsApp'ta verilir"* (`الأسعار بنشاركها على واتساب بس`) cümlesi PDF içeriğiyle çelişmekteydi.
- **Yeni Kural:** Messenger yanıtlarında `kartelas 1 - fiyatlı.pdf` gönderilirken *"fiyat sadece WhatsApp'ta verilir"* ibaresi **kesinlikle kaldırılır**; bunun yerine **hem modellerin hem fiyatların ekteki PDF'te bulunduğu** (`وكل موديلاتنا وأسعارها موجودة في الملف المرفق (PDF) 📎`) yazılır, detay/sipariş/randevu için `https://wa.me/201066830373` linkine yönlendirilir.

## 10 Kasım 2026 — Meta Business Suite'te "Sen: Merhaba ..." Otomatik Karşılama Önizlemesi Tuzağı
- **Hata / Tuzak:** Sol sohbet listesinde son önizlemesi `"Sen: Merhaba ..."` (veya `"Sen: أهلاً بيك في AB إسطنبول"`) ile başlayan bazı konuşmalarda, müşterinin reklam üzerinden gönderdiği soruların hemen ardından Meta'nın otomatik karşılama mesajı tetiklenebilmektedir. Yalnızca `"Sen:"` önekine bakılarak bu konuşmalar cevaplanmış sanıldığında gerçek cevapsız müşteri soruları gözden kaçmaktadır.
- **Kural & Doğrulama:** Taramada son önizlemesi `"Sen: Merhaba"` veya otomatik karşılama metniyle başlayan tüm konuşmalar cevapsız aday olarak açılıp doğrulanır. Ayrıca Lexical düzenleyiciye `ClipboardEvent("paste")` + `type_text` birlikte uygulanmaz (metni çift yazar), yalnızca `type_text` kullanılır; PDF yükleme kontrolünde üst banner'daki ilgisiz `progressbar` yerine `[role="listitem"] [role="progressbar"]` ve `[aria-busy="true"]` yokluğu ile son `Gönder` butonunun siyah (`rgb(0, 0, 0)`) aktif olması doğrulanır.

## 9 Kasım 2026 — Premiere Şablonlarında Çok Dilli Karmaşa Yasağı ve %100 Arapça Standardı
- **Kural & Karar:** Mısır pazarında yerel tekstil atölyeleri, konfeksiyon fabrikaları ve son tüketicilere hitap eden sosyal medya videolarında Türkçe veya İngilizce ara başlıklar dikkat dağıtmakta ve yabancı algısı oluşturmaktadır. Antigravity şablonlarında artık Türkçe/İngilizce çift dillilik yerine **%100 saf Mısır ticari Arapçası** uygulanır; Latin harfleri yalnızca gerekli https://wa.me/201066830373 linki ve dosya adlarında tutulur.

## 9 Kasım 2026 — Premiere Pro Antigravity 8: Kumaş Alanını Korumak İçin Alandan Tasarruf Eden Minimalist Cam Mimari ve Taş Baskı İzolasyonu
- **Bulgu & Analiz:** Video içinde kumaşın dökümünü, modelin duruşunu ve özellikle taşların ışıltısını gösterirken geniş/büyük arka planlı kartların ekranın %40-50'sini kapattığı ve videonun merkezindeki ürünü gölgelediği tespit edildi. Ayrıca sim ve taş baskının farklı operasyonlar olması nedeniyle şablonlarda sim unsurlarının bulunmaması talep edildi.
- **Kural & Çözüm:**
  1. **Minimalist Alan Tasarrufu (%85+ Açık Alan):** Şablonlar sadece üstte yüzen ince kapsül (Y: 220-350, Yükseklik ~120px) ve altta Reels güvenli alanının hemen üstündeki alt üçte bir (lower-third Y: 1420-1620) bölgelerine yerleştirilir. Merkez kumaş bölgesi (Y: 380-1400) %100 açık bırakılır.
  2. **Yalnızca Taş Baskı İzolasyonu:** Şablon metinlerinde kesinlikle sim/glitter ifadeleri yer almaz; yalnızca kristal strass taş baskı, metraj rulo kumaşa baskı, 3.20m geniş en kapasitesi, yıkama/dökülmeme garantisi ve ücretsiz numune vurgulanır.
  3. **Çift Formatlı Hareketli Grafik (ProRes 4444 MOV + MP4):** Premiere Pro'da sıfır ayarla doğrudan şeffaf oynatım için 10-bit alfa kanallı ProRes 4444 (.mov) standartlaştırıldı; hafif önizlemeler için de (.mp4) eşlik etti.

## 9 Kasım 2026 — Taşlı Şal Kadın Model Üretiminde Gerçek Çıktı Standardı
- **Bulgu & Analiz:** İndirilenler klasöründeki başarılı Gemini çıktılarında (11 görsel), modellerin elinde porselen fincan/nane çayı bardağı tutması, mermer kafe masaları ve nötr fonlar (fildişi/bej trençkot ve bluzlar) ile koyu renk mat kumaş (gece mavisi, bordo, zümrüt, espresso, füme) zıtlığının taş netliğini telefon ekranında katbekat artırdığı teyit edildi.
- **Kural:** 42 modelin tamamı için 21 başa sarılan ve 21 omuza alınan dengesi korunarak, her bir modelin mekan, yaş (21-28), ten/saç ve kıyafet detayları tekil olarak kurgulandı (promptlar/42_tasli_sal_kadin_manken_ozel_promptlari.md).

# Öğrenilenler ve hatalardan çıkan dersler

Her işte yapılan hata, sebebi ve bundan sonraki kural burada tutulur. En yeni üstte.

## 8 Kasım 2026 — Taş Baskı Şal/Tarha Promptlarında "Bordür Uydurma" ve "Kısmi Kapsama" Hatası
- **Hata:** Şal (tarha) promptunda (`Model 4 - 2.jpg`) model görsel üretirken desende olmayan harici çiçek/çerçeve süslemeleri uydurmuş ve taş desenini şalın tamamına değil yalnızca göğüs kenarına uygulamıştı.
- **Sebep:** Prompt metninde `stone-embellished border flowing across her chest` ifadesinin kullanılması, yapay zekanın (Midjourney/Flux/Gemini) deseni sadece bordüre hapsetmesine ve referansta olmayan bordür motifleri halüsinasyon etmesine yol açtı.
- **Kural (Taş Baskı Şal Prompt Standartı):**
  1. **Kesintisiz Tam Kapsama (`100% All-Over Seamless Coverage`):** Promptta mutlaka `The pattern must cover the ENTIRE surface area of the shawl from edge to edge continuously, including the headwrap, all folded layers, the draped ends, and the back. Zero unadorned blank sections, zero plain fabric patches.` kuralı yazılmalıdır.
  2. **Bordür Yasağı ve Sıfır Halüsinasyon (`Strict Motif Adherence`):** Referans kartelada açıkça bir bordür yoksa asla `border` veya `trim` kelimesi kullanılmaz; `STRICT MOTIF ADHERENCE: Replicate ONLY the motifs visible in the reference. Do NOT invent, hallucinate, or add any borders, frames, lace, floral trims, or extra shapes that are not in the reference.` kuralı kilitlenir.

## 7 Kasım 2026 — Meta Business Suite PDF Yükleme Süresi ve Asenkron Gönder Tuzağı
- **Hata:** Messenger yanıtlarında metin gittikten sonra PDF ekleme aracına dosya verildiğinde, 8.01 MiB'lık dosyanın Meta sunucularına yüklenmesi (progressbar) yaklaşık 4-6 saniye sürmesine rağmen Gönder butonuna hemen tıklanmıştı. Gönder butonu dosya tamamen hazır olmadan devre dışı (disabled) kaldığı için tıklama işlemi başarısız olmuş ve müşterilere yalnızca metin iletilmişti. Ayrıca sol listedeki "Sen: أهلاً..." önizlemesi mesajın gittiğini gösterdiği için yanıltıcı şekilde işlem başarılı sanılmıştı.
- **Sebep:** Meta Business Suite mesaj kutusunda büyük boyutlu PDF eklendiğinde `div[role="progressbar"]` elementinin yok olması ve Gönder butonunun `disabled` halden çıkıp tıklanabilir siyah renge dönmesi beklenmeden gönderim tetiklenmesi.
- **Kural (İstisnasız Yeni Doğrulama Standartı):**
  1. PDF yüklendikten sonra mutlaka `progressbar` elementinin kaybolduğu ve Gönder butonunun `aria-disabled="false"` olduğu DOM üzerinden beklenmelidir.
  2. Gönder butonuna tıklandıktan sonra sol listedeki metin önizlemesiyle **asla yetinilmez**; sağ paneldeki mesaj balonlarında `Dosya Ekini Aç, kartelas 1 - fiyatlı.pdf, 8,01 MiB` elementi açıkça belirmeden bir sonraki müşteriye geçilmez.

## 7 Kasım 2026 — Otomatik Kedihane Yönetimi ve Çift Repo Oturum Başlangıcı
- **Kullanıcı Kararı / Yeni Standart:** Bu projede açılan her yeni sohbette kullanıcının her defasında çalışma şeklini anlatmasına veya `"ekip:"` yazmasına gerek yoktur. Her yeni sohbet otomatik olarak `kedihane` (`c:\Users\dell\.gemini\antigravity\scratch\kedihane`) yönetiminde (Tekir şefliğinde) başlar ve `AB-Aycam-SosyalMedyaYonetimi` (`E:\ab ayçam\AB-Aycam-SosyalMedyaYonetimi` & `E:\ab ayçam\github-guncelleme`) reposunu yönetir.
- **Kalıcı Mekanizma:** `Kedihane+AB_Ayçam_Sosyalmedya` proje yapılandırmasına her iki git klasörü bağlandı; `session-start.ps1` kancası, `.agents/learnings/PROJECT.md`, `AGENTS.md`, `GEMINI.md` ve `PROJE_INSTRUCTIONS_GUNCEL.md` dosyaları bu kuralı her oturum başında otomatik uygulayacak şekilde eşitlendi.

## 3 Kasım 2026 — Mesaj/Yorum Raporlama ve Ön Onay Tablo Standardı (Gerçek Zamanlı İsim Hitabı)
- **Kullanıcı Kararı / Yeni Standart:** Gelen yorum ve mesajlar raporlanırken (kullanıcı açıkça sormasa dahi veya gelen soru/yorumlar incelendiğinde) daima aşağıdaki 5 sütunlu tam tablo formatı kullanılmalıdır:
  `| # | Mesajdan/Yorumdan Gelen Soru (Arapça) | Sorunun Türkçe Anlamı | Hazırlanan Cevap (Arapça) | Cevabın Türkçe Anlamı & Eklenti |`
- **{ISIM} Yerine Gerçek Zamanlı Müşteri Adı Zorunluluğu:** Hazırlanan cevabın hem Arapça metninde (`أهلاً {ISIM} 👋...`) hem de Türkçe açıklamasında (`"Merhaba {ISIM} 👋..."`), `{ISIM}` şablon değişkeni yerine **mesajı atan veya yorumu yapan kişinin gerçek profil adı canlı olarak doldurulmalıdır**.
- **Katalog Eki Belirteci:** Cevabın Türkçe sütununda eklenecek PDF (`📎 Ek: kartelas 1 - fiyatlı.pdf`) açıkça belirtilmelidir.
- **Kullanıcı Onayı Bekleme:** Bu tablo sunulduktan sonra kullanıcı "cevapları verebilirsin / onayla / gönder" demeden tek bir mesaj dahi gönderilmez.

## 2 Kasım 2026 — PDF Dosya Yolu Teyidi ve Tarayıcı MCP Yükleme Standardı
- **Hata / Ders (PDF Yolu Teyidi):** Sosyal medya yanıtlarında veya tarayıcı otomasyonunda gönderilecek PDF dosyası hafızadan/tahminle (`tüm kalıplar.pdf` vb.) seçilemez; daima `PROJE_INSTRUCTIONS_GUNCEL.md` içindeki tek yetkili güncel dosya olan `E:\ab ayçam\kartela görüntüsü\kartelas 1 - fiyatlı.pdf` (8,01 MiB) esas alınmalıdır.
- **Teknik Ders (Chrome DevTools MCP upload_file Kısıtı):** Chrome DevTools MCP sunucusu güvenlik gereği yalnızca `os.tmpdir()` (`C:\Users\dell\AppData\Local\Temp\`) dizinini varsayılan geçerli kök kabul eder. E: sürücüsündeki dosyalar doğrudan yüklenemez; yükleme öncesinde dosya geçici olarak Temp dizinine kopyalanıp oradan `upload_file` edilmelidir.

## 2 Kasım 2026 — Messenger Toplu Cevap Turu (Eksik PDF Düzeltmesi & Onay Doğrulaması Kapısı)
- **Hata / Eksiklik:** Cumartesi günü yanıtlanan mesajlarda ("كل موديلاتنا موجودة في الملف المرفق (PDF) 📎 اختار اللي يعجبك...") metin iletilmesine rağmen müşterilere katalog PDF dosyası (`kartelas 1 - fiyatlı.pdf`) ek olarak yüklenmemişti; yalnızca wa.me bağlantı önizlemesi gitmişti.
- **Düzeltme & Çözüm:** Kullanıcı onayıyla 8 müşterinin (`Khaled El Kady`, `Dada Dada`, `Gab Reyal`, `Mone Mone`, `Doaa Sami`, `محمد ابوراس`, `سيد ربيع`, `Macheal Abdo`) sohbetleri tek tek açılarak her birine `kartelas 1 - fiyatlı.pdf` (8,01 MiB) dosyası yüklendi, progressbar ve Gönder butonu aktifliği beklenip native click ile iletildi. Her bir konuşmada dosya balonu ve sol listedeki önizleme doğrulanarak eksiklik %100 giderildi.
- **Yeni Kural (İstisnasız İki Aşamalı Onay ve Tekil Doğrulama Kapısı):**
  1. **Ön Onay Zorunluluğu:** Hiçbir müşteriye (Messenger veya yorum) doğrudan ve habersiz yanıt gönderilmez. Önce yöneticiye Türkçe onay tablosu sunulur; kullanıcı "onay / gönder" demeden gönderim başlamaz.
  2. **Hiçbir İnsan Onay Doğrulaması Olmadan Geçilemez:** Her müşteriye mesaj/dosya iletildikten sonra:
     - Sağ panel başlığının müşteriyle eşleştiği,
     - Dosya yüklenmişse progressbar'ın bitip Gönder butonunun aktif siyah renge döndüğü,
     - Gönderim sonrası mesaj balonunda dosya ve sol listede *"Bir dosya eki gönderdin."* önizlemesinin belirdiği DOM üzerinden tek tek doğrulanmadan **asla bir sonraki kişiye geçilemez ve işlem tamamlandı sayılamaz**.
  3. **Tur Sonu Raporu:** Toplu cevap turlarında her müşterinin doğrulama durumu kullanıcıya eksiksiz raporlanır.

## 1 Kasım 2026 — Video 23 (17T Kurgu: Küçük PiP Yasağı, Tam-Sayı Crop Titremesi, DisplayMatrix ve Orijinal Bayrak Şablonu)
- **Hata 1 (Küçük Görseller ve Taşların Belli Olmaması):** Videonun içine küçük Picture-in-Picture (`370x520` PiP) kutuları, dar dikey ekran bölmeleri (`split-screen`) ve 4'lü küçük ızgaralar konulduğunda kıyafet üzerindeki strass/taş işlemeleri 1 piksellik noktalara dönüşerek hiç belli olmadı. Ayrıca `1792x2400` (`3:4`) katalog görselleri doğrudan `1080x1920` (`9:16`) boyuta ölçeklenince mankenler dikeyde %33 sündürüldü.
  - **Kural:** Taş (strass) ve sim detaylı model görsellerinde **asla küçük PiP kutusu, dar ekran bölmesi veya 4'lü küçük ızgara kullanılmaz**. Görseller (`1792x2400`), **sıfır sündürme (`1:1` gerçek piksel oranı)** ile doğrudan giysi ve taş işlemelerine odaklanan `9:16` pencereden (`1170x2080` veya `1260x2240` → `1080x1920` Lanczos) **tam ekran** kadrajlanır ve kristal taş fasetlerini belirginleştirmek için `UnsharpMask` uygulanır.
- **Hata 2 (Görsellerde Takıla Takıla Geçiş ve Göz Yorgunluğu):** Sabit görsellere FFmpeg'de `crop=1080:1920:'60+20*(t/dur)'` gibi zamana bağlı kaydırma ifadesi verildiğinde, `crop` filtresi koordinatları tam sayıya (integer piksel) yuvarladığı için görüntü 5 kare sabit kalıp 6. karede `1 piksel` sıçrayarak (`takıla takıla`) ilerledi ve gözü rahatsız etti. Ayrıca `0.25 sn` gibi kısa sürede `slideleft` / `slideright` / `wipe` / `circleopen` geçişleri kullanılması göz yorgunluğu yarattı.
  - **Kural:** Görsellerde FFmpeg `crop` ile yapay pan/zoom **kesinlikle kullanılmaz**; model portreleri **%100 sabit ve titremesiz** tutularak izleyicinin taş detaylarına rahatça odaklanması sağlanır. Sahne geçişlerinde sert kayma/silme yerine yalnızca müzik ritmine kilitli **`0.40 sn` yumuşak optik erime (`xfade=transition=fade`)** (bitiş kartlarında `fadeblack`) kullanılır.
- **Hata 3 (4K Dikey Videolarda `-noautorotate` ve `displaymatrix` Tuzağı):** `3840x2160` (`displaymatrix: rotation of -90.00 degrees`) dikey telefon videolarında `-noautorotate` kullanıldığında görüntü yatay kalıp `1080x1920`'ye basılarak ezildi; `-noautorotate` kaldırıldığında ise FFmpeg `filter_complex` çıkışındaki bazı MP4 segmentlerine kaynak videonun `-90 derece` `displaymatrix` etiketini kopyaladığı için `xfade` aşamasında `1080x1920 vs 1920x1080` boyut uyuşmazlığı oluştu.
  - **Kural:** Dikey telefon videoları işlenirken `-noautorotate` kullanılmaz; üretilen ara segmentlerdeki olası `displaymatrix` kalıntısı `ffmpeg -display_rotation 0 -i seg.mp4 -c copy` ile temizlendikten sonra `xfade` birleştirmesine sokulur.
- **Hata 4 (Bayrak Şablonunda Beyaz Kenar Boyama Yasağı & Nokta Atışı Segment Güncelleme):** Türk bayrağı dairesinin alt/üst beyaz boşluklarını yok etmek için bayrağı büyütmek yerine beyaz kısımların kırmızıya boyanması yamalı/çizgili kötü bir görüntü oluşturdu.
  - **Kural:** Bayrak sahnesi her zaman `E:\ab ayçam\premiere pro\17 - whatsaptan gelen videolar\video-tasarimlari\bayrak-sablon` içindeki orijinal `01_bayrak_sablonu_seffaf.png`, `02_bayrak_sablonu_koyu_zemin.png`, `images (1).png` (Türk bayrağı) ve `images.png` (Mısır bayrağı) dosyalarından üretilir. Bayrak asla elle boyanmaz; doğrudan daire yüksekliğini (`380 px`) tam dolduracak şekilde Lanczos ile büyütülür ve hilal-yıldız daire içinde ortalanır (`shift_x=-46`). Videoda yalnızca tek bir sahne düzeltilecekse tüm video baştan render edilmez; sadece ilgili segment (`seg_16.mp4`) güncellenip birleştirilir.

## 31 Ekim 2026 — Antigravity / Chrome-DevTools MCP ile dosya yükleme (Windows)
- **Ders (teknik):** Antigravity Windows ortamında `chrome-devtools` MCP server'ı yerel Windows dosya yollarında `Access denied: path ... is not within any of the configured workspace roots` hatası verir. MCP Context kodu incelendiğinde, istemci roots belirtmese dahi `os.tmpdir()` (`C:\Users\<user>\AppData\Local\Temp\`) dizininin her zaman varsayılan izinli kök (allowed root) olarak kabul edildiği tespit edildi.
- **Kural:** Antigravity ile tarayıcıda dosya yüklerken (PDF vb.) dosya önce `C:\Users\<user>\AppData\Local\Temp\` dizinine kopyalanır, ardından `upload_file` aracına bu geçici yol verilir. Dosya yüklemesi %100 başarıyla gerçekleşir.
- **Ders (teknik):** Meta Business Suite mesaj kutusunda (Lexical editor) doğrudan metin yapıştırma bazen kopyalamayı tekrarlayabilir veya yutabilir. En temiz yöntem: kutuya `paste` olayı ile metni bırakıp ardından snapshot'tan metnin tekil olduğunu doğruladıktan sonra `press_key` ile `Enter` göndermektir.

## 24 Ekim 2026 — Video 22 (Türk bayrağı dairesinde alt/üst beyaz boşluk hatası)
- **Hata:** Bayrak şablonunda Türk bayrağı (`images (1).png`) daire içine yerleştirilirken dairenin alt ve üst kısmında beyaz boşluklar (kenarlık) kaldı.
- **Sebep:** Kaynak `images (1).png` dosyası kare (`225x225`) bir tuval içinde yatay dikdörtgen bayrak olduğu için kendi içinde üstte ve altta geniş beyaz boşluklar barındırıyor. Resmi doğrudan daire çapına (`d_px`) ölçekleyince bu beyaz boşluklar dairenin içine girdi.
- **Kural (İstisnasız):** Herhangi bir bayrak veya görseli dairesel/çerçeveli yuvaya yerleştirmeden önce mutlaka dışındaki beyaz/şeffaf kenar boşluklarını (padding/letterbox) otomatik kırp (`autocrop` / sadece kırmızı bayrak alanını `getbbox` ile al), ardından **kırpılmış bayrak yüksekliği daire çapını (`d_px`) tamamen dolduracak ve taşacak şekilde** (`scale = d_px / cropped_height`) büyüt. Daire içinde asla beyaz zemin/boşluk kalmamalı.

## 24 Ekim 2026 — Video 22 (emoji glifi ve Windows ffmpeg)
- **Hata:** Alt yazı üst rozetinde (`العينات مجاناً 🎁`) emoji kullanıldığında Cairo fontunda emoji glifi olmadığı için kutu (`[]`) çıktı; ön izleme sayfasında yakalanıp emoji kaldırıldı. **Kural:** Pillow + Cairo ile üretilen PNG şablonlarda asla emoji kullanma; yalnızca Arapça/Latin harf ve yıldız/elmas vektör çizimleri kullan.
- **Ders (teknik):** Windows'ta CapCut içindeki `ffmpeg.exe` kısıtlı bir derlemedir (`-crf` parametresini tanımaz). Tam özellikli `libx264` + `xfade` render'ı için `uv run --with imageio-ffmpeg` içindeki `ffmpeg-win-x86_64-v7.1.exe` kullanılır.

## 24 Ekim 2026 — Video 21 (rakam kenarı tırtıklı)
- **Hata:** Telefon numarasının (0373) rakamları Cairo latin fontuyla doğrudan 1x/2x çizilince kenarlar tırtıklı çıktı. **Kural:** Şablonlar 4x çizilip LANCZOS ile küçültülür (`_kaynak\build21_hq.py`); tek tek `gen21.py 1|2` çalıştırma.

## 24 Ekim 2026 — Video 21 (Windows'ta Pillow Arapça harf birleştirme / Cairo fontu)
- **Ders (teknik):** Windows'taki standart Pillow kurulumunda `libraqm` yoktur (`features.check('raqm') == False`). `arabic_reshaper` varsayılan ayarla kullanıldığında ayrık (isolated) harfleri `0xFE8D` (`ا`), `0xFEB1` (`س`) gibi Presentation Forms-B kodlarına çevirir; ancak `@fontsource/cairo` alt küme fontlarında (`cairo-arabic-*.ttf`) ayrık harfler `0x06xx` taban Unicode kodlarında tutulur ve `0xFE8D` kutu (`[]`) olarak çıkar. Ayrıca tenvin (`ً`, `0x064B`) Cairo'da `مجاناً` kelimesinde çift çizgi taşması yapar.
- **Kural:** Windows'ta `cairo-arabic-*.ttf` ile üretim yaparken `arabic_reshaper.ArabicReshaper({'use_unshaped_instead_of_isolated': True, 'delete_harakat': True})` + `bidi.algorithm.get_display` kullanılır; üretim sonrası `fontTools` `cmap` kontrolü ve gri zeminde kontak sayfası ile eksik/taşan glif olmadığı doğrulanır.

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


## 21.10.2026 – Sim glitter promptları
- Hata: modeller 30-50 yaş yazıldı, Gemini 2. promptta yaşlı kadın üretti; sim yıldız/disk boyutu büyük çıktı. Kural: sim görsellerinde genellikle genç kadın (20'li yaşlar) yaz; sim boyutunu "çoğu 1-2 mm, 3-4 mm nadir, emin değilsen küçük" diye yaz.
- Hata: "wrap" yazınca Gemini şalı robe/ceket gibi üretti. Kural: sim görsellerinde "rectangular long shawl draped over shoulders, both ends hanging, NOT a jacket/robe/kimono, no sleeves" (omuzda) veya "shawl wrapped as a hijab" (başta) yaz; elbise/metrajlık sahne kullanma.

## 24 Ekim 2026 (Otomatik PDF Gönderimi ve Çoklu Ek Hatası)
- **Hata:** Döngü sol listede konuşma geçişini doğrulamadan Ctrl+V tetiklediği için aynı kişiye 4 adet PDF üst üste eklendi.
- **Sebep:** Business Suite liste tıklamasının konuşma başlığını (header) değiştirdiği beklenmeden ve ek kutusunda zaten dosya olup olmadığı kontrol edilmeden yapıştırma tetiklendi.
- **Yeni Kural:**
  1. Sol listeden kişiye tıklandıktan sonra üst başlıktaki (header) isim değişene kadar beklenir.
  2. Gönderimden önce konuşma geçmişinde veya ek kutusunda kartelas 1 - fiyatlı.pdf var mı kesinlikle kontrol edilir. Varsa ASLA tekrar PDF yapıştırılmaz.
  3. Metin ayrı, dosya ayrı gönderilir; ek yükleme kutusunda birden fazla çip varsa iptal edilip tek bir dosyaya düşürülür.
