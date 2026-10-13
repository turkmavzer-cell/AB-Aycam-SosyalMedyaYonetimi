# AB Ayçam – Tam Proje Context (Claude için kalıcı çalışma notu)

Son güncelleme: 13 Ekim 2026. Bu dosya projedeki tüm sohbetlerin birleşik özetidir (video üretim, taşlı yapay zeka görselleri, Premiere/kurgu, Meta mesaj/yorum yönetimi, ev tekstili ürün görselleri, TikTok, GitHub kayıt sistemi). Eski sürümlerin (`AB_Aycam_Proje_Context.md`, `AB_Aycam_Is_Akisi_Raporu.md`, 8 Ekim tarihli TAM) yerine bu dosyayı kullan.

> Not: Eski sohbetlerin bazı kısımları yalnızca son mesajlar üzerinden görülebildi. Emin olunmayan yerler "(doğrulanmadı)" ile işaretli.

Bu repo bir sohbete başlarken ilk okunacak yerdir. Okuma sırası: `README.md` → bu dosya → `ilerleme.md` → `bekleyen-isler.md` → ilgili `is-akislari/*.md` → gerekirse `promptlar/*.md`.

---

## 1. İşletme ve temel kurallar

- **AB Ayçam**: iki iş kolu. (1) Metraj kumaş üzerine taş/strass (hotfix, rhinestone) baskı; müşteri kumaşını getirir, kumaş satışı yok (ya da kararsız). (2) **Ev tekstili taş baskı ürünleri** (masa örtüsü seti; aşağıda bölüm 4).
- **Pazar:** Mısır (sıcak iklim). Türkiye bağlantılı "Türk kalitesi" mesajı kullanılır.
- **Adres:** العبور (Obour) · القليوبية · المنطقة الصناعية B&C · قطعة 7 · بلوك 27003 · الدور الثالث.
- **Telefonlar:** +20 106 895 6909 · +90 532 058 8023 · +20 106 683 0373 (WhatsApp). WhatsApp linki: https://wa.me/201066830373
- **Ana mesajlar:** Türk kalitesi · Mısır içinde üretim · metrajla baskı · 37+ farklı desen · ithalat, kargo ve bekleme yok · "ابعت لنا القماش بتاعك، وإحنا هنتولى التنفيذ بأعلى جودة".
- **Hedef kitle:** fabrikalar, tüccarlar, marka sahipleri (günlük giyim, tesettür, lingerie/gecelik).
- **Logo:** `E:\ab ayçam\logo png.png` (ayrıca `logo jpeg.jpg`, `logo png 2.png`, `AB AYÇAM.png`).
- **Dil:** İçerik (video, afiş, mesaj, müşteri cevapları) Arapça, Mısır lehçesi. Kullanıcıyla iletişim Türkçe.
- **Sosyal hesaplar:** Facebook sayfası "AB İstanbul dijital & Taş baskı" (Meta Business Suite ile yönetilir). TikTok şirket hesabı: @toqa7808 ("AB AYÇAM طباعة أستراس بالمتر", giriş bilgisi kayıp, bkz. `is-akislari/tiktok-hesap-kurtarma.md`).

### Kullanıcı tercihleri (her zaman uygula)
1. Soruya önce doğrudan cevap ver; istenmeyen işe başlama. Büyük işte önce plan sun, onay al.
2. Kısa ve net yaz. Gereksiz biçimlendirme yok.
3. Görsel/video içeriğini gerçekten incele (birden fazla kare); bozuk içeriği kullanma.
4. Altyazı/yazı sesle **birebir aynı** olmalı (özet yok).
5. Yazı ve efektler izleyiciyi yormamalı, profesyonel görünmeli.
6. Fotoğraf sahnelerinde arka plan düz renk olmasın; hareketli foto/video olsun.
7. Kullanıcının kendi düzenlediği dosyalara dokunma.
8. Şifre, doğrulama kodu girme; ödeme/kredi harcayan işlemlerde önce onay al; indirme için onay iste. Gönderme, silme, reklam seti ve otomasyon değişikliği sadece onayla.
9. Yapabildiğini ve sınırını dürüstçe söyle (ör. video izleyemem, ses dinleyemem; Premiere'de elle çizim kalitesi yok vb.).
10. Mısır pazarı için sıcak iklim: kış parçaları, kar, yün palto gibi sahne/kıyafet kullanma (taşlı giydirme promptlarında). Ev tekstili kar setinde ürünün kendisi kar desenidir, sahne ise sıcak/ev içi kalır.
11. **Fiyat ve model çeşitliliği bilgisi sadece WhatsApp'tan verilir.** Müşteriye WhatsApp'a yönlendirirken wa.me linki mutlaka konur; telefon numarası yazı olarak yazılmaz (Arapça metinde ters görünür).
12. **GitHub kayıt kuralı:** Yapılan her işin sonunda bu repodaki ilgili md dosyası ve `ilerleme.md` güncellenir. Kullanıcının "oldu / onay" dediği promptlar kelimesi kelimesine `promptlar/` klasörüne yazılır. Repoya şifre, token, müşteri adı ve mesaj içeriği yazılmaz. Repo özel (private) olmalıdır.

---

## 2. Klasör haritası (`E:\ab ayçam`)

| Yol | İçerik |
|---|---|
| `AB-Aycam-SosyalMedyaYonetimi\` | Bu GitHub reposunun yerel klonu (GitHub Desktop ile) |
| `taşlı yapay zeka\` | Gemini prompt dosyaları (v2–v14), `makina 2\kartela\jpeg` (kartela desen görselleri), `1`–`4`, `_work`, `Yeni klasör` |
| `taşlı yapay zeka\makina 2\kartela\jpeg` | Taş deseni referans görselleri (siyah zeminli, 1.jpg … 44; "copy" ekli adlar da var) |
| `taşlı yapay zeka\Ev Textili\` | Ev tekstili ürün fotoğrafları: kar, yıldız, çiçek × büyük, küçük, uzun (.jpg, her biri ~14 MB; Gemini'ye yüklemeden önce ~2000 px'e küçültmek hızlandırır) |
| `premiere pro\1`–`13` | Eski Premiere projeleri, videolar (6 +, 7 +, 8 +, 9 + vb. işaretli klasörler) |
| `premiere pro\14 lenceri\videolar` | Lingerie videoları (kolaj kurgusunun kaynağı) |
| `premiere pro\15` | Seslendirmeler, 6 yeni video, `Photos-1-001` (42 kumaş/makine klibi), `_kurgu_kodu` |
| `premiere pro\16\lenceri` | ~72 lingerie görseli (1792x2400) |
| `premiere pro\16\günlük` | 22 günlük giyim görseli (1–22) |
| `premiere pro\müzikler` | 16 şarkı mp3 |
| `premiere pro\vektor` | Paisley vektör çıktıları |
| `GITHUB AKTARIM TALIMATI.md` | Geçmiş işleri repoya aktarmak için hazırlanmış talimat |
| Kök | Kartela PDF/TIF/PSD/AI, kart vizit, fuar kataloğu, tabela, billboard tasarım, logo dosyaları, "tüm kalıplar", "tüm kumaşlar" görselleri |

---

## 3. Taşlı yapay zeka görselleri (Gemini / Nano Banana) – giydirme ve konsept

### Amaç
Kartela taş desenlerini (siyah zeminli referans görsel) AI ile üretilen kadın kıyafetlerinin üstüne işlemek; sosyal medya, katalog ve reklamda kullanmak.

### Ana sorun ve yaklaşım
- Üretimlerin yalnızca ~1/5–2/5'i kullanılabilir çıkıyor: taş deseni bozuluyor ya da taş olduğu anlaşılmıyor. Hedef: en az 2 üretimde 1 kullanılabilir sonuç.
- Önerilen çözüm planı: **iki aşamalı** – (1) AI yalnızca düz renkli kıyafet ve manken üretir; (2) gerçek kartela deseni kıvrımlara göre bilgisayarla/Photoshop'ta bindirilir; yedek: Nano Banana Pro / Flux Kontext ile bölgesel iyileştirme. (Test sonucu bilinmiyor – doğrulanmadı.)
- Fiilen kullanılan yöntem: Gemini'ye desen görselini yükleyip desene özel prompt yapıştırmak (v7+). Düz kıyafet promptları da var (Photoshop'ta taş eklemek için).
- Gemini aynı sohbette önceki görseli tekrar etme eğiliminde; yeni sahne için temiz sohbet veya net "yeni görsel" talimatı gerekir.

### Prompt dosyaları
Tam metinler: `promptlar/arsiv-gemini-giydirme/` (yerelde `taşlı yapay zeka\`). v8 bilerek repoya alınmadı.

| Dosya | Açıklama |
|---|---|
| düz kıyafetli mankenler | Desensiz düz kumaş (Photoshop'ta taş eklemek için) |
| v2 hareketli pozlar · v3 lingerie cüretkar · v4 lingerie tarzı elbise · v5 ev içi saten tül lingerie | İlk denemeler |
| v6 50 adet lingerie · v7 taşlı desen referanslı 50 adet | Desen referanslı lingerie seti |
| v8 42 desene özel | **Kullanma.** Çocuk ve lingerie içeriyordu; kullanıcı sadece yetişkin istedi |
| v9 42 desene özel | 21 tesettürlü + 21 tesettürsüz mütevazı yetişkin kombin (çocuk/lingerie yok) |
| v10 ev içi cüretkar 42 desene özel | Cüretkar kesimli lingerie/saten (bkz. kurallar) |
| v11 27–44 eli saçta olmayan pozlar | v10'dan elin saça dokunmadığı pozlar |
| v12 günlük ev içi ve dış mekan 12–44 | Günlük kıyafet (iç/dış mekan); desen 12–44 |
| v13 ev tekstili kar seti 3 konsept | **Reddedildi** (kumaş rengi değişti, oda sahnesi, üstten değil). Bkz. bölüm 4 |
| v14 ev tekstili kar seti üstten kolaj 3 konsept | Gemini aynı görseli üretti; kullanıcı konsept yerine model başına prompt istedi. Bkz. bölüm 4 |

Desen numaraları kartela klasöründeki dosya adlarıyla eşleşir; her prompt için önce ilgili desen görseli Gemini'ye yüklenir.

### Prompt yapısı (standart blok – giydirme promptlarında var)
Referans görsel siyah zeminli taş deseni; **siyah zemin desene dahil değil**, yalnızca taşlar ve motif düzeni kullanılır, ölçek/aralık korunur ve doğal tekrar edilir. Taşlar kumaş kıvrımını izler; cilde, saça, ele, çantaya ve arka plana geçmez; tülde renkli tül taşların arasında görünür. Her taş ~3 mm faceted kristal, küçük temas gölgesi, gölgede hafif sönük, ışıkta keskin parlama. Taban kumaş düz renk, başka baskı/logo/yazı/dantel yok. 3:4 dikey, 4K, gerçekçi cilt ve eller.

### Öğrenilen kurallar
- **Yetişkin kadın modeller.** Çocuk/genç kız içeriği yok (v8'de çıkan çocuk görseli sorun oldu).
- **Tesettürlü:** çok parçalı kombin (ceket, tunik, pantolon, kimono, yelek, hırka, pelerin + başörtüsü); tek parça elbise/ferace yok.
- **Tesettürsüz günlük:** mütevazı, kapalı, dekolte/yırtmaç yok.
- **Lingerie:** başta dekolte/cüretkarlık istenmemişti; **sonra cüretkar olabilir** denildi (derin V, bel/göğüs kesiği, yırtmaç). Kural: **opak astar, iç çamaşırı görünmez, çıplaklık yok.** Gemini reddederse "luxury loungewear / evening nightwear catalog" ifadesini koru, "sultry" yerine "confident" yaz.
- **Desen adı sahneyi etkiler:** "kar tanesi" yazınca Gemini kar sahnesi üretti. Motifi "kristal yıldız kümesi" gibi tarif et ve "kar/kış/soğuk yok, sıcak güneşli iklim" ekle. Benzer riskli desenler: yıldız, kalp, Paris kulesi, ayıcık, kediler.
- **Mısır sahneleri:** Nil corniche, Kahire sokakları, sıcak taş binalar, palmiyeler.
- **Model tipleri:** kullanıcı örn. "kızıl, açık tenli, hafif çilli, 20'li yaşlar" tarifi verdi. Renk seçimi desenle kontrast yapacak tonlardan (zümrüt, bordo, lacivert, ruby, plum vb.).
- Taşlar zayıfsa: "make the stones larger and more prominent"; yoğunluk için "spaced about 1 cm apart".
- Üretilen sonuçlar `1792x2400` ve 3:4. Kullanıcı tüm görselleri kendisi Gemini'de üretiyor.

### Video dönüşümü (görselden videoya) araştırması
- Kullanıcı üretilen fotoğrafları videoya çevirecek; **Pollo AI üyeliği almayı planlıyor**. Higgsfield, Pollo AI ve SuperGrok kıyaslandı: Pollo çok modelli ve ucuz deneme; Higgsfield kamera şablonları; SuperGrok Lite 480p ile sınırlı (taş detayı kaybolur).
- Pollo modelleri: Wan 3.0 (1080p, Unlimited Free), MiniMax H3 (2K, Unlimited Free), Seedance 2.0 (4K, ~9 kredi), Seedance 2.5 (1080p), Seedance 2.0 Mini (720p), Pollo 3.0 (480p, 10 kredi). Öneri: Wan 3.0 ve MiniMax H3'ü ücretsiz dene, tek Seedance 2.0 ile karşılaştır; dikey 9:16, 5 sn.
- Taş koruma video promptu: yavaş ve doğal hareket, yavaş push-in, "taşları değiştirme/bulanıklaştırma/yeniden çizme", yüz ve kıyafet aynı kalsın, kesme yok.
- Higgsfield erişimi: Claude için bağlayıcı yok; uygulama tarayıcısıyla arayüz kullanılabilir (giriş kullanıcıdan, kredi/indirme onayı gerekli, CAPTCHA'yı geçemez).

---

## 4. Ev tekstili taş baskı ürünleri ve ürün görselleri (Gemini / Nano Banana)

Ayrıntı ve adım adım yöntem: `is-akislari/ev-tekstili-urun-gorselleri.md`. Onaylı promptlar: `promptlar/ev-tekstili-*.md`.

- **Ürün hattı:** 5 farklı model, her modelin 3 boyutu: 75x75 cm büyük kare, 45x45 cm küçük kare (tabak altlığı), uzun parça (tencere altlığı; hafızada 45x100 cm, sahne promptunda yaklaşık 28x70 cm kullanıldı; **gerçek ölçü teyit bekliyor**). Uzun parçanın uçları sivri, altıgen kesimlidir. Kumaş krem/fildişi, taşlar gümüş kristal.
- **Çalışılan setler:** kar, yıldız, çiçek (klasörde kar/yıldız/çiçek × büyük/küçük/uzun). Çiçek seti ile ilerleniyor. Kar: ortada altı kollu büyük kar tanesi, küçük sekiz kollu kar taneleri, basamaklı geometrik köşe çerçeveleri. Yıldız: iç içe konsantrik anahat yıldız, çok sayıda küçük yıldız, bükümlü şerit kenar ve dört yapraklı çiçekler. Çiçek: haç düzeninde dört paisley-çiçek madalyon, köşelerde yaprak kümeleri ve çiçek dalları, baklava dilimli kenar.
- **Sunum kuralları:** Kumaş rengi değişmez. Üstten görünüm. Yerleşim kullanıcının çizdiği düzen: büyük parça uzun masanın ortasında çapraz (elmas), küçük parçalar masa uçlarında düz ve ortalı simetrik, uzun parça sağ üst boş alanda düz. Küçük parçalar masa genişliğinin ~%40'ı olacak şekilde küçük çizilmeli (Gemini büyük çiziyor, orana vurgu gerekiyor). Sade, aksesuar az, desen üzerine bir şey konmaz. Görsel 3:4 dikey (telefondan PDF katalog); yapılmayan desen gösterilmez.
- **Gemini'ye yükleme sırası:** 1 = onaylı sahne görseli (yerleşim referansı), 2 = çiçek büyük, 3 = çiçek küçük, 4 = çiçek uzun.
- **Konsept kararı (Mısır'da satış için):** Ev içi, doğal, sıcak (zeytin ağacı masa, hasır sandalye, kilim, keten perde) onaylandı. Ramazan iftar sofrası (koyu ceviz, fener, hurma) beğenildi, yedek. Nil kenarı terası beğenilmedi. Eski Kahire konsepti denenmedi.
- **Durum:** Onaylı sahne üretildi; 3 detay promptu yazıldı (tabak altlığı, büyük parça merkezi, kumaş köşe makro), detay görselleri üretimi bekliyor.

---

## 5. Video işleri

### 5.1 Kullanılan teknikler
- **Premiere Pro:** `premiere pro\*` klasörlerinde birçok proje. Claude, bilgisayar kontrolüyle Premiere'i kullanabiliyor; XML aktarımında logo/yazı konumu ve font bozulabiliyor.
- **Kodla video üretimi (Python + PIL + numpy + opencv + ffmpeg):** 6 yeni video bu yöntemle yapıldı. Kod: `premiere pro\15\_kurgu_kodu\`.
- Claude videoyu izleyemez/sesi dinleyemez; kare çıkararak inceler ve ses seviyesi/sessizliği ölçer.

### 5.2 Geçmiş video işleri
1. **Kolaj videosu (14 lenceri\videolar):** Her ~10 sn'de işi anlatan Arapça bilgi yazıları olan kurgu istendi; bir sohbette Claude Code abonelik hatası yüzünden ilerlemedi.
2. **"Şık ve eğlenceli video kurgusu" / Reels 13:** Premiere'de "AB AYCAM - Reels 13 v3" sequence'i: **logo sağ üst köşede, %30 opaklık, video boyunca**; **9 vurgu yazısı Tahoma Bold (Arapça düzgün), beyaz, mankenin arkasından geçecek şekilde ekranın alt kısmında**; kesim süresi ~3,3 sn. XML aktarımında logo ekran dışına kayıyor, yazılar boş altyazı katmanı oluyordu; Premiere içinde elle düzeltildi.
3. **Premiere kolaj için Arapça bindirme yazıları** (ilk dönem).
4. **İlk iki tanıtım videosu (kodla):** `tanitim_videosu_9x16*.mp4`, `tanitim_gunluk_9x16.mp4` (60 sn, 720x1280, ElevenLabs anlatımı, Arapça altyazı). `tanitim_videosu_9x16 pp.mp4` kullanıcının düzenlediği sürüm, dokunma.

### 5.3 6 seslendirmeli video
Seslendirme metinleri: `premiere pro\15\seslendirme yazilari.md/.txt` (Mısır Arapçası, kullanıcı ElevenLabs'te seslendirdi).

| # | Video | Ses | Süre | Alt başlık |
|---|---|---|---|---|
| 1 | `video_1_gunluk1.mp4` | günlük 1.mp3 | ~42,2 sn | على جميع أنواع الأقمشة |
| 2 | `video_2_gunluk2.mp4` | günlük 2.mp3 | ~36,6 sn | جودة تركية · بدون استيراد |
| 3 | `video_3_lingerie1.mp4` | lingerie 1.mp3 | ~37,3 sn | على الساتان والتل والشيفون |
| 4 | `video_4_lingerie2.mp4` | lingerie 2.mp3 | ~35,9 sn | لمسة فخامة على كل تصميم |
| 5 | `video_5_lingerie3.mp4` | lingerie 3.mp3 | ~39,0 sn | جودة تركية داخل مصر |
| 6 | `video_6_lingerie4.mp4` | lingerie 4.mp3 | ~39,4 sn | على جميع أنواع الأقمشة |

**Teknik:** 1080x1920, 30 fps, H.264 crf 18, AAC 192k, müzik yok; her sesin sonuna 1 sn ek bekleme.
**Tasarım:** Foto sahnesi = 936x1248 altın çerçeveli foto + yavaş zoom, arkada bulanık hareketli kumaş videosu, üstte logo + "طباعة الاستراس بالمتر" + alt başlık, altta altyazı. Video sahnesi = tam ekran klip + alt gradyan + altyazı. Geçişler 0,35 sn. Bitişte CTA ekranı (logo, "ابعت لنا القماش بتاعك", 3 telefon, adres).
**Altyazı zamanlama:** Whisper/HF model indirmesi 403 verdiği için ses sessizliklerinden (RMS, eşik = %95 dB − 34, min 0,12 sn) + senaryo metni eşleştirmesi. Zamanlama ±0,5 sn kayabilir.
**Medya kullanımı:**
- Klipler: `Photos-1-001` (42 klip; kullanıcı 16 bozuk klibi sildi). 28 iyi klip, hiçbir parça tekrar edilmedi. Kötü/sönük klip indeksleri: 2, 6, 9, 11, 19–21, 23, 36, 39, 41; 29 çok kısa.
- Lingerie fotoğrafları: V1'de önce 6a, 14, 16a, 10a, 27, 24, 2a, 3a, 8, 16, 28, 36a, 41a kullanılmıştı; V3–V6'da tekrar yok.
- Günlük: V1 → 4, 5, 8, 9, 10, 11, 12, 14; V2 → 15 (yeni) + 2, 3, 6, 7, 13, 16, 1, 17 (tekrar). 22 numaralı görsel kenar boşluğu nedeniyle kullanılmadı.
**Çalıştırma:** bash çağrısı ~175 sn ile sınırlı; her video 2 paralel parça (~2 dk). Arka plan işleri çağrı bitince ölür. `run.sh <video_no>`; plan `plan.json`, altyazılar `pages.json`. Font: Cairo (`/tmp/f/cairo_full.ttf`, geçici klasörde, yeniden indirilmesi gerekebilir).
**Revizyon yöntemi:** Kullanıcı "video no + saniye + istek" yazar; ilgili sahne `plan.json`'da değiştirilip yalnız o video yeniden render edilir.

### 5.4 Müzik önerileri (`premiere pro\müzikler`, dinlenmeden isim/tarza göre)
Günlük 1: Amr Diab & Orange – Lola El Banat · Günlük 2: Amr Diab – Getlak · Lingerie 1: Sherine – Tebaan Tebaan · Lingerie 2: Hamaki & Sherine – Bahareya · Lingerie 3: TUL8TE – El Hob Gany · Lingerie 4: TUL8TE & Saint Levant – Nano · Yedek: TUL8TE – Garee2a Awy.
Uygun değil: Kooty, Mekassarat, Players, Gamila, Hena Masr (konuşmayı bastırır), Baba, Ebtadena, Sahby Ya Sahby (anlam), Esam Sasa (sert). Müzik −18/−22 dB; Facebook/Instagram telif riski (Meta ses kütüphanesi daha güvenli). **Müzik henüz eklenmedi; kullanıcı onayı bekliyor veya kendisi ekleyecek.**

---

## 6. Facebook / Meta Business Suite / TikTok

Ayrıntı: `is-akislari/meta-mesaj-ve-yorum-cevaplama.md` ve `is-akislari/tiktok-hesap-kurtarma.md`.

- **Gelen mesaj ve yorum yönetimi:** Meta Business Suite gelen kutusundan (Messenger + Facebook yorumları). Cevaplar Arapça (Mısır lehçesi), kişinin adıyla, sadece wa.me linkiyle; fiyat ve model bilgisi sadece WhatsApp'tan verilir. Yorumlarda otomatik özel mesaj numarayı zaten gönderiyorsa tekrar cevap yazılmaz. Önce Türkçe tablo (kim, ne yazmış, cevap), onay, sonra gönderim.
- **Hazırlananlar:** sayfa açıklaması, kapak görseli metni, duyuru gönderisi, WhatsApp otomatik yanıtı, Arapça yorum yanıt şablonu.
- **Facebook sayfa adı değişikliği (çözülmedi):** hedef "AB Ayçam Metraj Taş Baskı"; doğrulama kodu erişilemeyen eski telefona gidiyor. Claude şifre/kod girmez.
- **TikTok:** Şirket hesabı @toqa7808, eski çalışan giriş bilgisini bırakmadı. Kurtarma sırası: şirket numarasıyla ve kullanıcı adıyla "şifremi unuttum", eski çalışana ipucu sorma, şirket e-postalarında "tiktok" arama, Chrome kayıtlı şifreleri, TikTok destek başvurusu. Bu Chrome'da açık olan @cihankrmz61 kullanıcının kişisel hesabıdır, şirket hesabı değildir. TikTok yorum/mesaj akışı hesaba giriş sonrası Facebook'takine benzer yürütülecek (TikTok'ta link tıklanmaz, hız sınırı var). Durum: beklemede.

---

## 7. Diğer işler
- **Paisley vektör:** `premiere pro\vektor\` – Illustrator Image Trace çıktıları (`paisley_vektor` 5 renk ~44 bin yol, `paisley_vektor_3renk` ~39 bin yol; .ai/.svg/.pdf) ve kodla çizilmiş taslak. Kullanıcı "profesyonel çizimci elinden, ince detaylı" istedi; kodla taslak bu seviyeye ulaşmadı. Seçenekler: gerçek çizimci, kullanıcının Illustrator'da devam etmesi veya Claude'un tek tek motif çizmesi (cevap bekleniyor).
- **Claude projesine bilgi (Context) ekleme:** Claude projenin Context bölümüne dosya ekleyemez ve yüklenen dosyayı düzenleyemez. Bu yüzden asıl kaynak bu GitHub reposudur; proje Instructions kısmı yeni sohbetin repoyu okumasını söyler.

---

## 8. Açık işler / sonraki adımlar
Güncel ve ayrıntılı liste: `bekleyen-isler.md`. Özet:
1. Ev tekstili: onaylı sahneden 3 detay görseli üretimi; uzun parçanın gerçek ölçüsü; yıldız ve diğer setler için aynı sahne düzeni.
2. Meta: eski Messenger mesajlarındaki yazılı telefon numaraları (düzenlenemez; silip yeniden göndermek geri alınamaz, kullanıcı kararı bekliyor), 2 haftalık eski yorum/mesaj taraması, makine videosunda gizli kalan 12 yorum, kalan numaralı yorum cevaplarının düzeltilmesi.
3. TikTok hesabına erişimin geri alınması, sonra yorum/mesaj akışı.
4. Facebook sayfa adı değişikliği; 2FA ve telefon temizliği; hesap kilidi açma son günü 25 Ekim 2026.
5. 6 videoda revizyonlar (video no + saniye); müziklerin eklenmesi.
6. Pollo AI üyeliği sonrası taş koruma video denemeleri.
7. Gemini giydirme üretimlerinin devamı (v12 sonrası, Mısır iklimine uyarlama).
8. Paisley vektör için yol seçimi.
9. İki aşamalı (düz kıyafet + desen bindirme) yöntemin testi: yapıldı mı doğrulanmadı.
10. GitHub: repo özel mi teyidi (görünüşe göre private yapıldı); bu dosyaları klona kopyalayıp Commit + Push.
