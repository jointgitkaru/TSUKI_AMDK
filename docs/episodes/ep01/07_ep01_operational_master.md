# TSUKI_AMDK — EP01 · MASTER OPERACIONAL
### Operational Master / Production Build A

Status: `WORKING MASTER — RECOMMENDED FOR PRODUCTION`
Episode: `EP01`
Title: `CASO Nº 001 — O Biscoito Que Não Estava Lá`
Duration target: `120s`
Language mode: `PT-BR base + EN production labels`

---

## 1. Lock aplicado nesta build / Applied lock for this build

Este arquivo consolida a versão operacional recomendada do EP01.
Se nada for redefinido manualmente, esta é a versão a seguir em produção.

### Creative lock
- **9 planos** como estrutura oficial de trabalho.
- **Pasta/dossiê** obrigatória na abertura e no fechamento.
- **Zero migalhas** como evidência visual canônica do caso.
- **Nenhum humano visível em quadro**.
- **Simba sabe a verdade**, mas essa verdade existe apenas na camada de pensamento.
- **Biscoito canônico:** biscoito canino de carne desidratada, formato osso.
- **Linguagem visual:** 16mm observacional, física, doméstica, sem glamour e sem CGI-look.

### Spatial lock note / Nota espacial
Há uma divergência entre materiais de cozinha mais amplos e materiais específicos do EP01.
Para esta build operacional:

- a **linha de evidência principal** do episódio fica no **eixo OESTE / base da bancada de trabalho**;
- a tigela é tratada como **zero-point dramático do EP01** nessa linha de ação;
- não usar a variante de staging da estação Leste nesta versão sem uma revisão completa de geografia.

### Dimensional lock / Lock dimensional
Aplicar também `docs/episodes/ep01/16_ep01_dimensional_lock.md` em todos os planos com leitura corporal clara.
Em resumo:
- Tsuki deve ler como **schnauzer miniatura pequeno, compacto, robusto**;
- Simba deve ler como **siamês esguio, leve e menos massivo que Tsuki**;
- nenhum dos dois pode parecer grande demais para a cozinha ou para a tigela.

### Allowed exception / Exceção permitida
A regra geral de “no text” não invalida:
- a **etiqueta datilografada do dossiê**;
- o **carimbo final** `CASO Nº 001 | CLASSIFICADO: ABERTO`.

---

## 2. Hierarquia operacional / Operational source-of-truth hierarchy

### Story truth
1. `docs/core/00_episode_core.md`
2. `docs/episodes/ep01/01_script_ep01.md`
3. `docs/episodes/ep01/02_scene_cards.md`

### Visual truth
1. `docs/core/02_visual_bible.md`
2. `docs/episodes/ep01/04_ep01_image_prompts_master.md`
3. `docs/episodes/ep01/05_ep01_keyframes_nanbanana.md`

### Execution truth
1. `docs/episodes/ep01/03_shot_list_and_prompts.md`
2. `docs/episodes/ep01/07_ep01_operational_master.md`
3. `docs/episodes/ep01/09_ep01_final_prompt_package.md`

---

## 3. Mapa do episódio / Episode map

| Ordem | Timecode | Shot ID | Tipo | Cardinal / Axis | Duração | Função |
|---|---|---|---|---|---:|---|
| 01 | 00:00–00:08 | S01_SH001 | INSERT / TOP-DOWN | TABLE / DOSSIER | 8s | Abertura do universo |
| 02 | 00:08–00:20 | S01_SH002 | WS LOW TRACK | SOUTH → WEST | 12s | Entrada investigativa |
| 03 | 00:20–00:34 | S01_SH003 | MCU LOW | WEST | 14s | Constatação da ausência |
| 04 | 00:34–00:42 | S01_SH004 | MACRO INSERT | WEST | 8s | Prova pericial |
| 05 | 00:42–01:00 | S02_SH005 | TWO-SHOT | NORTH | 18s | Interrogatório silencioso |
| 06 | 01:00–01:10 | S02_SH006 | CU SIMBA | NORTH | 10s | Beat do slow blink |
| 07 | 01:10–01:20 | S02_SH007 | CU TSUKI | NORTH | 10s | Hipótese de Tsuki |
| 08 | 01:20–01:44 | S03_SH008 | WS SUNSET | NORTH / WEST evidence axis | 24s | Vigília ao entardecer |
| 09 | 01:44–02:00 | S03_SH009 | INSERT / TOP-DOWN | TABLE / DOSSIER | 16s | Encerramento canônico |

**Total:** `120s`

---

## 4. Beat-to-voice map / Mapa de falas por bloco

### Tsuki narration
- **VO_TSUKI_01** → SH002–SH003
- **VO_TSUKI_02** → SH004
- **VO_TSUKI_03** → SH005–SH006
- **VO_TSUKI_04** → SH008

### Simba internal thought
- **VO_SIMBA_01** → SH006
- **VO_SIMBA_02** → SH007

### Silence blocks
- **SILENCE_HOLD_01** → centro de SH005
- **SILENCE_HOLD_02** → após slow blink em SH006
- **SILENCE_HOLD_03** → antes do fechamento do dossiê em SH009

---

# 5. Decupagem operacional por plano / Shot-by-shot operational breakdown

---

## SH001 — Abertura: a pasta do arquivo se abre

**Shot ID:** `TSUKI_AMDK_E01_S01_SH001_MASTER`  
**Scene:** `S01`  
**Timecode:** `00:00–00:08`  
**Shot type:** `INSERT / TOP-DOWN MACRO`  
**Camera state:** `SLOW_PULL / ZOOM OUT`  
**Primary refs:** `assets/references/props/TSUKI_AMDK_PROP_CASE_FOLDER.jpeg`, `assets/references/props/TSUKI_AMDK_PROP_CASE_FOLDER_OPEN.jpeg`

### Dramatic objective
Abrir o episódio como documento vivo, não como fábula pet.

### Approved production prompt
```text
Top-down macro insert on a closed heavy kraft dossier folder resting on a dark aged wooden table. Tight framing on the typed label: CASO Nº 001 — O Biscoito Que Não Estava Lá. Weathered cardboard fibers, oxidized metal grommets, warm tungsten side light from the left, deep restrained shadows, authentic 16mm film grain, tactile analog texture. The cover opens smoothly on its own while the camera performs a slow motivated zoom out, revealing the full open dossier with case papers inside. No human hands. No CGI sheen. Serious archival true-crime mood.
```

### Audio
- Cardboard creak
- Paper rustle
- Single restrained minor piano chord
- No VO at start

### Editorial note
Começar muito fechado no rótulo. O movimento de recuo deve revelar contexto, não espetáculo.

### Approval gate
- [ ] etiqueta legível o suficiente sem parecer design gráfico digital
- [ ] kraft, metal e madeira com textura física
- [ ] sem mão humana
- [ ] sem movimento mágico exagerado
- [ ] 16mm orgânico, não “vintage filter”

---

## SH002 — Entrada de Tsuki na cozinha

**Shot ID:** `TSUKI_AMDK_E01_S01_SH002_MASTER`  
**Scene:** `S01`  
**Timecode:** `00:08–00:20`  
**Shot type:** `WS LOW TRACK`  
**Camera state:** `OBSERVATIONAL_TRACK`  
**Cardinal reference:** `SOUTH → WEST line`  
**Primary refs:** `assets/references/characters/TSUKI_AMDK_CHAR_TSUKI_MASTER_V001.jpeg`, `assets/references/locations/TSUKI_AMDK_KITCHEN_Sul.png`

### Dramatic objective
Apresentar Tsuki em modo de procedimento, entrando em quadro como quem inicia uma rotina de patrulha séria.

### Approved production prompt
```text
Low-angle wide shot at approximately 25cm above the pine floorboards, looking from the southern doorway into the kitchen. Tsuki, matching the exact master reference, enters from the left with a measured investigative walk, body low but composed, ears attentive, eyes focused toward the west evidence line. Soft natural daylight motivated by the north window mixes with restrained domestic ambient fill. Authentic 16mm motion-picture look, organic grain, soft exposure rolloff, lived-in kitchen textures, no cuteness, no anthropomorphic acting, no people.
```

### Audio
- Soft claw clicks on wood
- Distant refrigerator hum
- Very low room tone

### Narration
**VO_TSUKI_01 — parte A**  
"Eram 14h31 quando o objeto foi catalogado."

### Editorial note
A câmera acompanha pouco. Se não houver motivação forte, quase estática.

### Approval gate
- [ ] identidade de Tsuki estável
- [ ] altura de câmera baixa e coerente
- [ ] caminhada realista de cão jovem
- [ ] cozinha doméstica, não set estilizado
- [ ] sem energia cômica

---

## SH003 — Constatação da tigela vazia

**Shot ID:** `TSUKI_AMDK_E01_S01_SH003_MASTER`  
**Scene:** `S01`  
**Timecode:** `00:20–00:34`  
**Shot type:** `MCU LOW`  
**Camera state:** `STATIC_OBSERVATIONAL`  
**Cardinal reference:** `WEST`  
**Primary refs:** `assets/references/characters/TSUKI_AMDK_CHAR_TSUKI_MASTER_V001.jpeg`, `assets/references/locations/TSUKI_AMDK_KITCHEN_Oeste.png`, `assets/references/props/TSUKI_AMDK_PROP_BISCUIT_BOWL.jpeg`

### Dramatic objective
Registrar o exato instante em que Tsuki entende que algo deveria estar ali e não está.

### Approved production prompt
```text
Medium close-up at approximately 20cm from the floor on the west work-counter line. Tsuki has stopped precisely in front of the empty cream ceramic bowl on the woven jute mat. Her snout lowers with forensic focus toward the rim and the floor perimeter. Preserve exact schnauzer identity: dark gray wiry coat, cream beard, caramel mouth stain, silver-gray brows, dark brown eyes, natural tail. Late-afternoon side light from the north window grazes the ceramic and the beard. Authentic 16mm analog character, intimate documentary realism, no sentimentality, no humanized expression.
```

### Audio
- Soft sniffing
- Quiet breathing
- Refrigerator hum slightly clearer

### Narration
**VO_TSUKI_01 — parte B**  
"Um biscoito canino, formato osso, consistência sólida. Às 14h37, em ronda de rotina, o objeto não existia mais."

### Editorial note
Deixe o plano respirar. O suspense vem da precisão do foco, não da pressa.

### Approval gate
- [ ] tigela vazia inequívoca
- [ ] Tsuki séria, não fofa
- [ ] luz lateral coerente
- [ ] fundo oeste consistente
- [ ] composição íntima, não retrato comercial pet

---

## SH004 — O perímetro forense

**Shot ID:** `TSUKI_AMDK_E01_S01_SH004_MASTER`  
**Scene:** `S01`  
**Timecode:** `00:34–00:42`  
**Shot type:** `MACRO INSERT`  
**Camera state:** `LOCKED_OFF`  
**Cardinal reference:** `WEST`  
**Primary refs:** `assets/references/locations/TSUKI_AMDK_KITCHEN_Oeste.png`, `assets/references/props/TSUKI_AMDK_PROP_BISCUIT_BOWL_MACRO.jpeg`

### Dramatic objective
Confirmar a tese central do caso: não há qualquer evidência material no perímetro.

### Approved production prompt
```text
Extreme ground-level macro insert at approximately 10cm height, focused on the lower glazed edge of the empty cream ceramic bowl, the braided jute mat, and the surrounding pine floorboards on the west evidence line. The floor surface must be meticulously clean: absolute zero crumbs, zero saliva, zero wet marks, zero disturbance. Raking low-angle daylight reveals fine wood grain and microtexture. Shot on authentic 16mm film stock with crisp analog focus, tactile realism, restrained procedural mood. No extra debris, no stylized forensic graphics, no people.
```

### Audio
- Near-silence
- Low room hum
- Maybe a single breath off-screen from Tsuki

### Narration
**VO_TSUKI_02**  
"O perímetro não apresenta perturbação mecânica. Tigela alinhada a quarenta centímetros do rodapé. Ausência total de migalhas ou resíduos biológicos. Em seis minutos, um corpo sólido não se dissolve espontaneamente no ar. A menos que tenha havido intervenção de um agente."

### Editorial note
Esse plano precisa ser cristalino. Se aparecer qualquer sujeira inventada, reprovar.

### Approval gate
- [ ] zero migalhas de verdade
- [ ] textura do chão legível
- [ ] escala macro correta
- [ ] tigela/juta coerentes com prop master
- [ ] sem ruído visual artificial

---

## SH005 — Interrogatório silencioso

**Shot ID:** `TSUKI_AMDK_E01_S02_SH005_MASTER`  
**Scene:** `S02`  
**Timecode:** `00:42–01:00`  
**Shot type:** `VERTICAL TWO-SHOT`  
**Camera state:** `SLOW_PUSH_IN`  
**Cardinal reference:** `NORTH`  
**Primary refs:** `assets/references/characters/TSUKI_AMDK_CHAR_TSUKI_MASTER_V001.jpeg`, `assets/references/characters/TSUKI_AMDK_CHAR_SIMBA_MASTER_V001.jpg`, `assets/references/locations/TSUKI_AMDK_KITCHEN_Norte.png`

### Dramatic objective
Estabelecer a assimetria intelectual do episódio: Tsuki pergunta sem linguagem, Simba responde com imobilidade.

### Approved production prompt
```text
Low-angle medium two-shot inside the kitchen looking toward the north window. Tsuki stands on the wooden floor in the lower frame, looking up at a 45-degree angle with unwavering investigative focus. Simba is perched above on the windowsill or counter line, looking down calmly with ice-blue eyes. The vertical distance is critical; the mood is procedural, serious, and silent. Strong but motivated late-afternoon daylight from the north window shapes both animals. Camera performs only a slow restrained push-in. Authentic 16mm film grain, tactile domestic space, no anthropomorphic posing, no people.
```

### Audio
- Score drops nearly out
- Fridge hum
- Very distant outdoor air tone
- Sustained silence is part of the scene

### Narration
**VO_TSUKI_03 — parte A**  
"Simba. Suspeito primário por proximidade geográfica e acesso irrestrito ao perímetro."

### Silence block
**SILENCE_HOLD_01** = 4s to 5s of real quiet tension.

### Editorial note
O plano depende de duração. Não cortar cedo demais.

### Approval gate
- [ ] diferença de altura forte e clara
- [ ] Tsuki abaixo / Simba acima sem ambiguidade
- [ ] north window perceptível como fonte real de luz
- [ ] zero pose humana
- [ ] tensão nasce da quietude, não de caricatura

---

## SH006 — O slow blink de Simba

**Shot ID:** `TSUKI_AMDK_E01_S02_SH006_MASTER`  
**Scene:** `S02`  
**Timecode:** `01:00–01:10`  
**Shot type:** `CU SIMBA`  
**Camera state:** `LOCKED_OFF`  
**Cardinal reference:** `NORTH`  
**Primary refs:** `assets/references/characters/TSUKI_AMDK_CHAR_SIMBA_MASTER_V001.jpg`, `assets/references/locations/TSUKI_AMDK_KITCHEN_Norte.png`

### Dramatic objective
Executar o beat central sem overacting: Simba pisca uma vez, devagar, e isso basta.

### Approved production prompt
```text
Close-up portrait of Simba at windowsill height, looking slightly downward toward Tsuki below frame. Preserve exact Siamese seal point identity: cream body, dark seal mask, large triangular ears, ice-blue almond eyes. He remains perfectly still, then performs one slow deliberate blink. Soft north window light reflects in the eyes and along the short fur texture. The background stays domestic and softly resolved. Authentic 16mm portrait texture, intimate observational cinema, restrained and serious, no fantasy-cat stylization, no comedy.
```

### Audio
- Almost no score
- Fine room tone
- Light outdoor breeze

### Narration
**VO_TSUKI_03 — parte B**  
"Quarenta e cinco segundos de contato visual sustentado. Às 14h42, o sujeito executa um fechamento palpebral prolongado. Hipótese inicial: código de comunicação não verbal felina. Hipótese secundária: admissão velada de culpa."

**VO_SIMBA_01**  
"Ela acha que eu comi o biscoito. Gatos não comem farinha prensada com sabor artificial de carne. A garota de trança veio às 14h33, pegou o biscoito e guardou no bolso do casaco antes de ir para a escola. Eu estava aqui. Eu vi."

### Silence block
**SILENCE_HOLD_02** = 1s a 2s após o blink antes do corte.

### Editorial note
O blink não pode parecer sonolento nem fofo. É controle, não preguiça.

### Approval gate
- [ ] olhos de Simba corretos
- [ ] blink lento único
- [ ] nada de expressão humana
- [ ] luz da janela natural e motivada
- [ ] close intimista sem glamour comercial

---

## SH007 — Tsuki cataloga a pista

**Shot ID:** `TSUKI_AMDK_E01_S02_SH007_MASTER`  
**Scene:** `S02`  
**Timecode:** `01:10–01:20`  
**Shot type:** `CU TSUKI`  
**Camera state:** `LOCKED_OFF`  
**Cardinal reference:** `NORTH`  
**Primary refs:** `assets/references/characters/TSUKI_AMDK_CHAR_TSUKI_MASTER_V001.jpeg`, `assets/references/locations/TSUKI_AMDK_KITCHEN_Norte.png`

### Dramatic objective
Mostrar o nascimento da hipótese errada de Tsuki com o menor gesto possível.

### Approved production prompt
```text
Tight close-up of Tsuki from about 20cm above floor level, looking upward toward Simba. Preserve exact miniature schnauzer identity and fur structure. Her head begins level and then tilts only 2 millimeters to the side in a micro-gesture of analytical deduction. Dark brown eyes remain sharp, serious, and fully non-ironic. The north kitchen background stays soft and indistinct. Authentic 16mm grain, tactile fur detail, restrained domestic light, documentary realism, no comedic dog expression.
```

### Audio
- Single returning piano note
- Faint room tone

### Narration
**VO_SIMBA_02**  
"Poderia descer e apontar para a porta por onde ela saiu. Não vou. Tsuki precisa aprender que nem todo mistério deixa rastro farejável. Ela está olhando para mim com aquela seriedade que... aquela palavra que eu ainda não encontrei."

### Editorial note
O tilt de 2mm é microscópico. Se parecer truque fofo, está errado.

### Approval gate
- [ ] Tsuki idêntica ao master
- [ ] tilt mínimo, não caricatural
- [ ] olhos e sobrancelhas legíveis
- [ ] sem humor visual involuntário
- [ ] coerência de contra-plano com SH006

---

## SH008 — Vigília ao entardecer

**Shot ID:** `TSUKI_AMDK_E01_S03_SH008_MASTER`  
**Scene:** `S03`  
**Timecode:** `01:20–01:44`  
**Shot type:** `WS SUNSET`  
**Camera state:** `STATIC_OBSERVATIONAL`  
**Cardinal reference:** `NORTH / WEST evidence axis`  
**Primary refs:** `assets/references/characters/TSUKI_AMDK_CHAR_TSUKI_MASTER_V001.jpeg`, `assets/references/characters/TSUKI_AMDK_CHAR_SIMBA_MASTER_V001.jpg`, `assets/references/locations/TSUKI_AMDK_KITCHEN_Norte.png`, `assets/references/props/TSUKI_AMDK_PROP_BISCUIT_BOWL.jpeg`

### Dramatic objective
Fechar a investigação sem solução fácil: Tsuki aceita apenas a vigília.

### Approved production prompt
```text
Wide kitchen shot at early evening golden hour, camera low and observational, looking toward the north window while preserving the west evidence axis in the foreground. Tsuki lies on the floor in a vigilant sphinx posture, chin resting about 10cm from the empty cream ceramic bowl. Her body is calm but committed. Simba remains farther back near the window, seated and quietly observing. The late-afternoon light has weakened into amber dusk, casting long restrained shadows across the worn pine floorboards. Authentic 16mm film look, domestic melancholy, physical textures, no melodrama, no sentimentality, no people.
```

### Audio
- Quiet room tone
- Very low piano
- Tsuki breathing
- Maybe light air at the window

### Narration
**VO_TSUKI_04**  
"O suspeito permanece não-cooperativo. Motivação e método de extração do objeto continuam sob análise. Estabelecendo vigilância contínua do local do evento."

### Editorial note
Este é o plano com maior duração. Ele precisa sustentar o peso do caso aberto.

### Approval gate
- [ ] luz de 18h04 convincente
- [ ] tigela permanece vazia e intocada
- [ ] Tsuki em posição de vigília, não de tristeza melodramática
- [ ] Simba discreto ao fundo
- [ ] sensação de casa vivida e silenciosa

---

## SH009 — Fechamento canônico

**Shot ID:** `TSUKI_AMDK_E01_S03_SH009_MASTER`  
**Scene:** `S03`  
**Timecode:** `01:44–02:00`  
**Shot type:** `INSERT / TOP-DOWN MACRO`  
**Camera state:** `SLOW_PUSH / ZOOM IN`  
**Primary refs:** `assets/references/props/TSUKI_AMDK_PROP_CASE_FOLDER_OPEN.jpeg`, `assets/references/props/TSUKI_AMDK_PROP_CASE_FOLDER_W_RUBBER.jpeg`

### Dramatic objective
Encerrar formalmente o episódio sem encerrar o caso.

### Approved production prompt
```text
Top-down dossier closing shot starting from the opened case folder on the same dark aged wooden table. The cover folds shut smoothly while the camera performs a slow motivated push-in toward the label and the final burgundy stamp. End on a tight macro of the kraft cardboard texture and the stamped classification CASO Nº 001 | CLASSIFICADO: ABERTO. Warm tungsten side light, deep restrained shadows, authentic 16mm grain, tactile analog archive mood. No human hands, no glossy graphics, no exaggerated magical motion.
```

### Audio
- Folder closing thump, soft and firm
- Final suspended minor piano chord
- Optional end air tone, then cut to black

### Visual text / On-screen text
`Nota de rodapé:`  
"A tigela foi inspecionada por mais 3 horas e 27 minutos. Nenhuma nova evidência material foi detectada."

### Silence block
**SILENCE_HOLD_03** = 1s after final chord before hard end.

### Editorial note
O carimbo deve ser imperfeito e físico. Nunca limpo demais.

### Approval gate
- [ ] dossiê consistente com SH001
- [ ] carimbo bordô legível e orgânico
- [ ] textura do kraft muito presente
- [ ] sem aparência motion-graphic
- [ ] final realmente irresoluto

---

## 6. Voice recording sheet / Folha de gravação de voz

### Tsuki

**Clip ID:** `TSUKI_AMDK_E01_VO_TSUKI_01_PT`  
```text
Eram 14h31 quando o objeto foi catalogado. Um biscoito canino, formato osso, consistência sólida. Às 14h37, em ronda de rotina, o objeto não existia mais.
```

**Clip ID:** `TSUKI_AMDK_E01_VO_TSUKI_02_PT`  
```text
O perímetro não apresenta perturbação mecânica. Tigela alinhada a quarenta centímetros do rodapé. Ausência total de migalhas ou resíduos biológicos. Em seis minutos, um corpo sólido não se dissolve espontaneamente no ar. A menos que tenha havido intervenção de um agente.
```

**Clip ID:** `TSUKI_AMDK_E01_VO_TSUKI_03_PT`  
```text
Simba. Suspeito primário por proximidade geográfica e acesso irrestrito ao perímetro. Quarenta e cinco segundos de contato visual sustentado. Às 14h42, o sujeito executa um fechamento palpebral prolongado. Hipótese inicial: código de comunicação não verbal felina. Hipótese secundária: admissão velada de culpa.
```

**Clip ID:** `TSUKI_AMDK_E01_VO_TSUKI_04_PT`  
```text
O suspeito permanece não-cooperativo. Motivação e método de extração do objeto continuam sob análise. Estabelecendo vigilância contínua do local do evento.
```

### Simba

**Clip ID:** `TSUKI_AMDK_E01_VO_SIMBA_01_PT`  
```text
Ela acha que eu comi o biscoito. Gatos não comem farinha prensada com sabor artificial de carne. A garota de trança veio às 14h33, pegou o biscoito e guardou no bolso do casaco antes de ir para a escola. Eu estava aqui. Eu vi.
```

**Clip ID:** `TSUKI_AMDK_E01_VO_SIMBA_02_PT`  
```text
Poderia descer e apontar para a porta por onde ela saiu. Não vou. Tsuki precisa aprender que nem todo mistério deixa rastro farejável. Ela está olhando para mim com aquela seriedade que... aquela palavra que eu ainda não encontrei.
```

### Performance notes
- **Tsuki:** seca, metodológica, precisa, sem ironia, sem ternura performada.
- **Simba:** íntimo, maduro, observador, baixo consumo emocional, sem melodrama.

---

## 7. Deliverables list / Lista de entregáveis

### Image stills
- SH001 start/end
- SH002 end or full still
- SH003 end
- SH004 macro
- SH005 start/end
- SH006 end blink
- SH007 end tilt
- SH008 start/end
- SH009 end stamp

### Video shots
- `TSUKI_AMDK_E01_S01_SH001_TAKE01_V001.mp4`
- `TSUKI_AMDK_E01_S01_SH002_TAKE01_V001.mp4`
- `TSUKI_AMDK_E01_S01_SH003_TAKE01_V001.mp4`
- `TSUKI_AMDK_E01_S01_SH004_TAKE01_V001.mp4`
- `TSUKI_AMDK_E01_S02_SH005_TAKE01_V001.mp4`
- `TSUKI_AMDK_E01_S02_SH006_TAKE01_V001.mp4`
- `TSUKI_AMDK_E01_S02_SH007_TAKE01_V001.mp4`
- `TSUKI_AMDK_E01_S03_SH008_TAKE01_V001.mp4`
- `TSUKI_AMDK_E01_S03_SH009_TAKE01_V001.mp4`

### Audio
- `TSUKI_AMDK_E01_VO_TSUKI_01_PT.wav`
- `TSUKI_AMDK_E01_VO_TSUKI_02_PT.wav`
- `TSUKI_AMDK_E01_VO_TSUKI_03_PT.wav`
- `TSUKI_AMDK_E01_VO_TSUKI_04_PT.wav`
- `TSUKI_AMDK_E01_VO_SIMBA_01_PT.wav`
- `TSUKI_AMDK_E01_VO_SIMBA_02_PT.wav`
- room tone stem
- piano stem
- foley stem

### Final masters
- `TSUKI_AMDK_E01_MASTER_LOCKED_V001.mov`
- `TSUKI_AMDK_E01_MASTER_REVIEW_V001.mp4`
- `TSUKI_AMDK_E01_MASTER_SUBS_PT_V001.mp4`

---

## 8. One-line operational directive

**Produzir em ordem: lock de keyframes principais → cobertura total de stills → geração de vídeo por shot → vozes → montagem de 120s → QC por canon antes do master final.**
