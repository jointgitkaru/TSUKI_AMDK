# TSUKI_AMDK — EP01 · Editorial Timeline Map
### Mapa editorial com vozes geradas

Status: `READY FOR ASSEMBLY`
Base duration target: `120s`
Voice assets generated: `YES`

---

## 1. Duração real dos clips gerados / Actual generated clip durations

| Asset | Duração |
|---|---:|
| `TSUKI_AMDK_E01_VO_TSUKI_01_PT.wav` | 15.24s |
| `TSUKI_AMDK_E01_VO_TSUKI_02_PT.wav` | 19.36s |
| `TSUKI_AMDK_E01_VO_TSUKI_03_PT.wav` | 26.52s |
| `TSUKI_AMDK_E01_VO_TSUKI_04_PT.wav` | 12.64s |
| `TSUKI_AMDK_E01_VO_SIMBA_01_PT.wav` | 16.24s |
| `TSUKI_AMDK_E01_VO_SIMBA_02_PT.wav` | 17.40s |

### Observação importante
A soma bruta das vozes é alta para um episódio de 120s se tudo tocar em série.
Portanto, a montagem ideal deve usar:
- sobreposição parcial controlada entre Tsuki e Simba;
- pausas reais;
- sustains visuais mais longos com pouca fala;
- possível trim fino de respiros em edição, sem deformar performance.

---

## 2. Estratégia editorial recomendada / Recommended editorial strategy

### Princípio
- Tsuki conduz a estrutura factual.
- Simba entra como camada interna, não como bloco separado demais.
- SH005–SH007 devem operar como um miolo de tensão com **sobreposição inteligente** de camadas narrativas.

### Overlap recomendado
- `VO_TSUKI_03` começa em SH005 e atravessa para SH006.
- `VO_SIMBA_01` entra em SH006 por baixo ou logo após o primeiro terço da fala de Tsuki.
- `VO_SIMBA_02` entra em SH007 sem pressa, podendo terminar nos primeiros segundos de SH008 se a montagem pedir ar.

---

## 3. Timeline sugerida / Suggested timeline

| Faixa de tempo | Shot | Ação editorial |
|---|---|---|
| 00:00–00:08 | SH001 | pasta abre, sem voz, só som e acorde inicial |
| 00:08–00:20 | SH002 | entrar `VO_TSUKI_01` início |
| 00:20–00:23 | SH003 | `VO_TSUKI_01` continua e termina |
| 00:23–00:34 | SH003 | sustentar sniffing e silêncio curto |
| 00:34–00:42 | SH004 | `VO_TSUKI_02` entra |
| 00:42–00:53 | SH005 | `VO_TSUKI_02` continua |
| 00:53–01:00 | SH005 | silêncio tenso, sem pressa |
| 01:00–01:10 | SH006 | iniciar `VO_TSUKI_03` |
| 01:10–01:20 | SH007 | `VO_TSUKI_03` continua |
| 01:20–01:26 | SH007/SH008 ponte | finalizar `VO_TSUKI_03` |
| 01:06–01:22 | SH006–SH007 overlap | entrar `VO_SIMBA_01` em camada íntima |
| 01:22–01:39 | SH007–SH008 overlap | entrar `VO_SIMBA_02` |
| 01:31–01:44 | SH008 | `VO_TSUKI_04` entra e conclui |
| 01:44–02:00 | SH009 | sem fala principal; som da pasta e acorde final |

---

## 4. Patch verbal por shot / Verbal patch by shot

## SH001
- **fala:** nenhuma
- **função:** preparar escuta

## SH002
- **fala principal:** Tsuki 01
- **uso:** começar a factualidade do caso

## SH003
- **fala principal:** final de Tsuki 01
- **uso:** casar “o objeto não existia mais” com a tigela vazia

## SH004
- **fala principal:** Tsuki 02
- **uso:** plano pericial puro, pouca concorrência sonora

## SH005
- **fala principal:** fim de Tsuki 02 + silêncio
- **uso:** segurar tensão antes do blink

## SH006
- **fala principal:** Tsuki 03 + início de Simba 01
- **uso:** dividir sentido entre hipótese errada e verdade retida

## SH007
- **fala principal:** final de Tsuki 03 + Simba 01/02
- **uso:** contra-ponto entre dedução de Tsuki e reserva de Simba

## SH008
- **fala principal:** final de Simba 02 + Tsuki 04
- **uso:** elipse emocional e retorno ao protocolo

## SH009
- **fala principal:** nenhuma
- **uso:** pasta fecha, caso permanece aberto

---

## 5. Recomendação de níveis relativos / Relative level suggestion

Escala simples, apenas como guia de intenção:

| Elemento | Nível relativo |
|---|---:|
| Tsuki VO | 0 dB referência |
| Simba VO | -1.5 a -3 dB abaixo de Tsuki |
| Room tone | -18 a -24 dB |
| Foley leve | -14 a -20 dB |
| Piano | -20 a -28 dB |

### Nota
Simba pode ficar um pouco mais íntimo/fechado no campo, mas não mais alto que Tsuki.

---

## 6. Ajustes editoriais prováveis / Likely editorial adjustments

### Se o episódio ficar falado demais
- reduzir respirações entre frases;
- encurtar pausas internas dos clips de Tsuki;
- iniciar Simba ligeiramente antes por overlap;
- deixar SH008 respirar mais pela imagem e menos pela palavra.

### Se o episódio ficar corrido demais
- manter SH005 e SH008 como shots de respiração;
- não acelerar artificialmente as vozes;
- alongar room tone entre camadas.

---

## 7. Uso prático / Practical use

Este documento já permite montar um **assembly cut** mesmo antes de mix final.
Use-o junto com:
- `docs/episodes/ep01/07_ep01_operational_master.md`
- `docs/episodes/ep01/11_ep01_voice_recording_direction.md`
- `docs/episodes/ep01/12_ep01_audio_mix_and_cue_sheet.md`
- `docs/episodes/ep01/08_ep01_asset_tracker.csv`

---

## 8. Diretiva final

**Na montagem, a voz de Tsuki organiza os fatos; a de Simba reorganiza o sentido.**
