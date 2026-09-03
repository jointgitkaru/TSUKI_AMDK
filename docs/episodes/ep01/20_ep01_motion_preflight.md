# TSUKI_AMDK — EP01 · Motion Preflight
### Preparação de motion pass a partir dos stills travados

Status: `READY FOR MOTION PREP`
Date: `2026-09-03`

---

## 1. Objetivo

Transformar o pacote de stills travados em uma folha operacional de motion.

Este documento define:
- par de frames por shot;
- duração alvo;
- movimento de câmera permitido;
- ação mínima dos personagens/objetos;
- risco principal por plano.

---

## 2. Ordem recomendada de motion pass

### Batch 01 — menor risco / melhor retorno
1. SH001
2. SH004
3. SH006
4. SH009

### Batch 02 — tensão controlada
5. SH005
6. SH007

### Batch 03 — espaço e performance
7. SH008
8. SH002
9. SH003

---

## 3. Motion sheet by shot

## SH001
- **Frames:** `SH001_START_V001` → `SH001_END_V001`
- **Duration:** 8s
- **Camera:** slow zoom out / pull back
- **Action:** pasta abre sozinha com física contida
- **Risk:** parecer mágica demais ou virar motion graphic
- **Pass condition:** textura do papel e peso da tampa precisam parecer reais

## SH002
- **Frame basis:** `SH002_END_V002`
- **Duration:** 12s
- **Camera:** low observational track
- **Action:** Tsuki entra do sul e segura ao final
- **Risk:** Tsuki parecer grande demais ou caminhar com energia cômica
- **Pass condition:** entrada metódica, escala pequena e coerente com a cozinha

## SH003
- **Frames:** `SH003_START_V001` → `SH003_END_V002`
- **Duration:** 14s
- **Camera:** almost static / subtle breathing only
- **Action:** Tsuki aproxima e abaixa o focinho sobre a tigela
- **Risk:** mismatch fino entre START e END; bowl parecer grande demais
- **Pass condition:** tensão por precisão, não por acting

## SH004
- **Frames:** `SH004_START_V001` → `SH004_END_V001`
- **Duration:** 8s
- **Camera:** locked macro
- **Action:** quase nenhuma; micro refocus permitido
- **Risk:** modelo inventar sujeira, migalhas ou movimento excessivo
- **Pass condition:** zero migalhas inequívoco do início ao fim

## SH005
- **Frames:** `SH005_START_V002` → `SH005_END_V001`
- **Duration:** 18s
- **Camera:** slow push-in
- **Action:** Tsuki abaixo olha para Simba acima; ambos quase imóveis
- **Risk:** quebra de escala, perda da assimetria vertical, poses humanas
- **Pass condition:** o silêncio deve ser sustentado pela composição

## SH006
- **Frames:** `SH006_START_V001` → `SH006_END_V001`
- **Duration:** 10s
- **Camera:** locked close-up
- **Action:** um slow blink único
- **Risk:** blink sonolento, caricato ou “fofo”
- **Pass condition:** serenidade controlada, micro-ação precisa

## SH007
- **Frames:** `SH007_START_V002` → `SH007_END_V002`
- **Duration:** 10s
- **Camera:** locked close-up
- **Action:** micro-tilt dedutivo de 2mm
- **Risk:** movimento pequeno demais para o gerador ou corte de continuidade
- **Pass condition:** parece o mesmo shot com mínima alteração analítica

## SH008
- **Frames:** `SH008_START_V001` → `SH008_END_V001`
- **Duration:** 24s
- **Camera:** static observational
- **Action:** quase nenhuma; respiração e mudança de luz são suficientes
- **Risk:** melodrama visual, pôr do sol publicitário, drift de proporção
- **Pass condition:** vigília imóvel, peso do tempo e da espera

## SH009
- **Frames:** `SH009_START_V001` → `SH009_END_V001`
- **Duration:** 16s
- **Camera:** slow push-in / zoom in
- **Action:** pasta fecha até o carimbo final
- **Risk:** carimbo perder legibilidade ou parecer design digital
- **Pass condition:** final físico, tátil e irresoluto

---

## 4. Motion-ready prompt principles

Usar sempre estes princípios na passagem para vídeo:
- movimento mínimo e motivado;
- preservação estrita de identidade;
- sem teatralização de câmera;
- sem adição de elementos novos;
- luz sempre com origem física compreensível;
- tensão por duração e precisão, não por exagero.

---

## 5. Gating before render

Antes de qualquer take de vídeo:
- [ ] conferir se o par start/end é o correto
- [ ] conferir escala relativa contra a referência dimensional
- [ ] conferir se o shot continua no cardinal correto
- [ ] conferir se nenhum frame concorrente mais forte ficou de fora
- [ ] conferir se o tempo do shot justifica o tipo de movimento

---

## 6. Diretiva final

**Iniciar o motion pass pelo que exige menos interpretação e mais controle físico: dossiê, macro forense, blink e fechamento.**
