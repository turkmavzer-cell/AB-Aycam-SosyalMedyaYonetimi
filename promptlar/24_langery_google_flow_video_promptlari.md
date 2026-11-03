# Google Flow (Veo) — Kusursuz Lingerie Video Kılavuzu (Yavaş Pan & Sakin Pozlar)

> **Kaynak Klasör:** `E:\ab ayçam\premiere pro\24 - langery\görseller` (21 adet görsel: `1 copy.jpg` - `21 copy.jpg`)
> **Hedef Araç:** Google Flow / Google Veo (VideoFX) — Image-to-Video (I2V)
> **Kamera Standardı:** Yalnızca Ultra Yavaş Yatay Pan & Sinematik Slider Hareketleri (Zero Zoom/Tilt Jerk)
> **Model Standardı:** Aşırıya Kaçmayan, Doğal, Sakin & Albenili Pozlama (Nefes Alma, Ağır Baş Dönüşü, Tebessüm)
> **Altın Kural (Sıfır Renk/Desen Bozulması):** Promptta yapay renk/desen tarifi YOKTUR; referans görseldeki elbise, kumaş rengi ve taş motifi %100 kilitlenir.

---

## 1. Neden Bu Yeni Promptlar Kusursuz Çalışır?

1. **Renk ve Desen Değişimini Önleme:** Önceki denemede videoda elbisenin renginin değişmesi (örneğin kırmızıdan maviye dönmesi) ve taşların kaybolması, promptta yapay renk tanımlarının yer almasından kaynaklanıyordu. Bu yeni sette hiçbir renk veya kumaş yeniden tarif edilmemiştir; Flow'a görseldeki mevcut kıyafet ve deseni **%100 koruması** emredilmiştir (`Maintain 100% strict visual consistency with the reference image...`).
2. **Sakin ve Akıcı Pan:** Tüm promptlarda kamera hareketi yalnızca **yavaş yatay pan (slow horizontal pan / slider glide)** olarak optimize edilmiştir. Kamera mankene aniden dalmaz, sadece zarifçe kayar.
3. **Aşırıya Kaçmayan Pozlama:** Mankenler abartılı el kol hareketi yapmaz (`hands remain resting naturally`). Yalnızca hafif bir nefes alır, başını ağır çekimde kameraya çevirir ve albenili, sakin bir tebessüm sunar.
4. **Önerilen Flow Ayarları:**
   - **Mod:** Image-to-Video (I2V)
   - **Motion Strength:** `Low / Medium-Low (2 veya 3 / 5)`
   - **Negatif Prompt:** `color shift, dress changing, pattern morphing, fast motion, sudden movement, face distortion, extra limbs, camera shake, low quality`

---

## 2. 21 Görsel İçin Bağımsız Video Oluşturma Promptları

### 1. `1 copy.jpg` — Görsel 1 (Şezlongda Oturuş)
- **Kamera Hareketi:** Soldan sağa ultra yavaş yatay pan (Slow horizontal pan from left to right)
- **Model Koreografisi:** Sakin nefes alış, omuzların zarifçe gevşemesi, başın yavaşça kameraya dönmesi ve hafif albenili tebessüm

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic luxury fashion video, shot on 50mm lens. Ultra-slow, perfectly stabilized horizontal camera pan gliding from left to right across the model seated on the chaise lounge. The woman poses with calm, tasteful elegance: breathing gently, her shoulders settling softly, and slowly turning her head toward the camera with an alluring, subtle half-smile and natural soft eye contact. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, texture, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Warm amber ambient lighting, realistic fabric drape, delicate crystal glimmers, 24fps filmic motion, completely stable anatomy, hyper-realistic.
```

---

### 2. `2 copy.jpg` — Görsel 2 (Kanepede Yana Yaslanış)
- **Kamera Hareketi:** Sağdan sola akıcı yatay pan (Smooth horizontal pan from right to left)
- **Model Koreografisi:** Vücut ağırlığını hafifçe değiştirme, çeneyi zarifçe kaldırma ve dingin büyüleyici bakış

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic luxury nightwear video, shot on 50mm lens. Slow, smooth horizontal camera pan from right to left tracking her relaxed posture on the sofa. The woman poses with effortless grace without overacting: exhaling gently, slowly tilting her chin, and casting a calm, captivating gaze into the camera with an enigmatic, soft smirk. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Warm interior glow, subtle specular crystal sparkles, creamy bokeh, 24fps cinematic motion, photorealistic.
```

---

### 3. `3 copy.jpg` — Görsel 3 (Yatak Kenarında Oturuş)
- **Kamera Hareketi:** Hafif kavisli yavaş panoramik pan (Gentle panoramic camera glide)
- **Model Koreografisi:** Bakışlarını yavaşça kaldırıp kamerayla buluşturma, samimi ve sıcak hafif gülümseme

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic intimate loungewear fashion video, shot on 50mm lens. Gentle, extremely slow panoramic camera glide framing her seated posture on the bed. The woman poses tastefully: breathing softly, raising her chin in ultra-slow motion, and meeting the camera with an enchanting, gentle smile and calm eyes. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Soft warm lighting, delicate crystal glints, luxury bedroom atmosphere, 24fps filmic cadence, pristine stability.
```

---

### 4. `4 copy.jpg` — Görsel 4 (Balkon Tülü Yanında Duruş)
- **Kamera Hareketi:** Perde hattından modele doğru yavaş yatay pan (Slow horizontal pan past the sheer curtains)
- **Model Koreografisi:** Omzu üzerinden geriye doğru ağır çekimde baş çevirme, vakur ve albenili bakış

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic luxury fashion video, shot on 50mm f/1.8 lens. Slow, elegant horizontal camera pan gliding past the sheer curtains toward the standing model. The woman poses with refined subtlety: slowly turning her head over her shoulder toward the camera, holding a poised, magnetic expression with relaxed charm. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Warm sunlit rim lighting, delicate fabric micro-flutter, sparkling crystal highlights, 24fps, crisp details, zero morphing.
```

---

### 5. `5 copy.jpg` — Görsel 5 (Puf Üzerinde Dik Duruş)
- **Kamera Hareketi:** Soldan sağa dengeli yatay kayma panı (Steady horizontal slider pan from left to right)
- **Model Koreografisi:** Omurgasını asilce dikleştirme, omuzları rahatlatma ve kendine güvenen zarif tebessüm

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic luxury loungewear video, shot on 50mm lens. Slow, silky horizontal slider pan from left to right across the model seated on the ottoman. The woman poses with poised composure without exaggerated gestures: taking a slow breath, subtly straightening her posture, and smiling softly into the lens with alluring charm. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Warm chandelier ambient light, crystal micro-shimmers, filmic depth of field, 24fps, pristine anatomy.
```

---

### 6. `6 copy.jpg` — Görsel 6 (Kapı Pervazına Yaslanış)
- **Kamera Hareketi:** Pervazdan modele doğru yavaş panoramik pan (Slow panoramic pan framing the doorway)
- **Model Koreografisi:** Ağırlığını hafifçe diğer ayağa aktarma, başı milimetrik eğme ve etkileyici göz teması

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic high-fashion editorial video, shot on 50mm lens. Ultra-slow, deliberate horizontal panoramic pan framing the doorway and the model. The woman poses with quiet intensity: breathing deeply and calmly, subtly shifting her weight with majestic slow poise while keeping captivating, tasteful eye contact with the camera. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Warm interior contrast, sparkling crystal reflections on the fabric, creamy bokeh, 24fps, hyper-realistic.
```

---

### 7. `7 copy.jpg` — Görsel 7 (Koltukta Rahat Oturuş)
- **Kamera Hareketi:** Koltuk boyunca sağdan sola yatay pan (Slow horizontal camera glide from right to left)
- **Model Koreografisi:** Koltuğa rahatça yaslanma, hafifçe gülümseme ve kameraya sıcak bir selamlama bakışı

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic luxury loungewear video, shot on 50mm lens. Slow, seamless horizontal camera glide from right to left across the plush armchair. The woman poses with effortless natural charm: relaxing gently into the cushions, slowly turning her gaze, and offering a warm, alluring smile to the camera. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Warm lamp glow, delicate crystal sparkles along fabric folds, 24fps cinematic quality, natural breathing, clean motion.
```

---

### 8. `8 copy.jpg` — Görsel 8 (Şömine Yanında Ayakta Duruş)
- **Kamera Hareketi:** Şömine mermerinden modele doğru yavaş yatay pan (Slow horizontal pan from mantle to model)
- **Model Koreografisi:** Gövdeyi hafifçe kameraya çevirme, çeneyi hafif düşürüp albenili bakış atma

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic high-end evening loungewear video, shot on 50mm lens. Slow, perfectly stabilized horizontal pan tracking from the fireplace mantel to the standing model. The woman poses with sophisticated allure: slowly turning her upper torso toward the lens and holding a confident, poised expression with alluring eyes. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Warm fireplace reflections, authentic crystal sparkles across the stone motifs, 24fps filmic look, lifelike stability.
```

---

### 9. `9 copy.jpg` — Görsel 9 (Bench Üzerinde Oturuş)
- **Kamera Hareketi:** Oturma hattı boyunca soldan sağa yavaş pan (Slow horizontal pan across the bench)
- **Model Koreografisi:** Gözlerini yavaşça yukarı kaldırıp kameraya bakma, dingin ve merak uyandıran ifade

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic luxury bedroom video, shot on 50mm prime lens. Slow, smooth horizontal camera pan gliding across the velvet bench. The woman poses with quiet elegance: breathing gently with hands resting gracefully, slowly raising her gaze to look directly at the camera with subtle allure and a calm expression. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Warm ambient lighting, shimmering crystal motifs, 24fps photorealistic physics, completely stable.
```

---

### 10. `10 copy.jpg` — Görsel 10 (Yastıklara Yaslanış)
- **Kamera Hareketi:** Yatak başlığı boyunca yavaş yatay pan (Slow horizontal pan across the plush cushions)
- **Model Koreografisi:** Yastıklara hafifçe daha rahat gömülme, başı tatlıca eğme ve sevimli albenili gülümseme

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic luxury sleepwear video, shot on 50mm lens. Very slow, steady horizontal camera pan across the headboard cushions. The young woman poses with relaxed charm: leaning back gently into the pillows and tilting her head in ultra-slow motion with a radiant, playful, yet tasteful smile. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Soft bedside lamplight, delicate crystal sparkles, filmic depth of field, 24fps organic motion, pristine anatomy.
```

---

### 11. `11 copy.jpg` — Görsel 11 (Odanın Ortasında Ayakta Asil Duruş)
- **Kamera Hareketi:** Geniş açıdan modele doğru yavaş panoramik pan (Slow panoramic sweep framing her full silhouette)
- **Model Koreografisi:** Derin ve sakin bir nefes alma, göğsün hafif yükselmesi, başın ışığa ve kameraya ağır dönüşü

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic luxury fashion editorial video, shot on 50mm lens. Slow, majestic horizontal panoramic sweep framing the woman standing in the grand bedroom suite. She poses with statuesque grace: breathing softly, her chest gently rising, slowly turning her gaze to the lens with calm, regal allure without any exaggerated movements. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Warm lighting cascading along the fabric, crystal stone lines glittering realistically, 24fps, steady and flawless.
```

---

### 12. `12 copy.jpg` — Görsel 12 (Kanepede Başı Ele Yaslama)
- **Kamera Hareketi:** Kanepe kolu boyunca soldan sağa yavaş pan (Slow horizontal pan along the settee armrest)
- **Model Koreografisi:** Yanağını eline hafifçe daha rahat bırakma, gözlerini yumuşakça kırpıp kamerayı süzen bakış

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic loungewear video, shot on 50mm lens. Extremely slow and steady horizontal camera pan gliding along the velvet sofa arm. The woman poses with soft intimacy: gently shifting her position, resting her cheek comfortably against her hand, and looking into the lens with alluring, playful eyes and a subtle smile. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Warm cozy room lights, sparkling rhinestone motifs, creamy bokeh, 24fps authentic fabric physics, hyper-realistic.
```

---

### 13. `13 copy.jpg` — Görsel 13 (Makyaj Pufunda Duruş)
- **Kamera Hareketi:** Ayna yansımasından modele doğru yavaş yatay pan (Slow horizontal pan from mirror reflection to model)
- **Model Koreografisi:** Omzunun üzerinden geriye doğru ağır çekimde bakış atma, zarif dudak kıvrımı ve tebessüm

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic boudoir fashion video, shot on 50mm lens. Slow, elegant horizontal pan moving gracefully past the vanity mirror toward the seated model. The woman poses tastefully: slowly turning her gaze over her shoulder toward the camera, smiling with enchanting, understated allure. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Warm vanity bulb glow, vibrant crystal glints, filmic 24fps cadence, natural skin tones, perfectly stable.
```

---

### 14. `14 copy.jpg` — Görsel 14 (Pencere Önünde Duruş)
- **Kamera Hareketi:** Pencere manzarasından modele doğru yatay pan (Slow horizontal pan from window edge to model)
- **Model Koreografisi:** Şehir ışıklarından bakışlarını yavaşça kameraya çevirme, vakur ve dingin albeni

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic luxury nightwear video, shot on 50mm lens. Slow, fluid horizontal tracking pan moving from the window view to the standing model. The woman poses with poised elegance: slowly turning her head from the evening city lights toward the camera, holding a calm, alluring gaze with effortless grace. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Contrast between exterior bokeh and warm ambient room light, sparkling crystal motifs, 24fps filmic motion, seamless.
```

---

### 15. `15 copy.jpg` — Görsel 15 (Antika Koltukta Asil Duruş)
- **Kamera Hareketi:** Koltuk gövdesi boyunca soldan sağa yavaş pan (Slow horizontal pan across the antique armchair)
- **Model Koreografisi:** Asil bir diklikte sakin nefes alma, gözleri yavaşça kırpma ve gizemli hafif tebessüm

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic luxury fashion editorial video, shot on 50mm lens. Ultra-slow, stable horizontal camera pan gliding across the ornate armchair. The woman poses with regal stillness: blinking softly in luxury slow pacing, maintaining a magnetic, alluring gaze at the camera with a faint, enigmatic half-smile. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Warm ambient interior, crystal stone bands sparkling brilliantly, 24fps filmic smoothness, pristine anatomy.
```

---

### 16. `16 copy.jpg` — Görsel 16 (Yatak Başlığında Minimalist Duruş)
- **Kamera Hareketi:** Kadife başlık boyunca sağdan sola yatay pan (Slow horizontal pan across the velvet headboard)
- **Model Koreografisi:** Sakin bir nefes veriş, başın mindere hafifçe eğilmesi ve samimi büyüleyici bakış

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic intimate bedroom video, shot on 50mm prime lens. Slow, gentle horizontal camera pan gliding across the velvet headboard. The woman poses with relaxed charm: exhaling gently, slowly tilting her head against the plush cushion with an alluring, intimate expression and soft eye contact. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Dim amber bedside light, delicate scattered crystal glimmers, dreamy atmosphere, 24fps fluid motion, hyper-realistic.
```

---

### 17. `17 copy.jpg` — Görsel 17 (Yaldızlı Ayna Yanında Duruş)
- **Kamera Hareketi:** Ayna çerçevesinden modele doğru yavaş yatay pan (Slow horizontal pan from gilded mirror to model)
- **Model Koreografisi:** Gözlerini aynadaki yansımasından kameraya yavaşça çevirme, kendine güvenen çekici tebessüm

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic luxury lifestyle video, shot on 50mm lens. Slow, smooth horizontal camera pan moving past the ornate gilded mirror toward the model. The woman poses with captivating confidence: slowly shifting her eyes from the mirror to the camera with an alluring, poised smile and statuesque posture. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Warm chandelier reflections, crisp crystal stone glints, 24fps boutique cinematography, flawless.
```

---

### 18. `18 copy.jpg` — Görsel 18 (Sedirde Bacak Bacak Üstüne Atış)
- **Kamera Hareketi:** Sedir boyunca soldan sağa yatay pan (Slow horizontal pan across the ivory settee)
- **Model Koreografisi:** Duruşunu sakin bir zarafetle tazeleme, gözlerini hafif indirip sonra kameraya kaldırma

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic high-end loungewear video, shot on 50mm lens. Slow, graceful horizontal camera pan tracking across the ivory settee. The woman poses in serene, ultra-slow motion: subtly shifting her seated posture, briefly lowering her gaze, and then lifting her eyes to the camera with calm, magnetic poise. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Rich warm interior tones, vertical crystal lines shimmering continuously, 24fps filmic cadence, steady and photorealistic.
```

---

### 19. `19 copy.jpg` — Görsel 19 (Halının Üzerinde Rahat Oturuş)
- **Kamera Hareketi:** Düşük açıdan soldan sağa yatay pan (Slow low-angle horizontal pan across the rug)
- **Model Koreografisi:** Pufa hafifçe daha rahat yaslanma, ellere dokunmadan kendine güvenen modern bir tebessüm sunma

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic modern luxury loungewear video, shot on 50mm lens. Slow, steady low-angle horizontal camera pan across the plush rug. The woman poses with effortless, relaxed charm: leaning back slightly against the ottoman, offering a calm, confident half-smile into the lens with bright, captivating eyes. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Diffused warm room light, crystal lettering twinkling subtly, clean aesthetic, 24fps organic micro-movements, stable limbs.
```

---

### 20. `20 copy.jpg` — Görsel 20 (Kemerli Kapı Önünde Duruş)
- **Kamera Hareketi:** Kemer mimarisinden modele doğru panoramik pan (Slow horizontal panoramic pan around the archway)
- **Model Koreografisi:** Üst gövdeyi yavaşça kameraya doğru döndürme, dökümlü sırtın hafif oturması, büyüleyici gülümseme

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic fashion catalog video, shot on 50mm lens. Slow, controlled horizontal panoramic pan moving past the warm archway toward the standing model. The woman poses with statuesque grace: slowly turning her upper torso toward the camera, holding an exquisite, alluring gaze with a gentle smile. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Warm golden background glow, crystal clusters gleaming softly, 24fps filmic smoothness, hyper-realistic.
```

---

### 21. `21 copy.jpg` — Görsel 21 (Makyaj Koltuğunda Oturuş)
- **Kamera Hareketi:** Makyaj masası hattında soldan sağa yavaş pan (Slow horizontal slider pan across the vanity)
- **Model Koreografisi:** Hafif bir nefes alma, başı tatlı bir açıyla yana eğme ve genç büyüleyici bir tebessüm

**Google Flow / Veo Promptu (Doğrudan Kopyalayın):**
```text
Cinematic luxury sleepwear video, shot on 50mm prime lens. Slow, seamless horizontal slider pan gliding across the vanity area. The young woman poses with captivating grace: breathing softly, tilting her head in slow, gentle motion, and smiling warmly into the camera with radiant allure. Maintain 100% strict visual consistency with the reference image: preserve the exact original garment, fabric color, and crystal rhinestone pattern without any alteration. Zero color shift, zero dress morphing, zero pattern distortion. Soft golden vanity lighting, crystal dot patterns glistening delicately, dreamy depth of field, 24fps, natural skin tones, photorealistic.
```

---
