# TSUKI_AMDK — EP01 · Asset Tracker
### Production tracker / controle de ativos

Status base: `READY / TODO template`
Episode build: `EP01 Build A`

---

## 1. Legenda de status / Status legend

- `READY` = referência já existente e utilizável
- `TODO` = ainda não produzido
- `WIP` = em produção
- `REVIEW` = aguardando avaliação
- `APPROVED` = aprovado para continuidade
- `REJECTED` = reprovado, não usar como canon
- `LOCKED` = aprovado e promovido a master operacional

---

## 2. Gates principais / Main gates

### Gate A — Reference integrity
- identidade dos personagens confere
- cardinal da cozinha confere
- prop confere com canon

### Gate B — Still approval
- frame sustenta 16mm orgânico
- sem antropomorfização
- sem drift de anatomia

### Gate C — Motion approval
- ação mínima e motivada
- câmera não vira espetáculo
- continuidade entre start e end frame preservada

### Gate D — Audio approval
- performance vocal correta
- silêncio mantido onde necessário
- música discreta

### Gate E — Final master
- 120s aproximados
- caso continua aberto
- nenhum plano quebra canon

---

## 3. Critical path / Caminho crítico

| Ordem | Grupo | Entregável | Status inicial |
|---|---|---|---|
| 1 | References | personagens, cozinha, props | READY |
| 2 | Keyframes | SH001, SH003, SH005, SH008, SH009 | LOCKED / MOSTLY LOCKED |
| 3 | Coverage stills | demais start/end frames | LOCKED WITH 1 HOLD |
| 4 | Motion | 9 takes de vídeo | READY FOR PREP |
| 5 | Audio | 6 clips de voz + stems | REVIEW |
| 6 | Edit | assembly cut | TODO |
| 7 | Master | review export + locked master | TODO |

---

## 4. Reference assets / Ativos de referência

| Asset ID | Tipo | Arquivo base | Status | Gate |
|---|---|---|---|---|
| REF_CHAR_TSUKI | CHARACTER_REFERENCE | `assets/references/characters/TSUKI_AMDK_CHAR_TSUKI_MASTER_V001.jpeg` | READY | A |
| REF_CHAR_SIMBA | CHARACTER_REFERENCE | `assets/references/characters/TSUKI_AMDK_CHAR_SIMBA_MASTER_V001.jpg` | READY | A |
| REF_LOC_KITCHEN_NORTH | LOCATION_REFERENCE | `assets/references/locations/TSUKI_AMDK_KITCHEN_Norte.png` | READY | A |
| REF_LOC_KITCHEN_SOUTH | LOCATION_REFERENCE | `assets/references/locations/TSUKI_AMDK_KITCHEN_Sul.png` | READY | A |
| REF_LOC_KITCHEN_WEST | LOCATION_REFERENCE | `assets/references/locations/TSUKI_AMDK_KITCHEN_Oeste.png` | READY | A |
| REF_PROP_BOWL | OBJECT_REFERENCE | `assets/references/props/TSUKI_AMDK_PROP_BISCUIT_BOWL.jpeg` | READY | A |
| REF_PROP_BOWL_MACRO | OBJECT_REFERENCE | `assets/references/props/TSUKI_AMDK_PROP_BISCUIT_BOWL_MACRO.jpeg` | READY | A |
| REF_PROP_BISCUIT | OBJECT_REFERENCE | `assets/references/props/TSUKI_AMDK_PROP_DOG_BISCUIT_MASTER.jpeg` | READY | A |
| REF_PROP_FOLDER_CLOSED | OBJECT_REFERENCE | `assets/references/props/TSUKI_AMDK_PROP_CASE_FOLDER.jpeg` | READY | A |
| REF_PROP_FOLDER_OPEN | OBJECT_REFERENCE | `assets/references/props/TSUKI_AMDK_PROP_CASE_FOLDER_OPEN.jpeg` | READY | A |
| REF_PROP_FOLDER_STAMPED | OBJECT_REFERENCE | `assets/references/props/TSUKI_AMDK_PROP_CASE_FOLDER_W_RUBBER.jpeg` | READY | A |

---

## 5. Priority keyframes / Keyframes prioritários

| Ordem | Asset ID | Shot | Entregável | Status | Gate | Observação |
|---|---|---|---|---|---|---|
| 1 | KF_SH001_START | SH001 | dossiê fechado / macro label | LOCKED | B | V001 travado |
| 2 | KF_SH001_END | SH001 | dossiê aberto | LOCKED | B | V001 travado |
| 3 | KF_SH003_END | SH003 | Tsuki + tigela vazia | LOCKED | B | V002 travado |
| 4 | KF_SH005_START | SH005 | two-shot Tsuki vs Simba | LOCKED | B | V002 travado |
| 5 | KF_SH008_START | SH008 | vigília ao entardecer | LOCKED | B | V001 travado |
| 6 | KF_SH009_END | SH009 | carimbo final | LOCKED | B | V001 travado |

---

## 6. Full shot asset matrix / Matriz completa por plano

| Shot | Still assets | Video asset | Audio assets | Status inicial |
|---|---|---|---|---|
| SH001 | START + END | TAKE01 | SFX_FOLDER + MUS_CUE_01 | READY FOR MOTION |
| SH002 | END principal | TAKE01 | VO_TSUKI_01A + ROOM_01 | READY FOR MOTION |
| SH003 | START + END | TAKE01 | VO_TSUKI_01B + FOLEY_SNIFF | READY WITH START HOLD |
| SH004 | START + END | TAKE01 | VO_TSUKI_02 + ROOM_QUIET | READY FOR MOTION |
| SH005 | START + END | TAKE01 | VO_TSUKI_03A + SILENCE_HOLD_01 | READY FOR MOTION |
| SH006 | START + END | TAKE01 | VO_TSUKI_03B + VO_SIMBA_01 | READY FOR MOTION |
| SH007 | START + END | TAKE01 | VO_SIMBA_02 + MUS_CUE_02 | READY FOR MOTION |
| SH008 | START + END | TAKE01 | VO_TSUKI_04 + ROOM_DUSK | READY FOR MOTION |
| SH009 | START + END | TAKE01 | SFX_FOLDER_CLOSE + MUS_CUE_03 | READY FOR MOTION |

---

## 7. Audio package / Pacote de áudio

| Asset ID | Tipo | Nome sugerido | Status | Gate |
|---|---|---|---|---|
| VO_TSUKI_01 | VO | `TSUKI_AMDK_E01_VO_TSUKI_01_PT.wav` | REVIEW | D |
| VO_TSUKI_02 | VO | `TSUKI_AMDK_E01_VO_TSUKI_02_PT.wav` | REVIEW | D |
| VO_TSUKI_03 | VO | `TSUKI_AMDK_E01_VO_TSUKI_03_PT.wav` | REVIEW | D |
| VO_TSUKI_04 | VO | `TSUKI_AMDK_E01_VO_TSUKI_04_PT.wav` | REVIEW | D |
| VO_SIMBA_01 | VO | `TSUKI_AMDK_E01_VO_SIMBA_01_PT.wav` | REVIEW | D |
| VO_SIMBA_02 | VO | `TSUKI_AMDK_E01_VO_SIMBA_02_PT.wav` | REVIEW | D |
| ROOM_KITCHEN_BASE | ROOM TONE | `TSUKI_AMDK_E01_ROOM_BASE_V001.wav` | TODO | D |
| FOLEY_PAWS_SNIFF | FOLEY | `TSUKI_AMDK_E01_FOLEY_PAWS_SNIFF_V001.wav` | TODO | D |
| MUS_PIANO_MINOR | MUSIC STEM | `TSUKI_AMDK_E01_MUS_PIANO_MINOR_V001.wav` | TODO | D |

---

## 8. Final delivery package / Pacote final

| Asset ID | Tipo | Nome sugerido | Status | Gate |
|---|---|---|---|---|
| EDIT_ASSEMBLY_01 | EDIT TIMELINE | `TSUKI_AMDK_E01_ASSEMBLY_V001` | TODO | E |
| MASTER_REVIEW_01 | REVIEW EXPORT | `TSUKI_AMDK_E01_MASTER_REVIEW_V001.mp4` | TODO | E |
| MASTER_LOCKED_01 | FINAL MASTER | `TSUKI_AMDK_E01_MASTER_LOCKED_V001.mov` | TODO | E |
| MASTER_SUBS_PT_01 | FINAL SUBBED | `TSUKI_AMDK_E01_MASTER_SUBS_PT_V001.mp4` | TODO | E |

---

## 9. Uso recomendado / Recommended use

- Atualize o CSV irmão (`docs/episodes/ep01/08_ep01_asset_tracker.csv`) durante a produção real.
- Use este `.md` como visão executiva.
- Consulte `docs/episodes/ep01/19_ep01_locked_stills_manifest.md` para o set visual travado.
- Consulte `docs/episodes/ep01/20_ep01_motion_preflight.md` e `docs/episodes/ep01/22_ep01_motion_batch_01_prompts.md` / `docs/episodes/ep01/23_ep01_motion_batch_02_prompts.md` / `docs/episodes/ep01/25_ep01_motion_batch_03_prompts.md` para o motion prep.
- Consulte `docs/episodes/ep01/24_ep01_assembly_blueprint.md` e `docs/episodes/ep01/26_ep01_timeline_edit_sheet.md` para o pre-assembly.
- Promova qualquer item para `LOCKED` somente depois de passar pelo gate indicado.
