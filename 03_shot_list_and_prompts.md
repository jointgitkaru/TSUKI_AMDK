# TSUKI_AMDK — Shot List & Prompts: Episódio 01

## Visão Geral da Sequência (9 Planos Principais)

```
S01_SH001: [MACRO INSERT] Abertura: A Pasta de Arquivo se abre (Zoom Out)
S01_SH002: [WS] Tsuki entra na Cozinha (Estabelecedor Sul)
S01_SH003: [MCU / LOW-ANGLE] Tsuki examina a tigela vazia no Oeste
S01_SH004: [MACRO INSERT] Detalhe do assoalho limpo ao redor da tigela
S02_SH005: [TWO-SHOT] Tsuki no chão encarando Simba no Norte (Janela)
S02_SH006: [CU] Simba na janela piscando devagar (Contato visual)
S02_SH007: [CU] Tsuki registrando o piscar com inclinação de 2mm
S03_SH008: [WS] Tsuki deitada ao lado da tigela ao entardecer (Vigília)
S03_SH009: [MACRO INSERT] Fechamento: A Pasta de Arquivo se fecha carimbada (Zoom In)
```

---

## Detalhamento dos Planos & Flow Prompts

### SHOT 001 — Abertura: A Pasta do Arquivo se Abre
* **Shot ID:** `TSUKI_AMDK_E01_S01_SH001_MASTER`
* **Tipo:** Macro Insert Shot (Top-down / Zoom Out)
* **Modelo:** Nano Banana (Keyframe) → Veo 3.1 (Ação)
* **Objetivo:** Estabelecer a abertura do dossiê investigativo sem mãos nem carimbos manuais.

> 🏷️ **FLOW TAGS:** `@Dossie` `@Dossie_Aberto`

#### Prompt Flow:
```text
[SHOT]
Top-down macro insert shot (INSERT), starting tight on label and zooming out.

[SUBJECT & OBJECT]
Using @Dossie. A heavy worn kraft cardboard binder folder (closed, NO rubber stamp) resting on a dark aged rustic wooden table. The camera starts in sharp macro close-up on the typed label: "CASO Nº 001 — O Biscoito Que Não Estava Lá | LOCAL: Foi aqui | DATA: 20/08/1996 | HORA: 14h31 | INVESTIGADOR/A: TSUKI".

[ACTION]
The kraft cardboard cover smoothly opens on its own, transitioning to reveal the open case dossier (@Dossie_Aberto) with thick internal case files and papers inside, while the camera executes a smooth, continuous zoom out / pull back to frame the full open folder resting on the dark textured wood. No human hands, no physical stamps.

[CAMERA]
Smooth continuous zoom out (pull back) starting from a tight macro close-up on the label to a wider top-down view of the opened folder.

[LIGHTING & TEXTURE]
Dramatic directional side lighting from left, warm tungsten glow, rich dark shadows, textured kraft cardboard grain, exposed paper fibers, and aged wood patina.

[VISUAL LANGUAGE]
Shot on 16mm vintage film stock. Organic grain, authentic gate weave, soft exposure imperfections, true crime noir procedural aesthetic.

[AUDIO]
Organic sound of cardboard creaking and paper sheets rustling open, followed by a soft, solitary minor-key piano chord.
```

---

### SHOT 002 — Entrada de Tsuki na Cozinha
* **Shot ID:** `TSUKI_AMDK_E01_S01_SH002_MASTER`
* **Tipo:** Wide Shot (WS) — Low-angle tracking
* **Modelo:** Veo 3.1
* **Objetivo:** Estabelecer a postura investigativa de Tsuki no espaço da cozinha.

> 🏷️ **FLOW TAGS:** `@Tsuki` `@Cozinha_Sul`

#### Prompt Flow:
```text
[SHOT]
Wide shot (WS), camera tracking at 25cm dog eye-level.

[SUBJECT]
Using @Tsuki (female Miniature Schnauzer, salt-and-pepper wiry coat, sculpted brows, beige/caramel mouth stain, cream beard, natural sickle tail intact). Tsuki walks methodically through the southern kitchen doorway into the room with steady, deliberate steps.

[ACTION]
Tsuki enters the frame from left, walking across the rustic pine floorboards with alert, procedural body language.

[ENVIRONMENT]
Using @Cozinha_Sul. Rustic kitchen doorway leading from the dark wood hallway corridor into the kitchen space.

[CAMERA]
Subtle observational handheld tracking moving smoothly parallel to Tsuki's movement, keeping camera 25cm above floor.

[LIGHTING]
Soft ambient interior light mixing with directional daylight entering from the North window in the background.

[VISUAL LANGUAGE]
16mm film stock, organic grain, naturalistic observational cinema. One continuous shot. No cuts.

[AUDIO]
Rhythmic clicking of claws on wooden floorboards, soft room tone, distant wall clock ticking.
```

---

### SHOT 003 — A Constatação da Tigela Vazia
* **Shot ID:** `TSUKI_AMDK_E01_S01_SH003_MASTER`
* **Tipo:** Medium Close-Up (MCU) — Low Angle
* **Modelo:** Veo 3.1
* **Objetivo:** Registrar o momento exato em que Tsuki detecta a ausência do biscoito sob a bancada Oeste.

> 🏷️ **FLOW TAGS:** `@Tsuki` `@Cozinha_Oeste` `@Tigela`

#### Prompt Flow:
```text
[SHOT]
Medium close-up (MCU), camera 20cm from the floor.

[SUBJECT & OBJECT]
Using @Tsuki and @Tigela. Tsuki stops precisely 20cm in front of the empty cream ceramic bowl resting on the woven jute mat near the base of the work counter.

[ACTION]
Tsuki lowers her snout slightly, sniffing the rim of @Tigela and the floor with intense forensic focus. She pauses, lifting her head slowly with deep investigative seriousness.

[ENVIRONMENT]
Using @Cozinha_Oeste. Rustic kitchen counter base, lower wooden cabinet doors, worn pine floorboards.

[CAMERA]
Static observational camera with very subtle handheld breathing, locked at 20cm height.

[LIGHTING]
Side-lit by soft window daylight, accentuating the cream texture of Tsuki's beard and the glazed ceramic rim.

[VISUAL LANGUAGE]
16mm analog texture, shallow depth of field, intimate documentary style.

[AUDIO]
Methodical sniffing sound, quiet breathing, faint refrigerator hum.
```

---

### SHOT 004 — O Perímetro Forense (Inserto)
* **Shot ID:** `TSUKI_AMDK_E01_S01_SH004_MASTER`
* **Tipo:** Macro Insert Shot (Floorboards)
* **Modelo:** Nano Banana (Keyframe)
* **Objetivo:** Comprovar pericialmente a ausência de migalhas no raio de 40cm.

> 🏷️ **FLOW TAGS:** `@Tigela` `@Cozinha_Oeste`

#### Prompt Flow:
```text
[SHOT]
Macro insert close-up at 10cm ground level.

[SUBJECT & OBJECT]
Using @Tigela. The edge of the cream ceramic pet bowl on the woven jute mat and the surrounding wooden floorboards. The floor surface is pristine, with natural wood grain, knots, and zero crumbs or residue anywhere in the frame.

[ENVIRONMENT]
Using @Cozinha_Oeste. Lower cabinet kickboard in the soft background.

[CAMERA]
Static locked-off macro lens.

[LIGHTING]
Raking low-angle sunlight skimming the floor texture, casting soft micro-shadows along the wood grain.

[VISUAL LANGUAGE]
16mm film aesthetic, tactile physical texture, crisp analog focus. No human hands, no text.
```

---

### SHOT 005 — Contato Visual com Simba (Two-Shot)
* **Shot ID:** `TSUKI_AMDK_E01_S02_SH005_MASTER`
* **Tipo:** Two-Shot (Low/High dynamic)
* **Modelo:** Veo 3.1
* **Objetivo:** Estabelecer a assimetria espacial e o confronto silencioso no Norte (Janela).

> 🏷️ **FLOW TAGS:** `@Tsuki` `@Simba` `@Cozinha_Norte`

#### Prompt Flow:
```text
[SHOT]
Medium two-shot establishing height, elevation difference, and distance.

[SUBJECTS]
Using @Tsuki and @Simba.
Tsuki stands on the wooden floor looking up at a 45-degree angle with unwavering investigative focus.
Simba (Siamese seal point cat) is perched calmly on the windowsill above her, looking down directly at Tsuki with piercing ice-blue eyes.

[ACTION]
Both animals remain completely still in sustained eye contact. Tsuki does not bark; Simba does not move. The tension is purely intellectual and observational.

[ENVIRONMENT]
Using @Cozinha_Norte. Large dark iron-frame window with strong afternoon light entering behind Simba.

[CAMERA]
Subtle slow push-in toward the vertical space between them, camera positioned low at floor level.

[LIGHTING]
Warm afternoon window daylight creating soft rim light around Simba and gentle fill on Tsuki.

[VISUAL LANGUAGE]
16mm vintage film, naturalistic animal performance, restrained framing. One continuous shot. No cuts.

[AUDIO]
Total silence in the musical score, low ambient room hum, distant breeze.
```

---

### SHOT 006 — O Piscar de Olhos de Simba (Close-Up)
* **Shot ID:** `TSUKI_AMDK_E01_S02_SH006_MASTER`
* **Tipo:** Close-Up (CU) — Simba
* **Modelo:** Veo 3.1
* **Objetivo:** O beat central: o piscar calmo de Simba e o subtexto de quem sabe a verdade.

> 🏷️ **FLOW TAGS:** `@Simba` `@Cozinha_Norte`

#### Prompt Flow:
```text
[SHOT]
Eye-level close-up (CU) of Simba on the windowsill.

[SUBJECT]
Using @Simba (adult Siamese seal point male, dark seal brown mask, ice-blue almond eyes, serene restrained expression).

[ACTION]
Simba maintains calm, direct eye contact looking downward toward Tsuki. After three seconds of stillness, Simba blinks his ice blue eyes once, very slowly and deliberately, then keeps his gaze steady.

[ENVIRONMENT]
Using @Cozinha_Norte (background softly resolved).

[CAMERA]
Static locked-off portrait lens at windowsill height.

[LIGHTING]
Soft window light reflecting gently in Simba's blue eyes, highlighting fine fur microtexture.

[VISUAL LANGUAGE]
16mm film stock, organic halation, intimate observational cinema.

[AUDIO]
Faint sound of distant breeze outside, quiet natural room tone.
```

---

### SHOT 007 — Tsuki Catalogando a Pista (Close-Up)
* **Shot ID:** `TSUKI_AMDK_E01_S02_SH007_MASTER`
* **Tipo:** Close-Up (CU) — Tsuki
* **Modelo:** Veo 3.1
* **Objetivo:** Reação pericial de Tsuki interpretando o piscar de Simba.

> 🏷️ **FLOW TAGS:** `@Tsuki` `@Cozinha_Norte`

#### Prompt Flow:
```text
[SHOT]
Close-up (CU) of Tsuki looking upward.

[SUBJECT]
Using @Tsuki (female Miniature Schnauzer, dark gray wiry coat, off-white beard with caramel mouth stain, dark brown eyes, sculpted brows).

[ACTION]
Tsuki's dark eyes track Simba's slow blink. Her head tilts two millimeters to the side with razor-sharp analytical concentration. Her expression is utterly serious, devoid of any irony.

[ENVIRONMENT]
Using @Cozinha_Norte (soft background).

[CAMERA]
Static tight shot focused on Tsuki's eyes and brows, camera 20cm from floor.

[LIGHTING]
Warm ambient light with soft shadows under the brow.

[VISUAL LANGUAGE]
16mm film grain, tactile fur detail, documentary realism.

[AUDIO]
Subtle resumption of the minor piano melody with a single poignant note.
```

---

### SHOT 008 — Cena de Vigilância ao Entardecer
* **Shot ID:** `TSUKI_AMDK_E01_S03_SH008_MASTER`
* **Tipo:** Wide Shot (WS) — Sunset / Dusk
* **Modelo:** Veo 3.1
* **Objetivo:** Registro da vigília inabalável de Tsuki diante da tigela vazia.

> 🏷️ **FLOW TAGS:** `@Tsuki` `@Simba` `@Cozinha_Norte` `@Tigela`

#### Prompt Flow:
```text
[SHOT]
Wide shot (WS) of the kitchen floor space looking toward the North window.

[SUBJECTS]
Using @Tsuki, @Simba, and @Tigela.
Tsuki lies on the wooden floorboards with her front paws neatly folded and her chin resting 10cm in front of the clean ceramic bowl (@Tigela). Her eyes remain open and vigilant.
In the soft background, Simba remains seated near the window, quietly watching her.

[ACTION]
Minimal motion. Weakening late afternoon sunlight slowly glides across the floor. Tsuki remains committed to her post.

[ENVIRONMENT]
Using @Cozinha_Norte. Pine floorboards, lower cabinets, large iron-frame window with dusk light.

[LIGHTING]
Sunset light transitioning to dusk, casting long deep shadows across the room.

[VISUAL LANGUAGE]
Analog 16mm film look, warm golden tones, gentle grain, slow fade/dissolve.

[AUDIO]
Quiet room tone, gentle breathing, fading afternoon ambient.
```

---

### SHOT 009 — Fechamento Canônico: A Pasta de Arquivo se Fecha
* **Shot ID:** `TSUKI_AMDK_E01_S03_SH009_MASTER`
* **Tipo:** Macro Insert Shot (Top-down / Zoom In)
* **Modelo:** Veo 3.1
* **Objetivo:** Fechar formalmente o episódio com a pasta se fechando e a exibição do carimbo do status final do caso.

> 🏷️ **FLOW TAGS:** `@Dossie_Aberto` `@Dossie_Carimbado`

#### Prompt Flow:
```text
[SHOT]
Top-down macro insert shot (INSERT), starting wider and zooming in tight.

[SUBJECT & OBJECT]
Starting with @Dossie_Aberto and transitioning to @Dossie_Carimbado. The opened kraft cardboard dossier folder resting on the dark rustic wooden table. The cover has the typed label and is officially stamped in dark crimson ink: "CASO Nº 001 | CLASSIFICADO: ABERTO" inside a double rectangular border.

[ACTION]
The open kraft cover smoothly folds shut on its own over the case papers. As the folder closes firmly, the camera executes a continuous, smooth zoom in (push-in) towards the cover, locking onto the dark crimson rubber stamp (@Dossie_Carimbado) and typed label. No human hands.

[CAMERA]
Smooth continuous zoom in (push-in) moving from a medium top-down view to a tight macro close-up on the stamped classification.

[LIGHTING & TEXTURE]
Dramatic directional side lighting from left, rich tungsten glow, deep noir shadows, tactile cardboard fibers, and dark wood patina.

[VISUAL LANGUAGE]
Shot on 16mm vintage film stock. Organic grain, soft exposure imperfections, authentic procedural archive look.

[AUDIO]
Soft, solid muffled sound of the folder closing shut, followed by the final suspended unresolved minor-key piano chord.
```
