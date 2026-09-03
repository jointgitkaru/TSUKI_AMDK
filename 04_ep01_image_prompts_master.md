# TSUKI_AMDK — Guia Mestre de Prompts de Imagem (Episódio 01 & Assets Canônicos)
### Sistema de Produção Visual: Google Flow / Nano Banana / Gemini 3.7 Pro Image / ComfyUI

---

## 🧭 Índice do Sistema de Prompts de Imagem
1. [Arquitetura de Derivação e Regra de Ouro (Âncora → Derivações)](#1-arquitetura-de-derivação-e-regra-de-ouro)
2. [PACOTE DE PERSONAGENS — Prompts de Imagem (Turnaround & Expressões)](#2-pacote-de-personagens)
   - 2.1 Tsuki (`TSUKI_AMDK_CHAR_TSUKI_MASTER_V001`) — Âncora, 8 Cardinais, Poses & Closes
   - 2.2 Simba (`TSUKI_AMDK_CHAR_SIMBA_MASTER_V001`) — Âncora, 8 Cardinais, Poses & Closes
   - 2.3 Escala & Interação (`TSUKI_AMDK_CHAR_INTERACTION_MASTER_V001`) — Planos Conjuntos a 40cm
3. [PACOTE DO CENÁRIO — A Cozinha (`TSUKI_AMDK_LOC_KITCHEN_MASTER_WIDE_V001`)](#3-pacote-do-cenário--a-cozinha)
   - 3.1 Prompt-Âncora do Ambiente
   - 3.2 8 Direções Cardinais & Ordinais (Norte, Sul, Leste, Oeste, NE, NO, SE, SO)
   - 3.3 Variações de Iluminação do Ep01 (14h31 Início vs 18h04 Entardecer Dourado)
   - 3.4 Elevações & Câmeras Canônicas (25cm Chão, 90cm Balcão, 1.2m Master, 15cm Macro)
4. [PACOTE DE OBJETOS & PROPS DO EP01](#4-pacote-de-objetos--props-do-ep01)
   - 4.1 Pasta de Arquivo do Dossiê (`TSUKI_AMDK_PROP_CASE_FOLDER`) — Fechada Sem Carimbo, Aberta com Autos, Fechada com Carimbo Bordô
   - 4.2 Tigela de Cerâmica & Tapete de Juta (`TSUKI_AMDK_PROP_BISCUIT_BOWL`) — Master, Top-Down, 45°, Macro Piso Sem Migalhas
   - 4.3 O Biscoito Canônico (`TSUKI_AMDK_PROP_DOG_BISCUIT`) — Master Isolado
5. [KEYFRAMES DE CENA (SHOTS 01 A 09 — EPISÓDIO 01)](#5-keyframes-de-cena-shots-01-a-09)
   - SH001: Start Keyframe — Abertura da Pasta (Macro Etiqueta 14h31) + End Keyframe (Pasta Aberta)
   - SH002: Start Keyframe — Entrada de Tsuki na Porta Sul (25cm do Chão)
   - SH003: Start Keyframe — Tsuki a 20cm da Tigela Vazia (MCU Investigativo)
   - SH004: Start Keyframe — Detalhe Macro do Assoalho sem Migalhas (10cm do Chão)
   - SH005: Start Keyframe — Two-Shot de Interrogatório (Tsuki no Piso vs Simba no Balcão a 40cm)
   - SH006: Start Keyframe — Close-up de Simba no Balcão (Olhar Sereno Ice Blue)
   - SH007: Start Keyframe — Close-up de Tsuki Inclinando a Cabeça 2mm (Olhar Dark Brown)
   - SH008: Start Keyframe — Vigilância da Tigela ao Entardecer Dourado (Tsuki Deitada)
   - SH009: Start Keyframe — Fechamento da Pasta (Aberta) + End Keyframe (Carimbo Bordô "CLASSIFICADO: ABERTO")
6. [AUDITORIA DE CONTINUIDADE (12 Pontos & Matriz de Transições)](#6-auditoria-de-continuidade)

---

## 1. Arquitetura de Derivação e Regra de Ouro

```
                    [ 00_MASTER_ANCHOR_IMAGE ]
               (Primeira imagem gerada e travada)
                                 │
     ┌───────────────────────────┼───────────────────────────┐
     ▼                           ▼                           ▼
[ 8 ÂNGULOS CARDINAIS ]   [ EXPRESSÕES & DETALHES ]   [ KEYFRAMES DE CENA ]
 (Turnaround 0° a 315°)     (Closes, Olhos, Pelo)     (Shots 01 a 09 no Veo)
     │                           │                           │
     └───────────────────────────┴───────────────────────────┘
                                 │
               Reenvio SEMPRE da @MASTER_ANCHOR
                (NUNCA em cascata da anterior)
```

> **Regra de Ouro da Continuidade de Imagem:**  
> Cada derivação deve referenciar a imagem-mestra original (`@MASTER_ANCHOR`). Nunca gere uma derivação usando a imagem gerada no passo anterior, pois isso causa *drift* cumulativo de geometria, anatomia e iluminação.

---

## 2. PACOTE DE PERSONAGENS

### 2.1 TSUKI (`TSUKI_AMDK_CHAR_TSUKI_MASTER_V001`)
* **Espécie/Raça:** Fêmea Adulta, Schnauzer Miniatura (1-2 anos)
* **Altura na Cernelha:** 33 cm | **Postura:** Alerta, ereta, forense, cauda natural curvada (NÃO cortada)
* **Paleta Canônica:** Topcoat Cinza Escuro (`#4A4C50`), Sobrancelhas Cinza Claro (`#9B9E9F`), Barba/Patas Creme (`#E6DEC8`), Focinho/Lábios Bege Quente (`#D4B89B`), Trufa/Base Preto Carvão (`#1C1D1F`), Olhos Castanho Escuro (`#2B1D16`).

#### 📷 Prompt 2.1.0 — IMAGEM-MESTRA ÂNCORA (0° Frontal Master)
```text
Full body reference photograph of an adult female Miniature Schnauzer named Tsuki, front view, standing alert in a dignified investigative stance, facing directly toward the camera. 33cm shoulder height, compact and sturdy build. Dense wiry dark charcoal-gray topcoat (#4A4C50), distinct light silver-gray expressive bushy eyebrows (#9B9E9F), soft off-white cream beard and leg furnishings (#E6DEC8), warm beige tint around the mouth and lips (#D4B89B), charcoal black nose (#1C1D1F), and deep dark brown analytical eyes (#2B1D16). Natural un-docked tail curved gently over the back. Natural V-folded ears. Clean female ventral anatomy. Plain neutral studio gray background, soft diffused even lighting with no harsh cast shadows. Eye-level camera, natural 50mm lens perspective with zero wide-angle distortion. Authentic 16mm film stock texture, organic fine grain, tactile wiry fur detail. Sharp focus throughout, full body in frame, all four paws resting on the floor line.
```

#### 📷 Prompts 2.1.1 a 2.1.7 — TURNAROUND CARDINAL (Reenviando @TSUKI_MASTER_V001)

* **45° Três-Quartos Frontal Direito (`TSUKI_CHAR_TURN_45_R`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_TSUKI_MASTER_V001, generate the exact same character — identical Miniature Schnauzer female, identical dark gray wiry coat (#4A4C50), light gray eyebrows (#9B9E9F), cream beard (#E6DEC8), warm beige mouth tint (#D4B89B), dark brown eyes (#2B1D16), and natural un-docked curved tail — now shown in a three-quarter front view, rotated 45 degrees to the dog's right. Keep the same neutral gray background, same soft diffused studio lighting, same camera height (33cm eye-level), and same 50mm lens perspective. Standing alert investigative pose. Do not alter her anatomy, breed features, or proportions — only the viewing angle changes. 16mm analog film texture with organic grain.
```

* **90° Perfil Direito (`TSUKI_CHAR_TURN_90_R`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_TSUKI_MASTER_V001, generate the exact same character — identical Miniature Schnauzer female with wiry dark gray coat (#4A4C50), cream furnishings (#E6DEC8), warm beige mouth tint (#D4B89B), and natural un-docked sickle tail curved over back — now shown in a direct side profile view from the right side, rotated 90 degrees. Compact 33cm proportions, straight backline, alert neck posture. Plain neutral gray background, soft even studio lighting, eye-level camera. 16mm analog film grain, tactile fur textures. Only the viewing angle changes.
```

* **135° Três-Quartos Traseiro Direito (`TSUKI_CHAR_TURN_135_R`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_TSUKI_MASTER_V001, generate the exact same character — identical Miniature Schnauzer female — now shown in a three-quarter rear view, rotated 135 degrees. Full view of the natural un-docked sickle tail curving gracefully forward over the dark gray wiry back, back of folded ears, and cream rear leg furnishings. Plain neutral gray background, soft diffused lighting, eye-level camera. 16mm vintage film grain. Only the viewing angle changes.
```

* **180° Traseiro Direto / Costas (`TSUKI_CHAR_TURN_180_BACK`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_TSUKI_MASTER_V001, generate the exact same character — identical Miniature Schnauzer female — seen directly from behind (180 degrees rear view). Natural un-docked tail clearly visible centered and arched upward/forward over the dark gray backcoat, cream fur on hind legs. Symmetrical standing pose. Plain neutral gray background, soft even studio lighting, eye-level camera. 16mm film stock texture. Only the viewing angle changes.
```

* **225° Três-Quartos Traseiro Esquerdo (`TSUKI_CHAR_TURN_225_L`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_TSUKI_MASTER_V001, generate the exact same character — identical Miniature Schnauzer female — now shown in a three-quarter rear view from the left side, rotated 225 degrees. Natural un-docked curved tail over dark gray back, cream furnishings on left legs. Neutral gray studio background, soft even light, eye-level perspective. 16mm analog texture. Only the viewing angle changes.
```

* **270° Perfil Esquerdo (`TSUKI_CHAR_TURN_270_L`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_TSUKI_MASTER_V001, generate the exact same character — identical Miniature Schnauzer female — now shown in a direct side profile view from the left side, rotated 270 degrees. Showing alert head carriage, defined cream beard, dark gray wiry body, and natural curved sickle tail. Neutral gray background, soft even studio lighting, eye-level camera. 16mm film grain. Only the viewing angle changes.
```

* **315° Três-Quartos Frontal Esquerdo (`TSUKI_CHAR_TURN_315_L`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_TSUKI_MASTER_V001, generate the exact same character — identical Miniature Schnauzer female — now shown in a three-quarter front view, rotated 315 degrees (turned toward the dog's left). Alert investigative gaze, dark brown eyes, distinct light gray brows, cream beard with warm beige mouth tint. Neutral gray background, soft diffused lighting, eye-level camera. 16mm analog film stock look. Only the viewing angle changes.
```

#### 📷 Prompts 2.1.8 a 2.1.12 — POSES & EXPRESSÕES PERICIAIS DE TSUKI

* **Pose Forense: Farejamento no Chão (`TSUKI_CHAR_POSE_SNIFF_LOW`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_TSUKI_MASTER_V001, generate the exact same Miniature Schnauzer female in an intense forensic investigative posture. She is standing with her front limbs planted firmly and her snout lowered precisely 5cm from the floor, intently sniffing the ground with documentary-serious concentration. Ears slightly forward, dark brown analytical eyes focused on the floor plane, backline straight, natural tail arched alertly. Neutral studio background or weathered wooden floorboards. Side-lit with soft natural light, 16mm analog film grain, tactile fur detail.
```

* **Pose Forense: Inclinação de Cabeça 2mm (`TSUKI_CHAR_POSE_HEAD_TILT`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_TSUKI_MASTER_V001, generate a medium portrait of Tsuki with her head tilted precisely 2 millimeters to the right in sharp analytical deduction. Her dark brown eyes are wide and deeply focused, bushy light gray eyebrows knit in intense investigative thought, cream beard prominent, zero comedic or cartoonish exaggeration. Serious true-crime procedural documentary tone. Neutral gray background, soft directional side lighting, 16mm vintage film texture.
```

* **Pose Forense: Vigilância Deitada (`TSUKI_CHAR_POSE_PRONE_VIGIL`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_TSUKI_MASTER_V001, generate the exact same Miniature Schnauzer lying down in a sphinx-like vigilant stakeout position. Front paws neatly folded forward, chest resting on the floor, head held alertly 10cm above the ground with chin slightly extended, dark brown eyes wide open and staring fixedly forward into the distance. Natural curved tail resting calmly along her hip. Neutral background or rustic wooden floorboards. Soft warm side lighting, 16mm film stock, organic grain.
```

* **Macro Detalhe: Focinho e Barba (`TSUKI_CHAR_DETAIL_MUZZLE_BEARD`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_TSUKI_MASTER_V001, generate an extreme macro close-up of Tsuki's muzzle, nose, and beard. Textured charcoal black leather nose (#1C1D1F) with subtle moisture, warm beige tint around the mouth lips (#D4B89B), and individual wiry off-white cream beard strands (#E6DEC8). Razor-sharp macro focus, soft directional lighting revealing tactile hair textures. Neutral background, 16mm analog film character.
```

* **Macro Detalhe: Olho e Sobrancelha (`TSUKI_CHAR_DETAIL_EYE_BROW`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_TSUKI_MASTER_V001, generate an extreme macro close-up of Tsuki's left eye and brow. Deep dark brown iris (#2B1D16) reflecting a soft window light catchlight, surrounded by fine dark skin, with thick wiry silver-gray eyebrow hairs (#9B9E9F) arching overhead. Analytical, serious investigative expression. 16mm organic film grain, shallow depth of field.
```

---

### 2.2 SIMBA (`TSUKI_AMDK_CHAR_SIMBA_MASTER_V001`)
* **Espécie/Raça:** Macho Sênior, Gato Siamês Seal Point (9+ anos)
* **Comprimento:** 48 cm | **Postura:** Esguia, serena, imóvel, olhar de testemunha com acesso total à verdade
* **Paleta Canônica:** Corpo Fawn/Creme Claro (`#C9B29A`), Máscara e Orelhas Castanho Selo (`#7A5A3A` / `#2B1F19`), Extremidades/Patas/Cauda Carvão Escuro (`#1C1D1F`), Olhos Azul-Gelo (`#A8C7E6`), Trufa Preta/Marrom Escura (`#1C1D1F`).

#### 📷 Prompt 2.2.0 — IMAGEM-MESTRA ÂNCORA (0° Frontal Master)
```text
Full body reference photograph of a senior male Siamese cat (Seal Point) named Simba, front view, sitting upright in an elegant, composed, and tranquil posture, facing directly toward the camera. 48cm slender elongated body build. Short, sleek pale cream fawn body coat (#C9B29A), distinct dark seal brown facial mask (#2B1F19) covering muzzle and eyes, large triangular dark seal ears (#7A5A3A), dark seal brown points on paws, and long slender tapering tail curled neatly against paws. Piercing luminous ice-blue almond-shaped eyes (#A8C7E6) with a calm, all-knowing, unhurried expression. Dark charcoal nose leather (#1C1D1F). Plain neutral studio gray background, soft diffused even lighting with no harsh shadows. Eye-level camera (25cm height), natural 50mm lens perspective. Authentic 16mm film stock texture, fine organic grain, smooth glossy fur sheen. Sharp focus throughout, full body in frame.
```

#### 📷 Prompts 2.2.1 a 2.2.7 — TURNAROUND CARDINAL (Reenviando @SIMBA_MASTER_V001)

* **45° Três-Quartos Frontal Direito (`SIMBA_CHAR_TURN_45_R`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_SIMBA_MASTER_V001, generate the exact same Siamese Seal Point cat — identical pale cream body (#C9B29A), dark seal brown mask (#2B1F19), large triangular ears, ice-blue almond eyes (#A8C7E6), and dark points — now shown in a three-quarter front view, rotated 45 degrees to the cat's right. Sitting composed and dignified. Plain neutral gray background, soft diffused studio lighting, eye-level camera. 16mm analog film stock, organic fine grain. Only the viewing angle changes.
```

* **90° Perfil Direito (`SIMBA_CHAR_TURN_90_R`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_SIMBA_MASTER_V001, generate the exact same Siamese cat — identical slender elongated anatomy, pale cream coat, seal brown face mask, and long dark tapering tail — now shown in a direct side profile view from the right side, rotated 90 degrees. Elegant straight profile, sitting posture. Plain neutral gray background, soft even studio lighting, eye-level camera. 16mm film grain. Only the viewing angle changes.
```

* **135° Três-Quartos Traseiro Direito (`SIMBA_CHAR_TURN_135_R`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_SIMBA_MASTER_V001, generate the exact same Siamese cat — identical cream coat and dark seal brown ears and tail — now shown in a three-quarter rear view, rotated 135 degrees. Slender spine contour, dark seal points on hind legs and tail tip. Plain neutral gray background, soft even light, eye-level perspective. 16mm film texture. Only the viewing angle changes.
```

* **180° Traseiro Direto / Costas (`SIMBA_CHAR_TURN_180_BACK`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_SIMBA_MASTER_V001, generate the exact same Siamese cat seen directly from behind (180 degrees rear view). Symmetrical sitting posture, pale cream shoulders, dark seal brown back of triangular ears, and long dark tail wrapping neatly around the base. Plain neutral gray background, soft even studio lighting, eye-level camera. 16mm vintage film grain. Only the viewing angle changes.
```

* **225° Três-Quartos Traseiro Esquerdo (`SIMBA_CHAR_TURN_225_L`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_SIMBA_MASTER_V001, generate the exact same Siamese cat — identical seal point markings — now shown in a three-quarter rear view from the left side, rotated 225 degrees. Slender cream body, dark ears and tail. Neutral gray studio background, soft diffused lighting, eye-level camera. 16mm analog texture. Only the viewing angle changes.
```

* **270° Perfil Esquerdo (`SIMBA_CHAR_TURN_270_L`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_SIMBA_MASTER_V001, generate the exact same Siamese cat — identical anatomy and color points — now shown in a direct side profile view from the left side, rotated 270 degrees. Sitting upright, calm demeanor, dark mask and long tail clearly defined. Plain neutral gray background, soft even studio lighting, eye-level camera. 16mm film grain. Only the viewing angle changes.
```

* **315° Três-Quartos Frontal Esquerdo (`SIMBA_CHAR_TURN_315_L`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_SIMBA_MASTER_V001, generate the exact same Siamese cat — identical cream body, seal mask, and ice-blue eyes (#A8C7E6) — now shown in a three-quarter front view, rotated 315 degrees (turned toward the cat's left). Calm and serene expression, sitting poised. Plain neutral gray background, soft even studio lighting, eye-level camera. 16mm vintage film look. Only the viewing angle changes.
```

#### 📷 Prompts 2.2.8 a 2.2.11 — POSES & EXPRESSÕES DE TESTEMUNHA DE SIMBA

* **Pose: Poleiro no Balcão de 90cm (`SIMBA_CHAR_POSE_COUNTER_PERCH`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_SIMBA_MASTER_V001, generate Simba perched upright on the edge of a 90cm high rustic wooden kitchen counter, looking down at a 45-degree angle toward the floor. His front paws are neatly aligned together at the wooden countertop edge, long seal brown tail draped elegantly downward along the counter side, ice-blue eyes gazing calmly below with total serenity. Soft afternoon window light from side, warm rustic kitchen background in soft focus, 16mm film stock, organic grain.
```

* **Expressão: O Piscar Lento de Olhos (`SIMBA_CHAR_EXPR_SLOW_BLINK`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_SIMBA_MASTER_V001, generate an intimate eye-level portrait of Simba's face in the middle of a slow, deliberate blink. His ice-blue eyes (#A8C7E6) are half-closed in a relaxed, tranquil, enigmatic expression of calm feline observation. Fine seal-brown facial fur, white whisker strands catching the light. Dark background, soft natural window catchlight, 16mm analog film stock, shallow depth of field.
```

* **Macro Detalhe: Olhos Azul-Gelo (`SIMBA_CHAR_DETAIL_ICE_BLUE_EYES`):**
```text
Using the attached reference image @TSUKI_AMDK_CHAR_SIMBA_MASTER_V001, generate an extreme macro close-up centered on Simba's ice-blue almond-shaped eyes (#A8C7E6). Clear translucent crystalline iris with delicate dark radial striations, dark vertical slit pupils, surrounded by velvety dark seal brown mask fur (#2B1F19). Soft diffused highlight reflection in the cornea. 16mm organic fine grain, razor-sharp focus.
```

---

### 2.3 ESCALA & INTERAÇÃO (`TSUKI_AMDK_CHAR_INTERACTION_MASTER_V001`)

#### 📷 Prompt 2.3.1 — ESCALA CANÔNICA NO PISO (Piso a Piso a 40cm)
```text
Full body reference photograph establishing the exact scale relationship between Tsuki (@TSUKI_AMDK_CHAR_TSUKI_MASTER_V001) and Simba (@TSUKI_AMDK_CHAR_SIMBA_MASTER_V001) both on the same floor level. Tsuki (female Miniature Schnauzer, 33cm shoulder height, sturdy dark gray wiry coat, cream beard) stands on the left in an alert posture. Simba (senior Siamese cat, 48cm body length, slender cream coat, seal brown points) sits on the right in an upright pose. Exactly 40cm distance separates them face-to-face. Tsuki's head height sits slightly higher than Simba sitting, while Simba appears longer, leaner, and more elongated. Worn pine wood floorboards, plain neutral studio gray wall behind. Soft even diffused lighting, camera positioned at 30cm ground level, 50mm natural lens. 16mm vintage film grain.
```

#### 📷 Prompt 2.3.2 — ASSIMETRIA ESPACIAL BALCÃO / PISO (Interrogatório Ep01)
```text
Medium two-shot reference establishing vertical height and spatial asymmetry between Tsuki (@TSUKI_AMDK_CHAR_TSUKI_MASTER_V001) and Simba (@TSUKI_AMDK_CHAR_SIMBA_MASTER_V001). Tsuki stands firmly on the wooden kitchen floor at the base of the counter, looking upward at a sharp 45-degree angle with unwavering investigative focus. Simba is perched calmly on the 90cm high rustic wooden countertop directly above, looking straight down at Tsuki with tranquil, unblinking ice-blue eyes. Exactly 40cm horizontal baseline distance. Lived-in rustic kitchen environment, soft daylight streaming from the north window on the right, warm tungsten fill. 16mm analog film stock, rich shadows, documentary realism.
```

---

## 3. PACOTE DO CENÁRIO — A COZINHA

### 3.1 Prompt-Âncora do Ambiente (Fixo para Toda a Temporada)
```text
CANONICAL KITCHEN ENVIRONMENT ANCHOR:
Interior of a warm, lived-in, rustic domestic kitchen with natural patina and authentic domestic wear. Flooring is aged, matte pine wood floorboards with visible natural grain, subtle knots, and slight color variations (#8C6D4F / #B5936E). On the North wall: a large dark iron-framed window with small rectangular panes looking out to a green domestic yard, letting in soft natural daylight. In the Northwest corner: a rustic wooden countertop at 90cm height with a classic white ceramic sink and brass faucet. In the Northeast corner: a solid dark wooden dining table with two matching ladder-back wooden chairs. Along the East-center wall: the dedicated pet feeding station consisting of a small circular woven jute mat and a glazed cream ceramic pet bowl. On the South wall: an open doorway leading to the wooden hallway corridor. Warm tungsten practical ambient light balancing the cool exterior window daylight. Authentic 16mm film stock, organic fine grain, tactile physical textures, no digital shine.
```

### 3.2 8 Direções Cardinais & Ordinais (Câmera no Centro a 1.2m de Altura)

* **📷 3.2.1 CARDINAL NORTE (`LOC_KITCHEN_CARDINAL_NORTH` — Janela & Quintal):**
```text
[CANONICAL KITCHEN ENVIRONMENT ANCHOR]. Wide architectural reference shot with camera positioned at the center of the kitchen at 1.2m height, looking directly NORTH toward the large dark iron-framed window. The window frames the soft green yard outside and floods the room with soft directional afternoon daylight. Rustic pine wood floorboards run vertically in perspective. In the far left, the edge of the wooden counter; in the far right, the side of the wooden dining table. Balanced exposure, soft atmospheric dust motes, 16mm vintage film grain.
```

* **📷 3.2.2 CARDINAL SUL (`LOC_KITCHEN_CARDINAL_SOUTH` — Porta & Corredor):**
```text
[CANONICAL KITCHEN ENVIRONMENT ANCHOR]. Wide architectural reference shot with camera positioned at the center of the kitchen at 1.2m height, looking directly SOUTH toward the open wooden doorway leading into the darker hallway corridor. The warm pine floorboards continue into the corridor. Warm interior tungsten ceiling fixture creates soft, ambient rim light around the doorframe. Natural shadow falloff into the kitchen corners. 16mm analog film texture.
```

* **📷 3.2.3 CARDINAL OESTE (`LOC_KITCHEN_CARDINAL_WEST` — Balcão, Pia & Geladeira):**
```text
[CANONICAL KITCHEN ENVIRONMENT ANCHOR]. Wide architectural reference shot with camera positioned at the center of the kitchen at 1.2m height, looking directly WEST toward the kitchen workspace. The 90cm high wooden countertop with integrated white ceramic sink, vintage brass faucet, and retro cream-colored refrigerator along the wall. Side daylight from the north window on the right skims across the wooden counter surface. Tactile wood and ceramic textures, 16mm organic grain.
```

* **📷 3.2.4 CARDINAL LESTE (`LOC_KITCHEN_CARDINAL_EAST` — Mesa & Estação de Alimentação):**
```text
[CANONICAL KITCHEN ENVIRONMENT ANCHOR]. Wide architectural reference shot with camera positioned at the center of the kitchen at 1.2m height, looking directly EAST toward the dining area and feeding station. Solid wooden dining table and chairs against the wall. On the floor in the foreground-right: the small circular woven jute mat and clean cream ceramic bowl. Light from the north window on the left casts long gentle shadows toward the east wall. 16mm vintage film aesthetic.
```

* **📷 3.2.5 ORDINAL NORDESTE (`LOC_KITCHEN_ORDINAL_NE` — Canto Mesa de Jantar):**
```text
[CANONICAL KITCHEN ENVIRONMENT ANCHOR]. Wide architectural shot looking into the NORTHEAST corner of the kitchen. Showing the junction between the north iron window wall and the east dining area, framing the rustic wooden table, chair legs on pine floorboards, and the soft diffused light pooling in the corner. 16mm film stock, organic grain.
```

* **📷 3.2.6 ORDINAL NOROESTE (`LOC_KITCHEN_ORDINAL_NW` — Canto Balcão de Simba):**
```text
[CANONICAL KITCHEN ENVIRONMENT ANCHOR]. Wide architectural shot looking into the NORTHWEST corner of the kitchen. Showing the junction between the north window and the 90cm wooden countertop and ceramic sink where Simba perches. Bright natural window light falling directly across the corner counter. 16mm vintage film grain.
```

* **📷 3.2.7 ORDINAL SUDESTE (`LOC_KITCHEN_ORDINAL_SE` — Canto Corredor / Estação de Ração):**
```text
[CANONICAL KITCHEN ENVIRONMENT ANCHOR]. Wide architectural shot looking into the SOUTHEAST corner of the kitchen. Showing the area between the feeding station mat and the corridor entrance. Warm tungsten wall glow, deep cozy domestic shadows, 16mm film grain.
```

* **📷 3.2.8 ORDINAL SUDOESTE (`LOC_KITCHEN_ORDINAL_SW` — Canto Geladeira / Passagem):**
```text
[CANONICAL KITCHEN ENVIRONMENT ANCHOR]. Wide architectural shot looking into the SOUTHWEST corner of the kitchen. Showing the base of the refrigerator and the side wall meeting the hallway entrance. Rich shadow gradients, tactile pine floor wear, 16mm organic texture.
```

### 3.3 Variações de Iluminação do Episódio 01

* **📷 3.3.1 Início da Investigação (14h31-14h42 — Luz Natural de Início de Tarde):**
```text
[CANONICAL KITCHEN ENVIRONMENT ANCHOR]. Lighting state for early afternoon (14h31). Bright, clean, diffused directional daylight streaming at a 60-degree angle from the North iron window across the central floorboards. High dynamic range with soft shadow roll-off. Balanced interior tungsten practicals. Crisp forensic clarity, tactile wood fibers, 16mm vintage film stock.
```

* **📷 3.3.2 Encerramento / Vigília (18h04 — Entardecer Dourado / Golden Hour):**
```text
[CANONICAL KITCHEN ENVIRONMENT ANCHOR]. Lighting state for late sunset / golden hour (18h04). Low-angle warm amber and golden sunlight piercing horizontally through the North window, casting long dramatic orange shadows across the entire floor up to the East feeding station. Melancholic, quiet, contemplative atmosphere. Rich analog halation, deep tungsten room tone, 16mm organic grain.
```

### 3.4 Elevações & Câmeras Canônicas da Cozinha

* **📷 3.4.1 Câmera ao Nível do Chão (25cm — Tsuki POV):**
```text
[CANONICAL KITCHEN ENVIRONMENT ANCHOR]. Low-angle medium-wide shot positioned exactly 25cm above the pine floorboards. Raking low light reveals the physical texture, grain, and subtle knots of the wood planks in the sharp foreground, leading up to the ceramic pet bowl on the jute mat in the midground. Table and counter legs rise into the upper frame. 16mm analog documentary look.
```

* **📷 3.4.2 Câmera Elevada de Observação (90cm — Simba POV):**
```text
[CANONICAL KITCHEN ENVIRONMENT ANCHOR]. High-angle observational shot positioned at 90cm height from the kitchen counter edge, looking downward at a 45-degree angle across the floor space toward the doorway and feeding station. Wide downward perspective of the domestic terrain. 16mm vintage film grain.
```

* **📷 3.4.3 Câmera Macro de Perímetro (10-15cm):**
```text
Macro ground-level close-up (10cm height) focused sharply on the edge of the woven jute mat and the adjacent weathered pine floorboards in the kitchen. Pristine wood surface with fine dust motes and micro-grain, completely free of any biscuit crumbs or saliva marks. Raking side light creating crisp microscopic shadows. 16mm film texture.
```

---

## 4. PACOTE DE OBJETOS & PROPS DO EP01

### 4.1 Pasta de Arquivo do Dossiê (`TSUKI_AMDK_PROP_CASE_FOLDER`)

#### 📷 Prompt 4.1.1 — ESTADO 1: ABERTURA (Capa Fechada Sem Carimbo — Macro Início)
```text
Top-down macro product reference photograph of a closed vintage investigative dossier binder folder (@TSUKI_AMDK_PROP_CASE_FOLDER_UNSTAMPED_KEYFRAME) centered on a dark rustic aged wooden table with deep wood grain. The folder is made of thick, heavy, weathered kraft cardboard with worn creased edges, subtle grease smudges, and oxidized dark metal grommets along the spine. A rectangular white paper label with aged yellowed borders is typed in crisp black typewriter font: "CASO Nº 001 — O Biscoito Que Não Estava Lá | LOCAL: Foi aqui | DATA: 20/08/1996 | HORA: 14h31 | INVESTIGADOR/A: TSUKI". The folder cover is completely clean of any rubber stamps (NO STAMPS). Dramatic directional tungsten side-lighting from the left casting deep noir shadows. 16mm vintage film grain, tactile paper fiber textures.
```

#### 📷 Prompt 4.1.2 — ESTADO 2: PASTA ABERTA (Autos do Processo & Anotações de Tsuki)
```text
Top-down wide reference photograph of the heavy kraft cardboard dossier folder laying completely open on the dark rustic wooden desk. Inside: multiple stacked yellowed case file sheets, typed investigation report pages, carbon-copy forms, and handwritten pencil timeline notes ("14h31 - Biscoito catalogado", "14h37 - Ausência confirmada"). Oxidized metal binder rings holding the thick dossier together. Dramatic warm side lighting, tactile paper texture, coffee cup ring mark on paper corner. 16mm film stock, organic grain, true-crime procedural documentary aesthetic.
```

#### 📷 Prompt 4.1.3 — ESTADO 3: FECHAMENTO (Capa Fechada com Carimbo Bordô Oficial)
```text
Top-down macro reference photograph of the closed kraft cardboard dossier folder (@TSUKI_AMDK_PROP_CASE_FOLDER_MASTER_V001) resting on the dark aged wood. Typed label reads "CASO Nº 001 — O Biscoito Que Não Estava Lá". Prominently stamped across the center-right of the cover in dark crimson/burgundy archival ink (#7A1C1C) is the official rubber stamp: "CASO Nº 001 | CLASSIFICADO: ABERTO" inside a crisp double-lined rectangular border. Slight ink bleed on textured cardboard fiber. Dramatic tungsten side-lighting from the left, deep shadows, 16mm vintage film grain.
```

---

### 4.2 Tigela de Cerâmica & Tapete de Juta (`TSUKI_AMDK_PROP_BISCUIT_BOWL`)

#### 📷 Prompt 4.2.1 — TIGELA MASTER (Visão 45° Frontal)
```text
Product reference photograph of an artisan glazed cream ceramic pet bowl (@TSUKI_AMDK_PROP_BISCUIT_BOWL_MASTER_V001), three-quarter 45-degree view, resting on a small circular natural woven jute mat on worn pine floorboards. Low wide bowl with a smooth off-white glazed interior and a classic cobalt blue hand-painted floral trim around the exterior rim. The bowl is completely empty and clean with a small shallow puddle of clear still water in the bottom. Soft window daylight reflecting on the ceramic glaze. 16mm analog film character, tactile rope and ceramic textures.
```

#### 📷 Prompt 4.2.2 — TIGELA TOP-DOWN (Visão 90° Superior)
```text
Direct top-down (90 degrees overhead) macro photograph of the cream ceramic pet bowl on the circular woven jute mat. Pristine clean white/cream ceramic interior, blue glazed outer lip, surrounded by textured braided jute fibers and adjacent pine floor planks. Soft diffused lighting, crisp focus, 16mm fine film grain.
```

#### 📷 Prompt 4.2.3 — PERÍMETRO FORENSE MACRO (Piso Sem Migalhas a 10cm)
```text
Ground-level macro close-up photograph (10cm height) showing the outer edge of the woven jute mat and the adjacent pine wood floorboards. The wood surface displays rich natural grain, subtle varnish wear, and microscopic dust particles, but is completely and meticulously free of any biscuit crumbs, food residue, or wet marks in a 40cm perimeter. Low-angle raking sunlight highlighting wood texture. 16mm vintage film grain.
```

---

### 4.3 O Biscoito Canônico (`TSUKI_AMDK_PROP_DOG_BISCUIT`)

#### 📷 Prompt 4.3.1 — BISCOITO MASTER (Isolado em Madeira)
```text
Product macro reference photograph of a single artisan baked bone-shaped dog biscuit (@TSUKI_AMDK_PROP_DOG_BISCUIT_MASTER_V001), three-quarter view, resting on aged dark wood. Crunchy, golden-brown baked texture (#B87333 / #8B5A2B) with natural oven blisters, porous baked dough grain, and tiny baked flour flecks. Sharp macro focus, warm soft directional side lighting, 16mm vintage film grain, tactile bakery texture.
```

---

## 5. KEYFRAMES DE CENA (SHOTS 01 A 09 — EPISÓDIO 01)

### 🎬 SHOT 001 — Abertura: A Pasta do Arquivo se Abre
* **Shot ID:** `TSUKI_AMDK_E01_S01_SH001_MASTER` | **Cena:** S01 | **Tipo:** Macro Insert (Top-down)
* **Ingredientes Flow:** `@TSUKI_AMDK_PROP_CASE_FOLDER_UNSTAMPED_KEYFRAME`

#### 📷 SH001 Start Keyframe Prompt (Nano Banana / Gemini Image / Midjourney):
```text
Top-down macro insert keyframe. Tight close-up framing on the typed label of a closed kraft cardboard binder folder: "CASO Nº 001 — O Biscoito Que Não Estava Lá | LOCAL: Foi aqui | DATA: 20/08/1996 | HORA: 14h31 | INVESTIGADOR/A: TSUKI". Weathered kraft cardboard texture with oxidized chrome metal grommets along the spine, resting on dark rustic wood. No rubber stamp on cover. Dramatic tungsten side-lighting from left, deep noir shadows. Shot on 16mm vintage film stock, organic fine grain, tactile cardboard fiber texture. Starting frame for video zoom-out animation.
```

#### 📷 SH001 End Keyframe Prompt:
```text
Top-down medium keyframe showing the same heavy kraft cardboard folder now fully opened on the dark wooden desk, revealing typed case file pages and dossier sheets inside. Camera pulled back to show the full open binder. Warm tungsten side lighting, 16mm film grain.
```

---

### 🎬 SHOT 002 — Entrada de Tsuki na Cozinha
* **Shot ID:** `TSUKI_AMDK_E01_S01_SH002_MASTER` | **Cena:** S01 | **Tipo:** Wide Shot (25cm Low-Angle)
* **Ingredientes Flow:** `@TSUKI_AMDK_CHAR_TSUKI_MASTER_V001`, `@TSUKI_AMDK_LOC_KITCHEN_MASTER_WIDE_V001`

#### 📷 SH002 Start Keyframe Prompt:
```text
Low-angle wide shot keyframe, camera positioned 25cm above the wooden floorboards. Tsuki (@TSUKI_AMDK_CHAR_TSUKI_MASTER_V001, adult female Miniature Schnauzer, dark gray wiry coat, off-white cream beard, dark brown eyes, natural un-docked curled tail) is stepping into the kitchen through the southern doorway on the left of the frame in an alert, methodical investigative walk. Ahead on the wooden floor in the midground-right sits the circular woven mat and empty ceramic bowl (@TSUKI_AMDK_PROP_BISCUIT_BOWL_MASTER_V001). North iron-framed window in the background pouring soft early afternoon daylight across the pine floor. 16mm analog film stock, organic grain, naturalistic documentary cinematography.
```

---

### 🎬 SHOT 003 — Tsuki Examinando a Tigela Vazia
* **Shot ID:** `TSUKI_AMDK_E01_S01_SH003_MASTER` | **Cena:** S01 | **Tipo:** Medium Close-Up (20cm Low-Angle)
* **Ingredientes Flow:** `@TSUKI_AMDK_CHAR_TSUKI_MASTER_V001`, `@TSUKI_AMDK_PROP_BISCUIT_BOWL_MASTER_V001`

#### 📷 SH003 Start Keyframe Prompt:
```text
Medium close-up keyframe at 20cm floor level. Tsuki (@TSUKI_AMDK_CHAR_TSUKI_MASTER_V001) has stopped precisely 20cm in front of the empty cream ceramic bowl on the woven jute mat. Her snout is lowered milimetrically toward the bowl's blue floral rim with intense forensic focus, dark brown analytical eyes inspecting the empty dish, bushy light gray brows furrowed in serious concentration. Soft window daylight from the left rim-lighting her cream beard and wiry dark gray coat. Pine floorboards in shallow depth of field behind. 16mm vintage film grain, intimate true-crime documentary realism.
```

---

### 🎬 SHOT 004 — O Perímetro Forense Sem Migalhas
* **Shot ID:** `TSUKI_AMDK_E01_S01_SH004_MASTER` | **Cena:** S01 | **Tipo:** Macro Insert (10cm Floor Level)
* **Ingredientes Flow:** `@TSUKI_AMDK_PROP_BISCUIT_BOWL_MASTER_V001`

#### 📷 SH004 Start Keyframe Prompt:
```text
Macro insert keyframe at 10cm ground level. Extreme close-up showing the bottom glazed edge of the cream ceramic bowl, the braided border of the natural jute mat, and the surrounding weathered pine floorboards. The floor surface is pristine, showing rich wood grain and fine texture, with absolute zero biscuit crumbs, residue, or moisture anywhere in the frame. Low-angle raking daylight from the north window skimming the wood planks, casting fine micro-shadows. 16mm film stock, crisp analog focus, tactile physical realism.
```

---

### 🎬 SHOT 005 — Contato Visual Tsuki vs Simba (Two-Shot)
* **Shot ID:** `TSUKI_AMDK_E01_S02_SH005_MASTER` | **Cena:** S02 | **Tipo:** Medium Two-Shot (Vertical Asymmetry)
* **Ingredientes Flow:** `@TSUKI_AMDK_CHAR_TSUKI_MASTER_V001`, `@TSUKI_AMDK_CHAR_SIMBA_MASTER_V001`

#### 📷 SH005 Start Keyframe Prompt:
```text
Medium two-shot keyframe establishing height and spatial confrontation. In the lower-left foreground on the wooden floor, Tsuki (@TSUKI_AMDK_CHAR_TSUKI_MASTER_V001, Miniature Schnauzer) stands firmly looking up at a sharp 45-degree angle with unwavering investigative intensity. In the upper-right frame, Simba (@TSUKI_AMDK_CHAR_SIMBA_MASTER_V001, senior Siamese Seal Point cat) is perched upright on the 90cm high rustic wooden countertop, looking straight down at Tsuki with calm, tranquil ice-blue eyes. Exactly 40cm horizontal distance between them. Warm domestic kitchen interior, soft window daylight from north mixing with warm room ambient. 16mm vintage film grain, tense silent confrontation, documentary realism.
```

---

### 🎬 SHOT 006 — O Piscar de Olhos de Simba (Close-Up)
* **Shot ID:** `TSUKI_AMDK_E01_S02_SH006_MASTER` | **Cena:** S02 | **Tipo:** Close-Up (Simba Eye-Level at 90cm)
* **Ingredientes Flow:** `@TSUKI_AMDK_CHAR_SIMBA_MASTER_V001`

#### 📷 SH006 Start Keyframe Prompt:
```text
Eye-level close-up keyframe (90cm height) of Simba (@TSUKI_AMDK_CHAR_SIMBA_MASTER_V001) sitting on the wooden countertop. Direct frontal framing of his face: dark seal brown mask, large triangular ears, and luminous ice-blue almond eyes looking directly into the camera lens with serene, knowing tranquility. Soft natural window catchlight reflecting in both corneas, fine cream body fur visible at neck. Softly blurred warm kitchen background. 16mm analog film stock, organic fine grain, intimate documentary character study.
```

---

### 🎬 SHOT 007 — Tsuki Catalogando a Pista (Close-Up)
* **Shot ID:** `TSUKI_AMDK_E01_S02_SH007_MASTER` | **Cena:** S02 | **Tipo:** Close-Up (Tsuki Looking Upwards)
* **Ingredientes Flow:** `@TSUKI_AMDK_CHAR_TSUKI_MASTER_V001`

#### 📷 SH007 Start Keyframe Prompt:
```text
Low-angle close-up keyframe of Tsuki (@TSUKI_AMDK_CHAR_TSUKI_MASTER_V001) looking upward at a 45-degree angle. Framing focuses tightly on her expressive face: head tilted 2 millimeters to the side in razor-sharp analytical deduction, dark brown eyes wide and calculating, bushy light gray eyebrows, and prominent off-white cream beard. Utterly serious, non-ironic true-crime detective expression. Warm directional ambient light casting subtle shadows under the brow. 16mm film stock, organic grain, tactile wiry fur detail.
```

---

### 🎬 SHOT 008 — Cena de Vigilância ao Entardecer Dourado
* **Shot ID:** `TSUKI_AMDK_E01_S03_SH008_MASTER` | **Cena:** S03 | **Tipo:** Wide Shot (Sunset 18h04)
* **Ingredientes Flow:** `@TSUKI_AMDK_CHAR_TSUKI_MASTER_V001`, `@TSUKI_AMDK_LOC_KITCHEN_MASTER_WIDE_V001`, `@TSUKI_AMDK_PROP_BISCUIT_BOWL_MASTER_V001`

#### 📷 SH008 Start Keyframe Prompt:
```text
Wide shot keyframe of the entire kitchen floor at sunset (18h04). Low golden-hour sunlight streams horizontally through the north iron-frame window, casting long warm amber shadows across the worn pine floorboards. In the foreground-center, Tsuki (@TSUKI_AMDK_CHAR_TSUKI_MASTER_V001) lies in a vigilant stakeout position on the floor, front paws neatly folded and chin resting 10cm in front of the empty ceramic bowl (@TSUKI_AMDK_PROP_BISCUIT_BOWL_MASTER_V001), eyes wide open and alert. In the soft-focus background on the counter, Simba sits quietly watching her vigil. Melancholic, peaceful, atmospheric true-crime procedural tone. 16mm analog film stock, rich golden tones, soft analog halation, organic grain.
```

---

### 🎬 SHOT 009 — Fechamento: A Pasta de Arquivo se Fecha
* **Shot ID:** `TSUKI_AMDK_E01_S03_SH009_MASTER` | **Cena:** S03 | **Tipo:** Macro Insert (Top-down)
* **Ingredientes Flow:** `@TSUKI_AMDK_PROP_CASE_FOLDER_MASTER_V001`

#### 📷 SH009 Start Keyframe Prompt:
```text
Top-down medium-macro keyframe of the opened kraft cardboard dossier folder resting on the dark rustic wooden table, with internal case file pages visible inside. Starting frame for the folder closing animation. Warm tungsten side lighting from the left, 16mm vintage film grain.
```

#### 📷 SH009 End Keyframe Prompt (Frame Final do Episódio 01):
```text
Top-down macro keyframe locked tight on the closed kraft cardboard folder cover (@TSUKI_AMDK_PROP_CASE_FOLDER_MASTER_V001) on dark aged wood. The typed label "CASO Nº 001 — O Biscoito Que Não Estava Lá" is now stamped boldly in dark crimson ink (#7A1C1C) with the official classification: "CASO Nº 001 | CLASSIFICADO: ABERTO" inside a double rectangular border. Sharp macro focus on the textured cardboard fibers, ink bleed, and typed text. Dramatic side tungsten light, deep shadows, 16mm vintage film stock grain. Unresolved melancholy true-crime finale.
```

---

## 6. AUDITORIA DE CONTINUIDADE (12 Pontos & Matriz de Transições)

### 6.1 Auditoria dos 12 Pontos Canônicos

| # | Ponto de Continuidade | Status | Verificação Específica Ep01 |
|---|---|---|---|
| 1 | **Identidade de Personagens** | ✅ APROVADO | Tsuki: Schnauzer Fêmea 33cm, paleta Hex exata, cauda natural. Simba: Siamês Seal Point 48cm, olhos azul-gelo. |
| 2 | **Posição de Personagens** | ✅ APROVADO | Tsuki entra pelo Sul (SH02) → vai à tigela a Leste (SH03) → base do balcão a Oeste (SH05) → volta à tigela (SH08). Simba permanece no balcão a 90cm (SH05, SH06, SH08). |
| 3 | **Direção de Eixo / Tela** | ✅ APROVADO | Tsuki olha à esquerda/cima (45°) para o balcão; Simba olha à direita/baixo (45°) para o chão. Linha de 180° respeitada. |
| 4 | **Geografia do Cenário** | ✅ APROVADO | Janela Norte, Pia/Balcão Noroeste, Mesa Nordeste, Estação Ração Leste, Porta Sul. 100% alinhado nos cardinais. |
| 5 | **Posição de Objetos / Props** | ✅ APROVADO | Tigela sempre sobre tapete de juta no chão a Leste. Pasta de arquivo na mesa de madeira escura. |
| 6 | **Direção da Iluminação** | ✅ APROVADO | Luz natural vinda sempre do Norte (janela), luz de preenchimento tungstênio quente do Sul/teto. |
| 7 | **Linha Temporal (Horário)** | ✅ APROVADO | 14h31 (Abertura SH01) → 14h37 (Chegada SH02-04) → 14h42 (Interrogatório SH05-07) → 18h04 (Vigília / Sunset SH08-09). |
| 8 | **Pelagem & Trajes** | ✅ APROVADO | Pelo aramado sem cortes modernos, barba creme íntegra, máscara e pontos de Simba consistentes em todos os ângulos. |
| 9 | **Estado Emocional** | ✅ APROVADO | Tsuki: Metódica, sem ironia, hiper-focada. Simba: Sereno, paciente, detentor do segredo. |
| 10 | **Lógica de Câmera** | ✅ APROVADO | Câmeras ancoradas no ponto de vista animal (25cm, 10cm, 90cm, 1.2m), sem movimentos gratuitos. |
| 11 | **Linguagem Visual 16mm** | ✅ APROVADO | Textura de película 16mm, grão orgânico, roll-off suave, sem estética 3D digital ou saturação artificial. |
| 12 | **Ambiente Sonoro** | ✅ APROVADO | Passos de unhas na madeira, zumbido de geladeira, acorde menor solitário de piano, farfalhar de papel kraft. |

### 6.2 Matriz de Transições Entre Planos (Shot-to-Shot Matrix)

```
SH001 (Dossiê Aberto 14h31)
  │ Transição: Corte direto para chão da cozinha
  ▼
SH002 (Entrada Porta Sul às 14h37 → Direção Leste)
  │ Transição: Continuidade de movimento até parar a 20cm da tigela
  ▼
SH003 (Tsuki abaixa focinho na tigela vazia)
  │ Transição: Corte no eixo para macro do chão
  ▼
SH004 (Macro 10cm do piso: Perímetro de 40cm limpo)
  │ Transição: Corte para tomada de dois corpos (Two-shot)
  ▼
SH005 (Two-shot: Tsuki no piso a 45° vs Simba no balcão a 90cm)
  │ Transição: Corte no contra-campo para o topo do balcão
  ▼
SH006 (Close-up Simba: Piscar de olhos sereno às 14h42)
  │ Transição: Corte no contra-campo para o chão
  ▼
SH007 (Close-up Tsuki: Inclinação de cabeça de 2mm)
  │ Transição: Elipse temporal suave (14h42 → 18h04 Sunset)
  ▼
SH008 (Plano geral entardecer: Tsuki deitada em vigília na tigela)
  │ Transição: Fade/Dissolve para mesa do dossiê
  ▼
SH009 (Dossiê fechando-se com carimbo bordô: "CASO Nº 001 | CLASSIFICADO: ABERTO")
```

---
*Este documento é o artefato mestre oficial de Prompts de Imagem do Episódio 01 e do Ecossistema TSUKI_AMDK.*
