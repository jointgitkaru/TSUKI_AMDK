# TSUKI_AMDK — EP01 · Assembly Blueprint
### Blueprint de montagem usando stills travados + vozes geradas

Status: `READY FOR PRE-ASSEMBLY`
Target duration: `~120s`

---

## 1. Objetivo

Este blueprint permite montar um corte preliminar do EP01 mesmo antes do motion final.

Ele serve para:
- testar ritmo;
- validar duração;
- checar excesso de fala;
- planejar transições e silêncios.

---

## 2. Base do corte

### Imagem
Usar os stills travados listados em:
- `docs/episodes/ep01/19_ep01_locked_stills_manifest.md`

### Voz
Usar os clips gerados listados em:
- `docs/episodes/ep01/13_ep01_voice_cast_registry.md`
- `docs/episodes/ep01/14_ep01_editorial_timeline_map.md`

### Som de base
Mesmo sem stems finais, o pre-assembly já pode usar:
- room tone placeholder leve;
- silêncio construído;
- marcas simples de entrada/saída musical.

---

## 3. Estrutura do corte por shot

| Shot | Duração alvo | Imagem base | Função editorial |
|---|---:|---|---|
| SH001 | 8s | START→END dossiê | abrir escuta e linguagem |
| SH002 | 12s | hold/slow move | entrada factual de Tsuki |
| SH003 | 14s | aproximação + inspeção | descoberta da ausência |
| SH004 | 8s | macro forense | tese de zero migalhas |
| SH005 | 18s | two-shot silencioso | pressão dramática |
| SH006 | 10s | close Simba | beat do blink |
| SH007 | 10s | close Tsuki | formulação da hipótese |
| SH008 | 24s | vigília | tempo, espera, caso aberto |
| SH009 | 16s | dossiê fecha | encerramento formal |

---

## 4. Voice placement

### SH001
- sem voz
- som do dossiê + acorde inicial

### SH002 → SH003
- `VO_TSUKI_01`
- terminar a frase “o objeto não existia mais” sobre a leitura da tigela vazia

### SH004 → início de SH005
- `VO_TSUKI_02`
- deixar a última frase cair com peso factual, não com suspense de trailer

### SH005 → SH006 → SH007
- `VO_TSUKI_03` atravessa os shots
- `VO_SIMBA_01` entra por overlap em SH006
- `VO_SIMBA_02` assume SH007 e pode avançar um pouco em SH008

### SH008
- `VO_TSUKI_04`
- deve soar como protocolo de vigilância, não tristeza

### SH009
- sem fala principal
- nota de rodapé pode entrar como texto on-screen apenas

---

## 5. Transition plan

| De | Para | Tipo de transição |
|---|---|---|
| SH001 | SH002 | corte direto |
| SH002 | SH003 | continuidade de ação / corte simples |
| SH003 | SH004 | corte para insert |
| SH004 | SH005 | corte seco |
| SH005 | SH006 | contra-plano |
| SH006 | SH007 | contra-plano |
| SH007 | SH008 | elipse temporal suave |
| SH008 | SH009 | dissolve/fade curto |

---

## 6. Pre-assembly build suggestion

### Pass 1 — imagem dura
- montar os 9 shots com duração provisória
- usar stills com pequenos pushes e holds se motion ainda não existir

### Pass 2 — voz
- encaixar Tsuki como espinha factual
- inserir Simba como contraponto interno

### Pass 3 — silêncio
- proteger SH005 e SH006 de preenchimento excessivo

### Pass 4 — música mínima
- só marcar começo, dobra do interrogatório e fechamento

---

## 7. Warning points

### Excesso de fala
Se o episódio parecer verbal demais:
- cortar respiros menos importantes;
- aumentar overlap entre Tsuki e Simba;
- deixar SH008 carregar mais peso visual.

### Excesso de imagem estática
Se o pre-assembly parecer parado demais:
- usar pushes lentos muito discretos;
- variar duração por tensão, não por enfeite;
- não compensar com música excessiva.

### Quebra de canon
Reprovar qualquer montagem que faça:
- Tsuki soar irônica;
- Simba soar como vilão teatral;
- o final parecer resolvido;
- o caso perder sua pequena escala doméstica.

---

## 8. Deliverable suggestion

Quando o pre-assembly existir, criar:
- `TSUKI_AMDK_E01_ASSEMBLY_STILLS_V001`
- `TSUKI_AMDK_E01_MASTER_REVIEW_NOTES_V001.md`

---

## 9. Diretiva final

**Mesmo sem motion final, o episódio já pode ser testado como montagem de ritmo e sentido.**
