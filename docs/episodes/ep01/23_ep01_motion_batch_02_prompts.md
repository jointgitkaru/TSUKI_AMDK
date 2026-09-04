# TSUKI_AMDK — EP01 · Motion Batch 02 Prompts
### Tension-control motion batch

Status: `READY`
Scope: `SH005 / SH007`

---

## Purpose

Este lote cobre o miolo dramático do episódio.
É mais sensível do que o Batch 01 porque depende de:
- relação espacial entre personagens;
- contenção absoluta de acting;
- leitura de silêncio e micro-gesto.

A meta aqui não é espetáculo.
A meta é **pressão dramática por imobilidade**.

---

## SH005 — Interrogatório silencioso

**Start frame:** `outputs/renders/TSUKI_AMDK_E01_S02_SH005_START_V002.png`  
**End frame:** `outputs/renders/TSUKI_AMDK_E01_S02_SH005_END_V001.png`  
**Target duration:** `18s`

```text
Use the locked start and end frames as strict continuity anchors. Create a low-angle north-window interrogation shot in which Tsuki remains below on the floor and Simba remains above on the windowsill, preserving the exact vertical asymmetry and the corrected relative scale. The camera performs only a slow, restrained push-in. Both animals remain almost perfectly still, sustaining eye contact across the vertical gap. No barking, no overt head turns, no human-like posing, no added props, no scale drift. Preserve the late-afternoon window light, lived-in kitchen textures, and tactile 16mm realism. The shot must feel serious, procedural, and tense through duration rather than action.
```

### Performance rule
- Tsuki: unwavering upward focus
- Simba: calm downward witness stillness
- both: almost no body motion

### Pass condition
- dog below / cat above reads instantly
- no scale drift across push-in
- silence feels active, not empty

### Main risk
The generator may try to animate too much or rebalance the frame in a way that weakens the interrogation geometry.

---

## SH007 — Tsuki cataloga a pista

**Start frame:** `outputs/renders/TSUKI_AMDK_E01_S02_SH007_START_V002.png`  
**End frame:** `outputs/renders/TSUKI_AMDK_E01_S02_SH007_END_V002.png`  
**Target duration:** `10s`

```text
Use the locked start and end frames as strict continuity anchors. Create a tight counter-shot close-up of Tsuki from low height, preserving the same three-quarter angle, the same upward eyeline toward Simba above frame, the same fur detail, the same domestic background blur, and the same dimensional proportions. The only meaningful motion is a precise micro analytical head tilt of about 2 millimeters, with a subtle sharpening of focus in the eyes. No front-facing portrait drift, no comedic curiosity, no exaggerated motion, no lens change, no lighting change. Preserve tactile 16mm realism and procedural seriousness.
```

### Performance rule
- no smile read
- no “cute dog reaction”
- deduction is physical but microscopic

### Pass condition
- looks like one continuous shot
- tilt is readable but minimal
- eyeline remains clearly upward

### Main risk
The generator may under-animate the tilt or accidentally produce a new portrait instead of a continuity pair.

---

## Batch 02 render guidance

### Recommended order
1. SH005
2. SH007

### Why
- SH005 establishes the pressure field
- SH007 resolves that pressure into Tsuki's mistaken hypothesis

### Approval logic
Only move forward if:
- SH005 preserves vertical asymmetry without scale drift
- SH007 preserves the V002 counter-shot logic
- neither shot becomes sentimental or pet-commercial

---

## Final directive

**If Batch 02 works, the emotional core of EP01 is visually solved.**
