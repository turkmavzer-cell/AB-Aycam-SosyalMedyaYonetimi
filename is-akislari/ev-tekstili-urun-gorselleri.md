# İş akışı: Ev tekstili ürün görselleri (Gemini / Nano Banana)

Son güncelleme: 13.10.2026

## Amaç
Ev tekstili taş baskı setini (büyük, küçük, uzun parça) Gemini Nano Banana ile gerçekçi, sade ve katalog kalitesinde sahne görsellerinde göstermek. Görseller Mısır'da satış için telefondan bakılacak PDF katalogda (3:4 dikey) kullanılacak.

## Girdiler
- Ürün fotoğrafları: `E:\ab ayçam\taşlı yapay zeka\Ev Textili\` – kar, yıldız, çiçek × büyük, küçük, uzun (.jpg, ~14 MB; yüklemeden önce ~2000 px'e küçült).
- Ürün hattı: 5 model × 3 boyut. Büyük 75x75 cm, küçük 45x45 cm (tabak altlığı), uzun parça (tencere altlığı, uçları sivri altıgen kesim; ölçü teyit bekliyor).
- Kumaş krem/fildişi, taşlar gümüş kristal. Kumaş rengi hiçbir görselde değişmez.

## Yöntem (iki aşama)
**1. Aşama – tam üstten sahne.** Yerleşim kullanıcının çizdiği düzen: uzun yemek masası; büyük parça ortada çapraz (elmas); iki küçük parça masa uçlarında düz, masa genişliğinde ortalı ve simetrik; uzun parça sağ üstte boş alanda düz. Etrafında sandalyeler, masada az aksesuar (desenin üstüne bir şey konmaz). Prompt: `promptlar/ev-tekstili-cicek-sahne-dogal-misir-onayli.md`. Yükleme: 1 = onaylı yerleşim görseli, 2 = büyük, 3 = küçük, 4 = uzun.

**2. Aşama – detay çekimleri.** Onaylı sahne görseli + 3 orijinal yüklenir. Promptlar: `promptlar/ev-tekstili-cicek-detay-promptlari.md` (tabak altlığı, merkez desen, makro köşe). 3:4 dikey.

## Kurallar ve kararlar
- Görsel tek karede, üstten, sade: "sadece modelleri yan yana koymak" reddedildi; güzel ve konseptli ama detaylarla boğmayan bir sunum istendi.
- Parçalar gerçek orana uygun çizilmeli. Gemini küçük parçaları büyük çiziyor, biri masa kenarına kayıyor; çözüm: ölçü cümleleri (küçük parça masa genişliğinin ~%40'ı, büyüğün köşegeninin %42'si), "mirror pair", "exactly centered" ve gerekirse "shrink by another 15%".
- Taş gerçekçiliği: "gri basılı nokta" değil, parlak facetli kristal; temas gölgesi, parlama ve gökkuşağı yansıması.
- Masa üstüne konan aksesuarlar sadece boş ahşap alanda, hiçbir desenli parçanın üstünde değil.
- Gemini aynı sohbette önceki görseli tekrar edebilir; yeni sahne için temiz sohbet.
- Mısır pazarı: ev içi, doğal, sıcak konsept seçildi.

## Denenen ve olmayanlar
- **v13 (3 oda konsepti, kar seti):** reddedildi. Kumaş rengi değişti (lacivert kadife, şampanya saten, adaçayı keten), oda sahnesi oldu, üstten çekim değildi.
- **v14 (üstten kolaj, 3 konsept):** Gemini aynı görseli üretti; kullanıcı "konsept olmasın, her model için prompt" istedi.
- **Model başına düz üstten promptlar (kar):** parçalar gri-mavi yüzeyde düz yan yana, taşlar mat gri çıktı; "böyle olmasın". Çözüm: kullanıcının çizdiği masa yerleşimi + parlak kristal tarifi.
- **Nil kenarı terası (dış mekan, gün batımı):** beğenilmedi; "daha ev içi ve doğal olsun".
- **Ramazan iftar sofrası (koyu ceviz, fener, hurma):** beğenildi, yedek konsept.
- **Eski Kahire (mashrabiya, pirinç):** üretilmedi.
- **Açık ahşap, modern Skandinav sahne:** onaylandı, yerleşim referansı oldu.

## Mevcut durum
Çiçek seti: onaylı sahne üretildi, detay görselleri üretimi bekliyor. Yıldız ve diğer setler için aynı sahne düzeni uygulanacak. Bekleyenler `bekleyen-isler.md` dosyasında.
