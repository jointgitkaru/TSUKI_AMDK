# TSUKI_AMDK — Dimensional Lock
### Aplicado ao EP01 a partir de 2026-09-03

Status: `ACTIVE SCALE CORRECTION GUIDE`

---

## 1. Motivo

Este documento corrige um problema detectado nas primeiras gerações de stills: **desproporção de escala entre Tsuki, Simba e o ambiente**.

A partir deste ponto, toda geração visual do EP01 deve usar a referência:

- `assets/references/dimensional/Tsuki e Simba - referencia visual e dimencional.png`

como **guia dimensional prioritário**.

---

## 2. Lock dimensional principal

### Tsuki
- altura na cernelha: **33 cm**
- altura total em pé: **46 cm**
- comprimento corporal: **41 cm**
- largura máxima: **16 cm**
- profundidade máxima: **19 cm**
- cauda: **13 cm**
- leitura visual: **pequena, compacta, robusta, nunca porte médio**

### Simba
- altura na cernelha: **33 cm**
- altura total em pé: **42 cm**
- comprimento corporal: **38 cm**
- largura máxima: **16 cm**
- profundidade máxima: **18 cm**
- cauda: **25 cm**
- leitura visual: **esguio, leve, estreito, ligeiramente menor na presença total do que Tsuki**

---

## 3. Regra visual simplificada

Se a imagem estiver “visualmente correta”, ela deve ler assim:

- Tsuki é **mais volumosa** que Simba.
- Simba é **mais fino e leve** que Tsuki.
- Nenhum dos dois deve parecer grande demais para a cozinha.
- Tsuki nunca deve parecer cão de porte médio.
- Simba nunca deve parecer gato grande demais para a janela, bancada ou cadeira.

---

## 4. Regra para planos abertos

Em planos wide ou medium-wide:
- os animais devem ocupar uma fração modesta do ambiente;
- rodapés, portas, cadeiras, pernas de mesa, peitoril e gabinete devem servir de controle de escala;
- a tigela deve parecer pequena e compatível com um schnauzer miniatura;
- evitar qualquer sensação de “bowl gigante” ou “dog oversized”.

---

## 5. Regra para planos com ambos os personagens

Quando Tsuki e Simba aparecem no mesmo quadro:
- Tsuki deve ler como **mais robusta e um pouco mais dominante em massa**;
- Simba deve ler como **mais estreito e elegante**;
- a diferença não é cartunesca, é sutil e realista;
- a perspectiva de lente pode variar, mas não pode destruir a leitura de escala.

---

## 6. Diretiva prática para prompts

Adicionar sempre, quando houver corpo inteiro ou meia distância:

```text
Use the supplied dimensional reference as a scale guide. Tsuki must read as a small compact Miniature Schnauzer, never medium-sized. Simba must read as a slim Siamese with lighter mass and slightly smaller total presence than Tsuki. Keep both animals modest in relation to cabinet height, chair legs, bowl size, window sill, and door proportions.
```

---

## 7. Política de correção

- novos stills já devem nascer sob este lock;
- stills antigos com distorção evidente de escala devem ser regenerados em versões `V002+`;
- a revisão é visual-prática, não matemática milimétrica de cada quadro.

---

## 8. Regra final

**Se a cozinha parecer pequena demais para os animais, a imagem falhou no lock dimensional.**
