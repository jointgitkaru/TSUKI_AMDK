# TSUKI_AMDK — EP01 · Motion Batch 03 Prompts
### Space-and-performance completion batch

Status: `READY`
Scope: `SH008 / SH002 / SH003`

---

## Purpose

Este lote completa o pacote operacional dos shots restantes.

Ele é mais delicado porque combina:
- escala dos personagens no espaço;
- tempo de observação mais longo;
- blocking simples, mas fácil de desproporcionar;
- risco de drifting entre stills com funções diferentes.

A prioridade aqui é manter:
- escala correta;
- geografia compreensível;
- ação mínima;
- coerência de tom com os batches 01 e 02.

---

## SH008 — Vigília ao entardecer

**Start frame:** `outputs/renders/TSUKI_AMDK_E01_S03_SH008_START_V001.png`  
**End frame:** `outputs/renders/TSUKI_AMDK_E01_S03_SH008_END_V001.png`  
**Target duration:** `24s`

```text
Use the locked start and end frames as strict continuity anchors. Create a low observational wide shot of the kitchen at 18h04 moving slightly deeper into dusk. Tsuki remains lying in a vigilant sphinx posture with her chin near the empty bowl. Simba remains seated farther back near the window as a quiet witness presence. Motion must be minimal: subtle breathing, tiny ambient shifts, and a gentle progression of late-afternoon light toward slightly cooler dusk. Preserve the corrected relative scale of both animals against the cabinets, chair legs, bowl, and room depth. No melodrama, no sentimental pet look, no major repositioning, no extra actions, no scale drift. Preserve tactile 16mm realism and domestic stillness.
```

### Performance rule
- Tsuki does not relax into sleep
- Simba does not perform
- the room carries time, not the bodies

### Pass condition
- vigil feels sustained and credible
- dusk progression reads without becoming dramatic spectacle
- scale remains believable from start to end

### Main risk
The shot may become too scenic, too sentimental, or too painterly instead of procedural.

---

## SH002 — Entrada de Tsuki

**Frame basis:** `outputs/renders/TSUKI_AMDK_E01_S01_SH002_END_V002.png`  
**Target duration:** `12s`

```text
Use the locked SH002 end frame as the visual destination and preserve the dimensional reference logic. Create a low-angle wide entry shot from the southern doorway in which Tsuki enters with a measured, procedural walk and settles into alert stillness facing the west evidence line. Keep her clearly small and compact relative to the doorway, cabinets, floorboards, chair legs, and bowl. The camera may perform only a subtle observational track at dog-eye height. No rushing, no excitement, no tail exaggeration, no comedic energy, no added characters. Preserve lived-in domestic texture, motivated natural light, and tactile 16mm realism.
```

### Performance rule
- deliberate pace only
- no cute hesitation
- no obvious pet-performance energy

### Pass condition
- entrance reads as patrol, not play
- Tsuki scale remains miniaturized and plausible
- final hold aligns naturally with SH003

### Main risk
The generator may oversize Tsuki or give her an overly animated walk cycle.

---

## SH003 — Constatação da tigela vazia

**Start frame:** `outputs/renders/TSUKI_AMDK_E01_S01_SH003_START_V001.png`  
**End frame:** `outputs/renders/TSUKI_AMDK_E01_S01_SH003_END_V002.png`  
**Target duration:** `14s`

```text
Use the current start and locked end frames as continuity anchors, but prioritize the dimensional logic of the locked end frame. Create a restrained medium close-up on the west evidence line in which Tsuki completes her approach and lowers her snout into a precise forensic inspection of the empty bowl. Keep the bowl modest in scale relative to her muzzle, beard, front paws, and chest. The movement is slow, measured, and nearly static once she arrives. Preserve the side light from the north window, domestic kitchen wear, tactile bowl glaze, jute texture, and authentic 16mm realism. No extra crumbs, no exaggerated sniffing, no humanized expression, no scale drift.
```

### Performance rule
- focus, not emotion
- movement stops quickly into concentration
- the absence in the bowl is the real subject

### Pass condition
- the shot lands on forensic seriousness
- bowl scale remains credible
- the start-to-end transition does not feel like two unrelated images

### Main risk
The current start frame is still a light hold item, so motion generation may expose continuity mismatch more than a still review does.

---

## Batch 03 render guidance

### Recommended order
1. SH008
2. SH002
3. SH003

### Why
- SH008 has the longest duration but the least literal movement
- SH002 establishes gait and scale behavior
- SH003 is the most continuity-sensitive and should come last after the motion language is stable

### Approval logic
Only pass the batch if:
- SH008 sustains procedural stillness
- SH002 keeps Tsuki small and credible in the kitchen
- SH003 does not expose a distracting start/end mismatch

---

## Optional caution branch

If SH003 fails in motion due to continuity mismatch, regenerate a dedicated `SH003_START_V002` before attempting another video pass.

---

## Final directive

**Batch 03 should complete the operational motion package without expanding the visual language beyond what the stills already proved.**
