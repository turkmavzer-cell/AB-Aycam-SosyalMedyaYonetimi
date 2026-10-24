# Sim (glitter) kumaş şal görselleri — Gemini prompt iş akışı

Son güncelleme: 20.10.2026

## Amaç
AB Ayçam sim baskılı şal/eşarp kumaşları için kadın modelli Nano Banana (Gemini) görselleri; video ve şalcı/eşarpçı paylaşımlarında örnek görsel olarak kullanılır ("صور توضيحية" notu ile, gerçek iş gibi sunulmaz).

## Gerçek simin özellikleri (videolardan)
- Sim üfleme makinesi, kumaş ilerlerken sim serper: parçalar kumaşa rastgele ve eşit dağılır. Öbek, desen, şerit yok.
- Parçalar küçük, ince çubuk gibi, holografik (beyaz, turkuaz, yeşil, mor yansıma). Koyu kumaşta (siyah, zeytin) çok belirgin, açık gri/bej kumaşta az belirgin.
- Gerçek ürünler şifon/georgette şal ve eşarplar.

## Sürümler ve sonuçları
| Sürüm | Durum | Neden |
|---|---|---|
| v15 | REDDEDİLDİ | Simler öbek öbek, desen gibi çıktı; referans karelerde parlama lekeleri vardı |
| v16 | YETERSİZ | Dağılım düzeldi (serpme) ama sim belli olmuyordu |
| v17 | KISMEN | Daha belirgin sim; yarım boy şal çekimleri yine zayıf |
| v18 | ONAYLI | Başa sarılan şal ve portre promptları daha iyi sonuç verdi (promptlar\GEMINI PROMPTLARI v18 ...) |

## Çalışan yöntem
1. Referans: gerçek şal fotoğraflarından/videolarından kumaş-only kırpımlar (kişi/arka plan yok, parlama lekesi yok, yoğun sim yığını yok). Prompta "referansı SADECE kumaş ve sim için kullan, kişiyi ve arka planı kopyalama" yazılır.
2. Sim tarifi olumlu yazılır: rastgele ve eşit serpilmiş, her parça ayrı, tuz tanesi boyutunda, ilk bakışta görünür (yaklaşık 1-2 cm'de bir), keskin odakta, beyaz/turkuaz/yeşil/mor parıltı; öbek/desen yasağı aynı paragrafta. Taban kumaş mat düz renk, metalik veya payetli değil.
3. Sim kadrajda görünsün: kumaş kadrajın büyük kısmını kaplasın (başa sarılı şal, yakın çekim, portre), yan/arka ışık veya flaş kullan, koyu kumaşta daha belirgin olur.
4. Loş ortamda: tek lamba veya flaş; parıltı efekti, ışık çizgisi, lens flare yok.
5. Giysi mütevazı: uzun kollu, yüksek yaka, bol; genç modern tesettür için blazer/pantolon gibi şık ama kapalı kombin.
6. Gün batımı: alçak arka ışık simi canlandırır ama kırmızıyı turuncuya çekebilir; "true red, not orange" cümlesi eklenir.

## Sorun giderme cümleleri
v17 dosyasının sonunda (sim azsa, öbek olduysa, metalik çıktıysa, renk kaydıysa, referanstaki kişi kopyalandıysa).

## İlgili dosyalar
- Referans kareler: `premiere pro\19 - sim\gemini-referans-kareler-v2\` ve `gemini-referans-kareler-v3\`
- Promptlar: `promptlar\GEMINI PROMPTLARI v15 ... v18`


## Glitter referans görselli 28 prompt (21.10.2026)
- Yöntem: referans = poşet içindeki ham glitter fotoğrafı; prompt poşeti yok sayıp sadece simin renk/şekil/boyutunu alır ve yeni fotoğraf üretir (kumaş/şal/eşarp üzerinde serpme sim).
- Boyut kuralı: en büyük parçalar 0,5 cm altı (3-4 mm), küçükler ~1 mm. Yoğunluk prompt başına light/medium. Dosya: `promptlar\sim_glitter_28_prompt.md`. Durum: denenmedi.
