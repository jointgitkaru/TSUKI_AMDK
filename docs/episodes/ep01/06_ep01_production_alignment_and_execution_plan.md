# TSUKI_AMDK — EP01 · Plano de Alinhamento e Execução de Produção
### Production Alignment & Execution Plan

Status: `WORKING MASTER / RECOMMENDED PLAN`
Date: `2026-09-03`
Branch: `arena/01a06498-tsuki-amdk`

---

## 1) Objetivo / Objective

Este documento organiza o que já existe no repositório e propõe um caminho único para levar o **EP01 — CASO Nº 001: “O Biscoito Que Não Estava Lá”** até produção completa.

**Meta prática / Practical goal:**
- fechar o corte criativo do episódio;
- definir qual documento é fonte de verdade em cada área;
- listar os bloqueios de canon antes de gerar assets;
- transformar os materiais atuais em um pipeline executável de imagem, vídeo, áudio e master final.

---

## 2) Leitura do material atual / Current repo reading

### Documentos-base / Core files

| Arquivo | Função | Observação prática |
|---|---|---|
| `docs/core/00_episode_core.md` | Brief central do episódio | Define premissa, timeline factual e estrutura em 3 cenas |
| `docs/core/01_production_core.md` | Regras do sistema de produção | Define canon levels, camadas narrativas e anti-cliché protocol |
| `docs/episodes/ep01/01_script_ep01.md` | Roteiro canônico textual | Melhor fonte para narração, beats e intenção dramática |
| `docs/episodes/ep01/02_scene_cards.md` | Estrutura de cenas | Melhor fonte para propósito, estados de entrada/saída e continuidade macro |
| `docs/core/02_visual_bible.md` | Bíblia visual | Melhor fonte para câmera, luz, geografia e comportamento visual |
| `docs/episodes/ep01/03_shot_list_and_prompts.md` | Shot list curta + prompts de flow | Boa como versão operacional enxuta |
| `docs/episodes/ep01/04_ep01_image_prompts_master.md` | Pacote amplo de prompts | Forte para geração e derivação de assets |
| `docs/episodes/ep01/05_ep01_keyframes_nanbanana.md` | Storyboards + keyframes | Forte para execução de stills/start-end frames |
| `docs/episodes/ep01/05_episode_01_canonical_shotlist.md` | Shotlist cinematográfica expandida | Rica, mas hoje entra em conflito com o script e com a estrutura de abertura/fechamento |

---

## 3) Bloqueios de canon detectados / Canon blockers detected

Antes da produção final, há inconsistências que precisam ser tratadas como **decision gates**.

### Bloqueio A — Estrutura de planos: 9 shots vs 10 shots

**Conflito / Conflict:**
- `docs/episodes/ep01/03_shot_list_and_prompts.md` e `docs/episodes/ep01/05_ep01_keyframes_nanbanana.md` operam com **9 planos**.
- `docs/episodes/ep01/05_episode_01_canonical_shotlist.md` opera com **10 planos**.

**Impacto / Impact:**
- muda duração, ritmo e carga de geração;
- altera a montagem do episódio;
- muda quais frames precisam virar master.

### Bloqueio B — Moldura do dossiê existe ou não existe

**Conflito / Conflict:**
- `docs/core/00_episode_core.md`, `docs/episodes/ep01/01_script_ep01.md` e `docs/episodes/ep01/02_scene_cards.md` deixam claro que o episódio abre e fecha com a **pasta/dossiê**.
- `docs/episodes/ep01/05_episode_01_canonical_shotlist.md` não usa essa moldura como bookend central.

**Impacto / Impact:**
- isso muda a identidade formal da série;
- afeta abertura, encerramento e branding narrativo do universo.

### Bloqueio C — Evidência física: zero migalhas vs poucas migalhas

**Conflito / Conflict:**
- `docs/core/00_episode_core.md` e `docs/episodes/ep01/01_script_ep01.md` sugerem **ausência total de migalhas**.
- `docs/episodes/ep01/05_episode_01_canonical_shotlist.md` e alguns prompts usam **3 pequenas migalhas**.

**Impacto / Impact:**
- muda a lógica investigativa de Tsuki;
- muda inserts, keyframes e continuidade de vários planos.

### Bloqueio D — Humanos em quadro vs fora de quadro

**Conflito / Conflict:**
- vários materiais visuais reforçam **no people**.
- `docs/episodes/ep01/05_episode_01_canonical_shotlist.md` inclui um plano com **humano adulto desfocado ao fundo**.
- o roteiro usa a **humana pequena** como informação de Simba, mas não exige visualização dela.

**Impacto / Impact:**
- aumenta complexidade de geração;
- arrisca quebrar o foco procedural dos animais;
- muda o nível de revelação do mistério no EP01.

---

## 4) Recomendação de lock criativo / Recommended creative lock

### Versão recomendada para produção agora / Recommended production build now

**Eu recomendo consolidar o EP01 nesta forma:**

1. **Estrutura de 9 planos** como cut principal.
2. **Abertura e fechamento com o dossiê** obrigatórios.
3. **Zero migalhas como canon visual principal**.
4. **Nenhum humano visível em quadro** no EP01.
5. **Simba sabe a verdade, mas a informação permanece apenas no pensamento**.

### Por que esta versão é a mais forte / Why this version is strongest

- Está mais alinhada com o **core brief**, **script** e **scene cards**.
- Preserva a identidade procedural-arquivística da série.
- Simplifica produção e continuidade.
- Evita dispersão visual logo no piloto.
- Mantém o mistério pequeno, sério e elegante.

### Como tratar o material divergente / How to treat divergent material

- `docs/episodes/ep01/05_episode_01_canonical_shotlist.md` deve ser tratado, por enquanto, como **variant development file / expanded alternative**.
- Os materiais de 9 planos podem ser tratados como **production path A**.
- Se depois você quiser uma versão expandida, o arquivo de 10 planos pode virar **director’s cut / alt cut reference**.

---

## 5) Hierarquia de fonte de verdade / Source-of-truth hierarchy

Para evitar retrabalho, sugiro esta ordem:

### Story / Narrative truth
1. `docs/core/00_episode_core.md`
2. `docs/episodes/ep01/01_script_ep01.md`
3. `docs/episodes/ep01/02_scene_cards.md`

### Visual rules / Visual truth
1. `docs/core/02_visual_bible.md`
2. `docs/episodes/ep01/04_ep01_image_prompts_master.md`
3. `docs/episodes/ep01/05_ep01_keyframes_nanbanana.md`

### Execution / Production truth
1. `docs/episodes/ep01/03_shot_list_and_prompts.md`
2. `docs/episodes/ep01/05_ep01_keyframes_nanbanana.md`
3. este documento (`docs/episodes/ep01/06_ep01_production_alignment_and_execution_plan.md`)

---

## 6) Build recomendado do episódio / Recommended episode build

### Master cut de 9 planos / 9-shot master cut

| Ordem | Shot ID | Função dramática | Asset principal |
|---|---|---|---|
| 01 | S01_SH001 | Abrir o universo com a pasta | Dossiê fechado → aberto |
| 02 | S01_SH002 | Entrada investigativa de Tsuki | Tsuki + Cozinha Sul |
| 03 | S01_SH003 | Descoberta da tigela vazia | Tsuki + Cozinha Oeste + Tigela |
| 04 | S01_SH004 | Prova pericial da ausência | Inserto do perímetro / zero migalhas |
| 05 | S02_SH005 | Relação Tsuki vs Simba | Two-shot Norte |
| 06 | S02_SH006 | Simba guarda a verdade | Close de Simba / slow blink |
| 07 | S02_SH007 | Tsuki interpreta o blink | Close de Tsuki |
| 08 | S03_SH008 | Vigília ao entardecer | Wide final da cozinha |
| 09 | S03_SH009 | Fechamento canônico | Dossiê aberto → fechado carimbado |

---

## 7) Pipeline completo de produção / Complete production pipeline

## FASE 0 — LOCK / Canon lock

### Entregável
- decisão formal sobre os 4 bloqueios acima.

### Resultado mínimo para seguir
- shot count definido;
- estado da tigela/perímetro definido;
- política de humanos em quadro definida;
- moldura do dossiê confirmada ou removida.

### Recomendação prática
Se nada for decidido manualmente, usar o **lock recomendado da seção 4**.

---

## FASE 1 — REFERÊNCIAS / Reference package

### Objetivo
Garantir que todos os geradores usem o mesmo núcleo de identidade.

### Pacote que já existe
- `assets/references/characters/TSUKI_AMDK_CHAR_TSUKI_MASTER_V001.jpeg`
- `assets/references/characters/TSUKI_AMDK_CHAR_SIMBA_MASTER_V001.jpg`
- `assets/references/locations/TSUKI_AMDK_KITCHEN_Norte.png`
- `assets/references/locations/TSUKI_AMDK_KITCHEN_Sul.png`
- `assets/references/locations/TSUKI_AMDK_KITCHEN_Leste.png`
- `assets/references/locations/TSUKI_AMDK_KITCHEN_Oeste.png`
- `assets/references/props/TSUKI_AMDK_PROP_BISCUIT_BOWL.jpeg`
- `assets/references/props/TSUKI_AMDK_PROP_BISCUIT_BOWL_MACRO.jpeg`
- `assets/references/props/TSUKI_AMDK_PROP_DOG_BISCUIT_MASTER.jpeg`
- `assets/references/props/TSUKI_AMDK_PROP_BROKEN_DOG_BISCUIT_MASTER.jpeg`
- `assets/references/props/TSUKI_AMDK_PROP_CASE_FOLDER.jpeg`
- `assets/references/props/TSUKI_AMDK_PROP_CASE_FOLDER_OPEN.jpeg`
- `assets/references/props/TSUKI_AMDK_PROP_CASE_FOLDER_W_RUBBER.jpeg`

### Gate de aprovação
Cada referência deve ser classificada como:
- `[CHARACTER_REFERENCE]`
- `[LOCATION_REFERENCE]`
- `[OBJECT_REFERENCE]`
- `[MASTER]`

### Regra
Nenhum prompt de produção deve nascer sem citar:
- personagem;
- direção cardinal da cozinha;
- objeto, quando houver;
- gramática 16mm;
- regra de não-antropomorfização.

---

## FASE 2 — KEYFRAMES / Still generation

### Objetivo
Criar os frames aprovados que vão alimentar vídeo, continuidade e seleção final.

### Ordem recomendada de geração

#### Bloco A — Lock de look
1. SH001 start/end
2. SH003 start
3. SH005 start
4. SH008 start
5. SH009 end

#### Bloco B — Cobertura total
6. SH002
7. SH004
8. SH006
9. SH007
10. SH009 start

### Gate de aprovação por frame
- identidade de Tsuki correta;
- identidade de Simba correta;
- cozinha bate com o cardinal correto;
- altura de câmera baixa coerente;
- luz de fim de tarde coerente;
- textura 16mm presente;
- nada “fofo”, “cartoon” ou “humanizado”.

### Observação crítica
**SH004** é o plano mais sensível para canon, porque ele precisa confirmar claramente se o caso é:
- `ZERO_CRUMBS`, ou
- `THREE_CRUMBS`.

---

## FASE 3 — VÍDEO / Motion generation

### Objetivo
Transformar keyframes aprovados em planos com ação mínima, orgânica e observacional.

### Regra de performance
Os animais devem parecer reais, não performers humanos.

### Regra de câmera
- movimentos pequenos;
- sem virtuosismo gratuito;
- sem câmera “hero shot” digital;
- prioridade para `STATIC_OBSERVATIONAL`, `SUBTLE_PUSH`, `SLOW_PULL`, `MINIMAL_TRACK`.

### Recomendações por shot

| Shot | Movimento principal | Risco a evitar |
|---|---|---|
| SH001 | pasta abre + zoom out suave | parecer mágica demais |
| SH002 | tracking baixo paralelo | corrida ou energia cômica |
| SH003 | quase estático | exagero facial de Tsuki |
| SH004 | macro estático | sujeira inventada pelo modelo |
| SH005 | push-in lento | poses humanas dos animais |
| SH006 | blink lento único | blink dramático excessivo |
| SH007 | micro head tilt | acting caricatural |
| SH008 | quase imóvel / tempo passando | pôr do sol melodramático |
| SH009 | pasta fecha + zoom in | carimbo ou texto deformado |

---

## FASE 4 — ÁUDIO / Audio build

### Camadas de áudio / Audio layers

#### Layer 1 — Tsuki narration
Fonte: `docs/episodes/ep01/01_script_ep01.md`

**Qualidade desejada / Desired tone:**
- calma;
- seca;
- precisa;
- sem ironia;
- pausas calculadas.

#### Layer 2 — Simba internal thought
Fonte: `docs/episodes/ep01/01_script_ep01.md`

**Qualidade desejada / Desired tone:**
- maduro;
- econômico;
- observador;
- nunca sentimental.

#### Layer 3 — Ambiente / room tone
- geladeira distante;
- vento leve;
- ruído doméstico discreto;
- patas/unhas no chão quando necessário.

#### Layer 4 — Música
- piano menor;
- notas esparsas;
- resolução suspensa;
- nunca empurrar emoção demais.

### Estrutura recomendada de mix
- VO Tsuki sempre inteligível e dominante quando entra;
- pensamento de Simba levemente mais íntimo/seco;
- silêncio real como ferramenta dramática no interrogatório;
- música abaixo da palavra, não acima.

---

## FASE 5 — MONTAGEM / Editorial assembly

### Objetivo
Construir o episódio na faixa de **100–150s**, com alvo em **120s**.

### Corte recomendado / Recommended pacing

| Shot | Duração sugerida |
|---|---:|
| SH001 | 8s |
| SH002 | 12s |
| SH003 | 14s |
| SH004 | 8s |
| SH005 | 18s |
| SH006 | 10s |
| SH007 | 10s |
| SH008 | 24s |
| SH009 | 16s |
| **TOTAL** | **120s** |

### Lógica de ritmo
- CENA 1 constrói método.
- CENA 2 sustenta tensão pelo silêncio.
- CENA 3 não “resolve”; ela formaliza o fracasso parcial.

---

## FASE 6 — QC / Quality control

### Checklist final de aprovação

#### Canon
- [ ] Tsuki bate com master aprovado
- [ ] Simba bate com master aprovado
- [ ] Geografia da cozinha coerente
- [ ] Prop do biscoito segue versão canônica
- [ ] Tigela segue posição/estado aprovados

#### Visual
- [ ] Linguagem 16mm coerente
- [ ] Sem aparência CGI/cartoon
- [ ] Sem antropomorfização
- [ ] Sem exagero de luz “cinematográfica artificial”
- [ ] Sem enquadramentos que pareçam publicidade pet

#### Narrativa
- [ ] Tsuki não soa irônica
- [ ] Simba não entrega demais
- [ ] Mistério permanece aberto
- [ ] Final não parece moral fechado

#### Áudio
- [ ] Vozes claras
- [ ] Música discreta
- [ ] Silêncio usado com intenção
- [ ] Foley não compete com narração

#### Export
- [ ] Master final revisado do início ao fim
- [ ] Nome de export coerente
- [ ] Versão, data e status registrados

---

## 8) Convenção de naming / Naming convention

### Arquivos de imagem
`TSUKI_AMDK_E01_S01_SH001_START_V001.png`

### Arquivos de vídeo
`TSUKI_AMDK_E01_S02_SH005_TAKE03_V001.mp4`

### Áudio de voz
`TSUKI_AMDK_E01_VO_TSUKI_PT_V001.wav`
`TSUKI_AMDK_E01_VO_SIMBA_PT_V001.wav`

### Masters
`TSUKI_AMDK_E01_MASTER_LOCKED_V001.mov`
`TSUKI_AMDK_E01_MASTER_SUBS_V001.mp4`

---

## 9) O que já está pronto vs o que falta / Ready vs missing

### Já bastante maduro / Already mature
- conceito do episódio;
- script base;
- scene architecture;
- universo visual;
- referências principais;
- prompt pack robusto.

### Ainda falta fechar / Still to lock
- uma única versão de shot structure;
- um único estado de evidência física;
- política de presença humana;
- decisão oficial sobre qual arquivo é o master operacional.

### Ainda falta produzir / Still to produce
- seleção final de keyframes aprovados;
- vídeos por shot;
- vozes finais;
- trilha/ambiente final;
- montagem final do episódio.

---

## 10) Próxima ação recomendada / Recommended next action

### Se você quiser avançar agora, minha sugestão é esta:

**Passo 1.** Eu consolido um **MASTER OPERACIONAL DO EP01** em um único arquivo.  
Esse arquivo pode juntar:
- estrutura final de 9 planos;
- prompts prontos por shot;
- durations;
- falas/narrações por plano;
- checklist de aprovação por shot.

**Passo 2.** Depois eu crio um **ASSET TRACKER DE PRODUÇÃO** para controlar:
- referência;
- keyframe;
- take de vídeo;
- áudio;
- status;
- aprovado/rejeitado.

**Passo 3.** Se quiser, eu também posso transformar isso em:
- pacote de prompts final;
- planilha de produção;
- ordem de render;
- guia de montagem.

---

## 11) Decisão recomendada, em uma linha / One-line recommendation

**Produza primeiro a versão de 9 planos com dossiê abrindo/fechando, zero migalhas, nenhum humano em quadro e foco total no silêncio entre Tsuki e Simba.**
