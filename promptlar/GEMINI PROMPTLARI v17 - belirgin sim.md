# GEMINI PROMPTLARI v17 — Belirgin serpme sim (şal / eşarp)

v16'nın yerine geçer. Sorun: v16 görsellerinde sim belli olmuyordu. Gerçek ürün videolarına ve WhatsApp fotoğraflarına bakıldı (20.10.2026).

**Gerçek simin özellikleri (videolardan):**
- Sim küçük, ince, çubuk gibi holografik parçalardır. Işığı alınca beyaz, turkuaz, yeşil, mor parıltı verir.
- Makineyle üflendiği için kumaşın her yerine eşit ve rastgele dağılır. Öbek, desen yok.
- Koyu kumaşta (siyah, zeytin) çok belirgin, açık kumaşta (gri, bej) daha az belirgindir.

**Bu sürümde yapılanlar:** Sim boyutu ve yoğunluğu bilerek artırıldı (yine tek tek ve eşit dağılmış). Her kumaş için 4 prompt var: gün ışığı yarım boy, gün ışığı yakın çekim, loş ortam, flaşlı/yan ışık. Yakın çekimlerde kumaş kadrajı doldurduğu için sim en belirgin orada görünür.

## Nasıl kullanılır
1. Gemini'de yeni sohbet aç. Promptun "Referans" satırındaki kareleri yükle.
   - Zeytin, siyah, gri: `E:\ab ayçam\premiere pro\19 - sim\gemini-referans-kareler-v3` (gerçek şal fotoğraflarından kırpıldı)
   - Kırmızı, ahududu: `gemini-referans-kareler-v2` (bu renklerin yeni çekimi yok)
2. **BLOK 1**'i, altına seçtiğin promptu yapıştır.
3. Loş promptlarda BLOK 1 + **BLOK 2**, yakın çekimlerde BLOK 1 + **BLOK 3** ekle.
4. Sim hâlâ belli olmuyorsa veya öbek çıkarsa en alttaki "Sorun giderme" cümlelerini yaz.

---

## BLOK 1 — Standart (tüm promptlarda)

```
Use the attached reference photo(s) ONLY for the fabric: its colour, its matte fabric texture and, most importantly, its glitter. Do not copy the person, clothes or background from the reference. Do not change the fabric colour.

GLITTER (the most important part, it must be clearly visible): the fabric is dusted with real holographic glitter flakes that were blown onto it by a machine, so they are sprinkled completely at random and evenly over the whole fabric, including the folds, the drape over the shoulders and the parts hanging down the arms. Each flake is a tiny separate sliver, about the size of a grain of salt, with bare fabric between neighbouring flakes. Every flake catches the light and gives a bright white, cyan, green or magenta glint. Density: clearly visible at first glance, even on a phone screen, roughly one flake every 1 to 2 centimetres, much more noticeable than a faint dust. Keep the flakes sharp and in focus; some are brighter than others and a few catch strong highlights. The same density everywhere: no clusters, no clumps, no groups, no patches, no bands, no lines, no stripes, no waves, no flowers, no stars, no pattern of any kind. The base fabric stays a plain matte solid colour; it is not a metallic, shiny or sequin fabric.

The woman is a real person photographed naturally, with a modest and elegant look: plain long-sleeve clothes, high neckline, loose fit, nothing revealing. The glitter fabric is used as a large shawl draped over her shoulders and arms in natural soft folds. Photorealistic, high resolution, vertical 3:4 framing, no text, no watermark, no logo.
```

## BLOK 2 — Loş / karanlık ortam (loş ve flaşlı promptlarda)

```
LIGHTING: a dim, low-light environment. The glitter flakes catch the little available light and sparkle strongly as tiny bright points, each flake individually glinting, evenly spread over the whole shawl. The fabric keeps its true colour (do not darken, wash out or recolour it). The sparkle is realistic, like a phone photo or a candid flash photo taken in a dim room: no glow effects, no light streaks, no lens flare, no bokeh balls on the fabric.
```

## BLOK 3 — Yakın çekim (yakın çekim promptlarında)

```
COMPOSITION: a close-up detail shot. The shawl fills at least two thirds of the frame, shot from about one metre away with the glitter flakes in sharp macro-like focus and only the background softly blurred. The evenly scattered flakes are the main subject of the photo. The woman is only partly visible (shoulder, chin or neck).
```

---

## Kumaş profilleri

| Kod | Kumaş | Gerçek sim görünümü | Referans |
|---|---|---|---|
| A | Kırmızı | İnce, seyrek mor/gümüş | v2: A_kirmizi_1, A_kirmizi_2 |
| B | Ahududu (bordo-pembe) | Mor/gümüş, yer yer yeşil | v2: B_ahududu_1, B_ahududu_2, B_ahududu_yakin_cekim |
| C | Gri-açık gri | Beyaz ve koyu çubuk parçalar | v3: C_gri_gercek_1 + v2: C_gri-bej_1, C_gri-bej_2 |
| D | Zeytin yeşili | Turkuaz, yeşil, beyaz parıltı | v3: D_zeytin_gercek_1_yakin, D_zeytin_gercek_2, D_zeytin_gercek_1 |
| E | Siyah | Beyaz, turkuaz, mavi parıltı (en belirgin) | v3: E_siyah_gercek_1_yakin, E_siyah_gercek_2, E_siyah_gercek_3 |

---

## A — KIRMIZI

**A1 (gün ışığı, yarım boy)** — Referans: A_kirmizi_1
```
A woman in her 30s with long dark brown hair, standing in a bright sunlit living room next to a window, wearing a plain cream long-sleeve top and long skirt. She wears the red glitter fabric as a large shawl over both shoulders, one end falling in front. Soft natural daylight, half-body shot, gentle smile looking at the camera.
```

**A2 (gün ışığı, yakın çekim)** — Referans: A_kirmizi_2 — BLOK 1 + BLOK 3
```
A close-up of a woman's shoulder and upper arm in soft window daylight, wearing a plain beige long-sleeve top. The red glitter fabric is draped over her shoulder in soft folds, light coming from the side so the flakes glint. Only her chin and neck are visible.
```

**A3 (loş)** — Referans: A_kirmizi_1 — BLOK 1 + BLOK 2
```
A woman in her 30s with shoulder-length wavy hair, sitting at a table in a dimly lit cosy cafe in the evening, wearing a plain dark-grey long-sleeve dress. The red glitter fabric is draped over her shoulders as a shawl. Only a small warm lamp lights the scene. Candid photo, half-body.
```

**A4 (flaşlı)** — Referans: A_kirmizi_2 — BLOK 1 + BLOK 2
```
A woman in her 20s with long straight black hair, standing in a dim hallway at home at night, lit by the direct flash of the camera, wearing a plain white long-sleeve blouse and long trousers. The red glitter fabric is worn as a shawl over her shoulders, one hand holding its edge. Half-body shot.
```

---

## B — AHUDUDU

**B1 (gün ışığı, yarım boy)** — Referans: B_ahududu_1
```
A woman in her 30s with long light-brown hair, standing by a large bright window in a modern white room, wearing a plain ivory long-sleeve dress. The raspberry glitter fabric is draped as a shawl over her shoulders and falls in soft folds. Soft daylight, half-body shot, calm expression.
```

**B2 (gün ışığı, yakın çekim)** — Referans: B_ahududu_yakin_cekim — BLOK 1 + BLOK 3
```
A close-up of a woman's shoulder from the side in soft daylight, wearing a plain beige long-sleeve top. The raspberry glitter fabric is draped over her shoulder; the fabric fills most of the frame. Only her chin is visible.
```

**B3 (loş)** — Referans: B_ahududu_2 — BLOK 1 + BLOK 2
```
A woman in her 40s with an elegant low ponytail, at an evening family gathering in a softly dim room with warm lights far in the background, wearing a plain black long dress. The raspberry glitter fabric is worn as a shawl over her shoulders. Half-body candid photo.
```

**B4 (flaşlı)** — Referans: B_ahududu_1 — BLOK 1 + BLOK 2
```
A woman in her 20s with long dark curly hair, standing outside a building at dusk on a dim blue-grey street, lit by a camera flash, wearing a plain long black skirt and a long-sleeve top. The raspberry glitter fabric is draped around her shoulders. Three-quarter shot.
```

---

## C — GRİ (açık gri)

Not: Açık kumaşta sim zor seçilir. Bu yüzden C promptlarında koyu zemin ve yan ışık kullanıldı.

**C1 (gün ışığı, yarım boy)** — Referans: C_gri_gercek_1, C_gri-bej_1
```
A woman in her 30s with brown hair in a loose braid, standing in a bright room with white walls and strong side window light, wearing a plain dusty-rose long-sleeve dress. The light grey glitter fabric is draped as a shawl over her shoulders. The sun hits the shawl from the side so the flakes sparkle. Half-body shot, gentle look at the camera.
```

**C2 (gün ışığı, yakın çekim)** — Referans: C_gri_gercek_1, C_gri-bej_2 — BLOK 1 + BLOK 3
```
A close-up of a woman's shoulder in strong sunlight from a window on the side, wearing a plain dark-brown long-sleeve top so the light grey shawl stands out. The light grey glitter fabric is draped over her shoulder in soft folds. Only her chin is visible.
```

**C3 (loş)** — Referans: C_gri_gercek_1 — BLOK 1 + BLOK 2
```
A woman in her 30s with long wavy hair, seated in a dim restaurant lounge in the evening with a small warm candle lamp on the table, wearing a plain deep-burgundy long-sleeve dress. The light grey glitter fabric is draped as a shawl over her shoulders. Half-body candid shot.
```

**C4 (flaşlı)** — Referans: C_gri-bej_2 — BLOK 1 + BLOK 2
```
A woman in her 20s with a sleek ponytail, in a dark room at night lit only by a camera flash, wearing a plain black long-sleeve dress. The light grey glitter fabric is worn as a shawl, her hands holding its front edges. Half-body shot.
```

---

## D — ZEYTİN

**D1 (gün ışığı, yarım boy)** — Referans: D_zeytin_gercek_2, D_zeytin_gercek_1
```
A woman in her 30s with long dark hair, standing in a bright sunlit hall with a cream curtain behind, wearing a plain white long-sleeve blouse and long skirt, seen from the three-quarter back so the shawl over her shoulders and back is the focus. The olive-green chiffon glitter fabric is draped as a shawl. Soft daylight, half-body shot.
```

**D2 (gün ışığı, yakın çekim)** — Referans: D_zeytin_gercek_1_yakin — BLOK 1 + BLOK 3
```
A close-up of a woman's back and shoulder in soft daylight, wearing a plain white long-sleeve top. The olive-green chiffon glitter fabric is draped over her shoulder and back in soft folds, filling most of the frame. The face is not visible.
```

**D3 (loş)** — Referans: D_zeytin_gercek_2 — BLOK 1 + BLOK 2
```
A woman in her 30s with long straight brown hair, in a dimly lit living room in the evening with one warm table lamp, wearing a plain black long dress. The olive-green chiffon glitter fabric is draped over her shoulders as a shawl. Half-body candid photo.
```

**D4 (flaşlı)** — Referans: D_zeytin_gercek_1 — BLOK 1 + BLOK 2
```
A woman in her 20s with wavy dark hair, standing on a quiet street at night with distant dim lights, lit by a gentle camera flash, wearing a plain grey long-sleeve dress. The olive-green chiffon glitter fabric is worn as a shawl over her shoulders, seen from the three-quarter back. Half-body shot.
```

---

## E — SİYAH

**E1 (gün ışığı, yarım boy)** — Referans: E_siyah_gercek_2, E_siyah_gercek_1
```
A woman in her 30s with light-brown hair, standing in a bright room with pale walls, wearing a plain pastel-pink long-sleeve dress so the black fabric stands out, seen from the three-quarter back. The black chiffon glitter fabric is draped as a shawl over her shoulders. Soft daylight, half-body shot.
```

**E2 (gün ışığı, yakın çekim)** — Referans: E_siyah_gercek_1_yakin, E_siyah_gercek_3 — BLOK 1 + BLOK 3
```
A close-up of a woman's back and shoulder in bright daylight, wearing a plain ivory long-sleeve top. The black chiffon glitter fabric is draped over her shoulder in soft folds and fills most of the frame, the flakes sparkle white, cyan and blue against the black. The face is not visible.
```

**E3 (loş)** — Referans: E_siyah_gercek_2 — BLOK 1 + BLOK 2
```
A woman in her 30s with long wavy hair, at an evening event in a dim hall with warm lights far behind, wearing a plain light-grey long-sleeve dress. The black chiffon glitter fabric is draped as a shawl over her shoulders; the evenly scattered flakes glint against the black. Half-body candid photo.
```

**E4 (flaşlı)** — Referans: E_siyah_gercek_3 — BLOK 1 + BLOK 2
```
A woman in her 20s with a low bun, in a dark room at night lit only by a camera flash, wearing a plain cream long-sleeve blouse and long skirt. The black chiffon glitter fabric is worn as a shawl, one hand holding its edge. Half-body shot.
```

---

## Sorun giderme
- **Sim hâlâ belli olmuyorsa:** `Make the glitter flakes larger and brighter: about twice as many visible flakes, each one clearly sparkling, still evenly and randomly scattered, no clusters.`
- **Sim öbek/desen çıktıysa:** `The glitter is clustered. Regenerate: every flake must be a separate tiny dot, randomly and uniformly sprinkled over the entire fabric with bare fabric between them, no groups, no patterns, same density everywhere.`
- **Kumaş parlak/metalik çıktıysa:** `The base fabric must stay matte and solid colour; only the tiny separate flakes sparkle.`
- **Kumaş rengi kaydıysa:** `Keep the fabric colour exactly as in the reference photo.`
- **Referanstaki kişi veya arka plan kopyalandıysa:** `Use the reference only for the fabric and glitter, create a new woman and a new scene.`
- **Yüz/kıyafet açık çıktıysa:** `Modest plain long-sleeve high-neck clothing only.`

## Notlar
- Görsellerde sim, gerçek üründen biraz daha belirgin olacak (bilerek). Müşteriye "örnek görsel" notuyla gösterilmeli (videoda "صور توضيحية" yazısı var).
- Üretilen görseller beğenilirse hangilerinin "oldu" olduğunu söyle, `promptlar` klasörüne kelimesi kelimesine işleyeyim.
