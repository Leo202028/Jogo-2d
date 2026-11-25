# Floresta dos Olhos Rubros — RPG 2D Top-Down

Jogo 2D de RPG em visão superior (top-down) desenvolvido em **HTML5 Canvas + JavaScript puro + CSS3**.

## Como executar

### Opção 1 — Direto no navegador (mais simples)
1. Abra o arquivo `index.html` com um duplo clique no seu navegador preferido (Chrome, Edge, Firefox).

### Opção 2 — Servidor local (opcional)
```bash
python -m http.server 8000
```
Depois acesse `http://localhost:8000` no navegador.

## Controles
- **Movimentação:** `W`, `A`, `S`, `D` ou **Setas direcionais**
- **Atacar (espada):** `Espaço`, `J` ou **Clique esquerdo** na direção desejada
- **Trocar roupa equipada:** Teclas `1`, `2`, `3`, `4`
- **Pausar / Continuar:** `P` ou `Esc`
- **Silenciar som:** `M`

## Estrutura do projeto
- `index.html` — Estrutura da página e telas de Início, Pausa e Fim de Jogo
- `style.css` — Estilos visuais das telas e do palco do jogo
- `js/config.js` — Configurações gerais, catálogo de roupas e definições dos monstros
- `js/mapa.js` — Geração do mapa da floresta, obstáculos e colisões
- `js/sprites.js` — Desenho top-down do herói vestido, monstros verdes de olhos vermelhos e itens
- `js/entidades.js` — Classes `Heroi` e `Monstro` (com 3 comportamentos de IA distintos)
- `js/combate.js` — Fórmula de dano (ataque vs defesa), ataque em arco e efeitos visuais
- `js/progressao.js` — Experiência (XP), subida de nível, drops de poções e roupas
- `js/interface.js` — HUD no canvas (vida, XP, roupas, minimapa) e controle das telas modais
- `js/jogo.js` — Loop principal (`requestAnimationFrame`), áudio Web Audio e entrada do jogador

