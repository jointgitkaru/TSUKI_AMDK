# TSUKI_AMDK

> **PT-BR**: Bíblia de produção, canon visual e pipeline de assets para **TSUKI — O Arquivo Morto da Cozinha**.  
> **EN**: Production bible, visual canon, and asset pipeline for **TSUKI — The Dead Kitchen Archive**.

## Overview

`TSUKI_AMDK` organiza o desenvolvimento completo de uma série curta centrada em **Tsuki**, uma schnauzer miniatura investigadora, e **Simba**, um siamês que quase sempre sabe mais do que diz.

O repositório reúne:
- canon narrativo;
- bíblia visual;
- prompts de imagem e vídeo;
- organização de produção do **EP01**;
- rastreamento de assets;
- vozes geradas;
- stills e renders de revisão.

## Current status

- **Project phase:** pre-production / visual development
- **Current focus:** `EP01 — CASO Nº 001 — O Biscoito Que Não Estava Lá`
- **Build in progress:** 9-shot operational cut
- **Visual lock:** 16mm observational domestic procedural
- **Scale lock:** active via dimensional reference

## Recommended starting points

### Read first
- [`docs/core/00_episode_core.md`](docs/core/00_episode_core.md)
- [`docs/core/01_production_core.md`](docs/core/01_production_core.md)
- [`docs/core/02_visual_bible.md`](docs/core/02_visual_bible.md)

### Episode 01 operational docs
- [`docs/episodes/ep01/07_ep01_operational_master.md`](docs/episodes/ep01/07_ep01_operational_master.md)
- [`docs/episodes/ep01/08_ep01_asset_tracker.md`](docs/episodes/ep01/08_ep01_asset_tracker.md)
- [`docs/episodes/ep01/09_ep01_final_prompt_package.md`](docs/episodes/ep01/09_ep01_final_prompt_package.md)
- [`docs/episodes/ep01/14_ep01_editorial_timeline_map.md`](docs/episodes/ep01/14_ep01_editorial_timeline_map.md)

### Reviews and corrections
- [`docs/episodes/ep01/16_ep01_dimensional_lock.md`](docs/episodes/ep01/16_ep01_dimensional_lock.md)
- [`docs/episodes/ep01/17_ep01_scale_correction_review.md`](docs/episodes/ep01/17_ep01_scale_correction_review.md)
- [`docs/episodes/ep01/18_ep01_sh007_regen_review.md`](docs/episodes/ep01/18_ep01_sh007_regen_review.md)

## Repository structure

```text
TSUKI_AMDK/
├── README.md
├── assets/
│   └── references/
│       ├── characters/
│       ├── dimensional/
│       ├── locations/
│       └── props/
├── docs/
│   ├── core/
│   ├── episodes/
│   │   └── ep01/
│   └── storyboards/
├── outputs/
│   ├── audio/
│   └── renders/
└── .github/
```

## Production logic

```text
DEFINE → REFERENCE → DESIGN → GENERATE → REVIEW → SELECT → PRESERVE → CONTINUE
```

## Canon summary

### Project rules
- Tsuki has **zero ironic consciousness**.
- Simba has **total observational irony**, but it remains internal.
- Pets understand humans; humans do not understand pets.
- The project avoids pet-commercial language, cartoon behavior, and generic AI melodrama.

### EP01 lock
- **9 shots**
- **dossier opens and closes the episode**
- **zero crumbs** as the main forensic condition
- **no visible humans in frame**
- **case remains open** at the end

## Asset references

### Characters
- [`assets/references/characters/TSUKI_AMDK_CHAR_TSUKI_MASTER_V001.jpeg`](assets/references/characters/TSUKI_AMDK_CHAR_TSUKI_MASTER_V001.jpeg)
- [`assets/references/characters/TSUKI_AMDK_CHAR_SIMBA_MASTER_V001.jpg`](assets/references/characters/TSUKI_AMDK_CHAR_SIMBA_MASTER_V001.jpg)

### Locations
- [`assets/references/locations/TSUKI_AMDK_KITCHEN_Norte.png`](assets/references/locations/TSUKI_AMDK_KITCHEN_Norte.png)
- [`assets/references/locations/TSUKI_AMDK_KITCHEN_Sul.png`](assets/references/locations/TSUKI_AMDK_KITCHEN_Sul.png)
- [`assets/references/locations/TSUKI_AMDK_KITCHEN_Leste.png`](assets/references/locations/TSUKI_AMDK_KITCHEN_Leste.png)
- [`assets/references/locations/TSUKI_AMDK_KITCHEN_Oeste.png`](assets/references/locations/TSUKI_AMDK_KITCHEN_Oeste.png)

### Props and scale
- [`assets/references/props/TSUKI_AMDK_PROP_BISCUIT_BOWL.jpeg`](assets/references/props/TSUKI_AMDK_PROP_BISCUIT_BOWL.jpeg)
- [`assets/references/props/TSUKI_AMDK_PROP_CASE_FOLDER.jpeg`](assets/references/props/TSUKI_AMDK_PROP_CASE_FOLDER.jpeg)
- [`assets/references/dimensional/Tsuki e Simba - referencia visual e dimencional.png`](assets/references/dimensional/Tsuki%20e%20Simba%20-%20referencia%20visual%20e%20dimencional.png)

## Outputs

See [`outputs/README.md`](outputs/README.md).

### Audio
Generated voice clips live in `outputs/audio/` locally.

### Renders
Keyframes, contact sheets, and review stills live in `outputs/renders/` locally.

## GitHub profile suggestion

**Suggested description:**  
Production bible, visual canon, prompts, and asset pipeline for TSUKI — O Arquivo Morto da Cozinha.

**Suggested topics:**  
`ai-filmmaking`, `storyboard`, `preproduction`, `visual-development`, `prompt-design`, `short-film`, `worldbuilding`, `audio-post`

## Notes

- The repository is documentation-first.
- Output assets are organized as reviewable production material, not final delivery masters.
- The current production pass includes generated stills and voice samples for EP01.

## License / rights

No license file is defined yet. Add one before public reuse or external distribution.
