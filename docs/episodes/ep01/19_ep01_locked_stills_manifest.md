# TSUKI_AMDK — EP01 · Locked Stills Manifest
### Seleção operacional travada para continuidade e motion prep

Status: `LOCKED STILL SET / BUILD A`
Date: `2026-09-03`

---

## 1. Objetivo

Este documento promove os stills mais estáveis do EP01 para o conjunto operacional travado.
A função dele é simples:
- definir qual versão usar por shot;
- evitar drift entre versões concorrentes;
- preparar a etapa de motion pass e montagem.

---

## 2. Locked selection by shot

| Shot | Frame | Versão travada | Caminho local | Status |
|---|---|---|---|---|
| SH001 | START | `V001` | `outputs/renders/TSUKI_AMDK_E01_S01_SH001_START_V001.png` | LOCKED |
| SH001 | END | `V001` | `outputs/renders/TSUKI_AMDK_E01_S01_SH001_END_V001.png` | LOCKED |
| SH002 | HOLD / END | `V002` | `outputs/renders/TSUKI_AMDK_E01_S01_SH002_END_V002.png` | LOCKED |
| SH003 | START | `V001` | `outputs/renders/TSUKI_AMDK_E01_S01_SH003_START_V001.png` | REVIEW HOLD |
| SH003 | END | `V002` | `outputs/renders/TSUKI_AMDK_E01_S01_SH003_END_V002.png` | LOCKED |
| SH004 | START | `V001` | `outputs/renders/TSUKI_AMDK_E01_S01_SH004_START_V001.png` | LOCKED |
| SH004 | END | `V001` | `outputs/renders/TSUKI_AMDK_E01_S01_SH004_END_V001.png` | LOCKED |
| SH005 | START | `V002` | `outputs/renders/TSUKI_AMDK_E01_S02_SH005_START_V002.png` | LOCKED |
| SH005 | END | `V001` | `outputs/renders/TSUKI_AMDK_E01_S02_SH005_END_V001.png` | LOCKED |
| SH006 | START | `V001` | `outputs/renders/TSUKI_AMDK_E01_S02_SH006_START_V001.png` | LOCKED |
| SH006 | END | `V001` | `outputs/renders/TSUKI_AMDK_E01_S02_SH006_END_V001.png` | LOCKED |
| SH007 | START | `V002` | `outputs/renders/TSUKI_AMDK_E01_S02_SH007_START_V002.png` | LOCKED |
| SH007 | END | `V002` | `outputs/renders/TSUKI_AMDK_E01_S02_SH007_END_V002.png` | LOCKED |
| SH008 | START | `V001` | `outputs/renders/TSUKI_AMDK_E01_S03_SH008_START_V001.png` | LOCKED |
| SH008 | END | `V001` | `outputs/renders/TSUKI_AMDK_E01_S03_SH008_END_V001.png` | LOCKED |
| SH009 | START | `V001` | `outputs/renders/TSUKI_AMDK_E01_S03_SH009_START_V001.png` | LOCKED |
| SH009 | END | `V001` | `outputs/renders/TSUKI_AMDK_E01_S03_SH009_END_V001.png` | LOCKED |

---

## 3. Curatorial notes

### Promoted with confidence
- SH001 start/end
- SH002 end V002
- SH003 end V002
- SH004 start/end
- SH005 start V002 + end V001
- SH006 start/end
- SH007 start/end V002
- SH008 start/end
- SH009 start/end

### Held for caution
- `SH003_START_V001` permanece como `REVIEW HOLD`.

Motivo:
- funciona como aproximação;
- ainda não recebeu uma correção dimensional dedicada como SH002/SH003_END/SH005/SH008;
- pode ser usado provisoriamente, mas vale reabrir se o motion exigir continuidade fina demais.

---

## 4. Preferred motion-ready pairs

| Shot | Par sugerido |
|---|---|
| SH001 | START V001 → END V001 |
| SH003 | START V001 (provisório) → END V002 |
| SH004 | START V001 → END V001 |
| SH005 | START V002 → END V001 |
| SH006 | START V001 → END V001 |
| SH007 | START V002 → END V002 |
| SH008 | START V001 → END V001 |
| SH009 | START V001 → END V001 |

---

## 5. Regra de uso

A partir deste ponto:
- não usar versões antigas se já existir uma versão travada melhor;
- qualquer nova regeneração deve nascer como `V003+` e justificar por que substitui o lock atual.

---

## 6. Diretiva final

**O pacote visual do EP01 agora está estável o suficiente para entrar em preparação de motion pass.**
