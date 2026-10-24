# GEMINI PROMPTLARI v16 — Sim kumaş şal (serpme sim + loş ortam)

Bu sürüm v15'in yerine geçer. v15 reddedildi: simler öbek öbek / desen gibi çıkıyordu.

**Sim gerçeği:** Sim üfleme makinesi kumaş ilerlerken simi rastgele serper. Yani simler kumaşın her yerine, eşit ve dağınık, birbirinden ayrı tek tek parçacıklar halinde düşer. Küme, grup, şerit, çiçek, yıldız, dalga veya geometrik desen yoktur.

## Nasıl kullanılır
1. Gemini'de yeni sohbet aç. Her görsel için o promptun "Referans" satırındaki kareyi yükle (klasör: `E:\ab ayçam\premiere pro\19 - sim\gemini-referans-kareler-v2`).
2. Önce **BLOK 1**'i, hemen altına seçtiğin promptu yapıştır.
3. Loş promptlarda **BLOK 2** de eklenir (BLOK 1 + BLOK 2 + prompt).
4. Sim çok yoğun veya öbek çıkarsa en alttaki "Sorun giderme" cümlesini ekle.

---

## BLOK 1 — Standart (tüm promptlarda)

```
Use the attached reference photo as the exact fabric. Reproduce the fabric's colour, matte texture and the glitter exactly as in the reference; do not change the fabric colour.

GLITTER DISTRIBUTION (most important): the glitter was blown onto the moving fabric by a machine, so it is sprinkled completely at random and evenly over the whole fabric surface. Every glitter speck is a tiny separate dot (about the size of a grain of fine sand), with clear bare fabric between neighbouring specks. The density is the same everywhere: no clusters, no clumps, no groups, no patches, no bands, no lines, no stripes, no waves, no flowers, no stars, no repeating or symmetric arrangement, no pattern of any kind. It looks like a fine scatter of salt grains, uniformly spread, including over folds and drapes. The fabric is a plain solid colour with only the sparse random glitter dust on it.

The woman is a real person photographed naturally. Modest, elegant look: she wears simple plain clothes (long sleeves, high neckline, loose fit, nothing revealing). Her hair and styling are as described. The glitter fabric is used as a large shawl draped over her shoulders and arms, with natural soft folds. Photorealistic, high resolution, vertical 3:4 framing, no text, no watermark, no logo.
```

## BLOK 2 — Loş / karanlık ortam (sadece loş promptlarda)

```
LIGHTING: a dim, low-light environment. The glitter specks catch the little available light and sparkle as tiny bright points, each speck individually glinting, evenly spread over the shawl. The fabric itself stays its true colour (do not darken, wash out or recolour it). The sparkle is subtle and realistic, like a phone photo or a candid flash photo taken in a dim room: no glow effects, no light streaks, no lens flare, no bokeh balls on the fabric.
```

---

## Kumaş profilleri

| Kod | Kumaş | Sim | Referans karesi |
|---|---|---|---|
| A | Kırmızı | Çok ince, seyrek gümüş/mor ışıltı | A_kirmizi_1, A_kirmizi_2 |
| B | Ahududu (koyu pembe-bordo) | Orta seyreklikte mor/gümüş, yer yer yeşil minik parça | B_ahududu_1, B_ahududu_2, B_ahududu_yakin_cekim |
| C | Gri-bej | İnce gümüş toz | C_gri-bej_1, C_gri-bej_2 |
| D | Zeytin yeşili | İnce gümüş/mavi ışıltı | D_zeytin_1, D_zeytin_2 |
| E | Siyah | Gümüş/beyaz-mavi ışıltı, orta seyreklik | E_siyah_1, E_siyah_2 |

Not: C_gri-bej_1 ve E_siyah_1/2 kareleri yoğun sim lekesi içeren bölümler çıkarılarak kırpıldı. Referans karesini değiştirme.

---

## A — KIRMIZI

**A1 (gün ışığı)** — Referans: A_kirmizi_1
```
A woman in her 30s with long dark brown hair, standing in a bright sunlit living room next to a window, wearing a plain cream long-sleeve top and long skirt. She wears the red glitter fabric as a large shawl over both shoulders, one end falling in front. Soft natural daylight, half-body shot, gentle smile looking at the camera.
```

**A2 (gün ışığı)** — Referans: A_kirmizi_2
```
A woman in her 40s with a neat low bun, in a sunny garden terrace with green plants softly blurred behind, wearing a plain black long dress with a high neckline. The red glitter fabric is draped as a shawl around her shoulders and arms. Natural afternoon light, three-quarter body shot, relaxed pose.
```

**A3 (loş)** — Referans: A_kirmizi_1 — BLOK 1 + BLOK 2
```
A woman in her 30s with shoulder-length wavy hair, sitting at a table in a dimly lit cosy cafe in the evening, wearing a plain dark-grey long-sleeve dress. The red glitter fabric is draped over her shoulders as a shawl. Only a warm small lamp lights the scene. Candid photo, half-body.
```

**A4 (loş)** — Referans: A_kirmizi_2 — BLOK 1 + BLOK 2
```
A woman in her 20s with long straight black hair, standing in a dim hallway at home at night, lit by a single flash from the camera, wearing a plain white long-sleeve blouse and long trousers. The red glitter fabric is worn as a shawl over her shoulders, one hand holding its edge. Close half-body shot.
```

---

## B — AHUDUDU

**B1 (gün ışığı)** — Referans: B_ahududu_1
```
A woman in her 30s with long light-brown hair, standing by a large bright window in a modern white room, wearing a plain ivory long-sleeve dress. The raspberry glitter fabric is draped as a shawl over her shoulders and falls in soft folds. Soft daylight, half-body shot, calm expression.
```

**B2 (gün ışığı, yakın çekim)** — Referans: B_ahududu_yakin_cekim
```
Close-up of a woman's shoulder and upper arm from the side, in soft daylight, wearing a plain beige long-sleeve top. The raspberry glitter fabric is draped over her shoulder; the fabric fills most of the frame so the evenly scattered glitter specks are clearly visible. Her face is only partly visible or cropped at the chin.
```

**B3 (loş)** — Referans: B_ahududu_2 — BLOK 1 + BLOK 2
```
A woman in her 40s with an elegant low ponytail, at an evening family gathering in a softly dim room with warm lights far in the background, wearing a plain black long dress. The raspberry glitter fabric is worn as a shawl over her shoulders. Half-body candid photo.
```

**B4 (loş)** — Referans: B_ahududu_1 — BLOK 1 + BLOK 2
```
A woman in her 20s with long dark curly hair, standing outside a building at dusk, the street dim and blue-grey, lit only by a camera flash, wearing a plain long black skirt and a long-sleeve top. The raspberry glitter fabric is draped around her shoulders. Three-quarter shot.
```

---

## C — GRİ-BEJ

**C1 (gün ışığı)** — Referans: C_gri-bej_1
```
A woman in her 30s with brown hair in a loose braid, standing in a bright airy room with white walls, wearing a plain dusty-rose long-sleeve dress. The grey-beige glitter fabric is draped as a shawl over her shoulders. Soft daylight, half-body shot, gentle look at the camera.
```

**C2 (gün ışığı)** — Referans: C_gri-bej_2
```
A woman in her 40s with shoulder-length dark hair, on a sunny balcony with soft green plants behind, wearing a plain navy long-sleeve dress. The grey-beige glitter fabric is worn as a large shawl wrapped loosely around her shoulders and arms. Natural light, three-quarter shot.
```

**C3 (loş)** — Referans: C_gri-bej_1 — BLOK 1 + BLOK 2
```
A woman in her 30s with long wavy hair, seated in a dim restaurant lounge in the evening with a small warm candle lamp on the table, wearing a plain deep-burgundy long-sleeve dress. The grey-beige glitter fabric is draped as a shawl over her shoulders. Half-body candid shot.
```

**C4 (loş)** — Referans: C_gri-bej_2 — BLOK 1 + BLOK 2
```
A woman in her 20s with a sleek ponytail, in a dark room at night lit by a single flash, wearing a plain black long-sleeve dress. The grey-beige glitter fabric is worn as a shawl, her hands holding its front edges. Half-body shot.
```

---

## D — ZEYTİN

**D1 (gün ışığı)** — Referans: D_zeytin_1
```
A woman in her 30s with long dark hair, standing in a sunlit room with a cream curtain behind, wearing a plain white long-sleeve blouse and long skirt. The olive-green glitter fabric is draped as a shawl over her shoulders. Soft daylight, half-body shot, warm smile.
```

**D2 (gün ışığı)** — Referans: D_zeytin_2
```
A woman in her 40s with a neat bun, standing in a bright cafe near a window, wearing a plain cream long-sleeve dress. The olive-green glitter fabric is wrapped around her shoulders and arms as a shawl. Natural daylight, three-quarter shot.
```

**D3 (loş)** — Referans: D_zeytin_1 — BLOK 1 + BLOK 2
```
A woman in her 30s with long straight brown hair, in a dimly lit living room in the evening with one warm table lamp, wearing a plain black long dress. The olive-green glitter fabric is draped over her shoulders as a shawl. Half-body candid photo.
```

**D4 (loş)** — Referans: D_zeytin_2 — BLOK 1 + BLOK 2
```
A woman in her 20s with wavy dark hair, standing on a quiet street at night with distant dim lights, lit by a gentle camera flash, wearing a plain grey long-sleeve dress. The olive-green glitter fabric is worn as a shawl over her shoulders. Half-body shot.
```

---

## E — SİYAH

**E1 (gün ışığı)** — Referans: E_siyah_1
```
A woman in her 30s with light-brown hair, standing in a bright room with pale walls, wearing a plain pastel-pink long-sleeve dress so the black fabric stands out. The black glitter fabric is draped as a shawl over her shoulders. Soft daylight, half-body shot.
```

**E2 (gün ışığı)** — Referans: E_siyah_2
```
A woman in her 40s with shoulder-length hair, on a sunlit terrace with soft green plants behind, wearing a plain ivory long-sleeve dress. The black glitter fabric is worn as a large shawl over her shoulders and arms. Natural light, three-quarter shot.
```

**E3 (loş)** — Referans: E_siyah_1 — BLOK 1 + BLOK 2
```
A woman in her 30s with long wavy hair, at an evening event in a dim hall with warm lights far behind, wearing a plain light-grey long-sleeve dress. The black glitter fabric is draped as a shawl over her shoulders; the evenly scattered specks glint against the black. Half-body candid photo.
```

**E4 (loş)** — Referans: E_siyah_2 — BLOK 1 + BLOK 2
```
A woman in her 20s with a low bun, in a dark room at night lit only by a camera flash, wearing a plain cream long-sleeve blouse and long skirt. The black glitter fabric is worn as a shawl, one hand holding its edge. Half-body shot.
```

---

## Sorun giderme
- **Sim öbek/desen çıktıysa**, aynı sohbette şunu yaz: `The glitter is clustered. Regenerate: every glitter speck must be a separate tiny dot, randomly and uniformly sprinkled over the entire fabric with bare fabric between them, no groups, no patterns, same density everywhere.`
- **Sim çok yoğun çıktıysa:** `Reduce the glitter to the sparse density of the reference photo.`
- **Kumaş rengi kaydıysa:** `Keep the fabric colour exactly as in the reference photo.`
- **Loşta kumaş çok koyulaştıysa:** `Show the fabric in its true colour, just slightly dim.`
- **Yüz/kıyafet açık çıktıysa:** `Modest plain long-sleeve high-neck clothing only.`

## Kullanım notları
- Fiyat ve yazı içermez. Görseller Meta reklamı/video için kullanılacaksa kumaş rengi değişmemiş olmalı; ürünle karşılaştır.
- Üretilen görsellerin sim dağılımını kumaş videosuyla karşılaştırıp onayla; onaylananları bana söyle, `promptlar` klasörüne kelimesi kelimesine işleyeyim.
