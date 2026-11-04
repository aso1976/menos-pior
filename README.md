# Quem é menos pior? 90 casos mapeados

Mapa interativo do artigo **“Mas afinal, quem é menos pior?”**, de André Oliveira.

90 casos de lulismo, bolsonarismo e STF (versão 2 do levantamento, com 115 candidatos triados), posicionados por **alvo** (Estado ou eleitor) e por **modo** (corrosão ou ruptura). Passe o mouse ou toque num ponto para ver a ficha do caso: notas, descrição, crítica e defesa (STF) e a prova documental. Clique duas vezes no ponto (no celular, toque duas vezes ou use “Ler o caso”) para abrir o resumo do caso com as fontes.

O botão **Desconsiderados (25)** mostra, sozinhos, os candidatos que não passaram pela triagem. Eles foram pontuados com as mesmas réguas e numerados de X1 a X25 pela ordem de impacto deles, sem entrar nas médias nem nas contagens dos 90. O ícone segue o grupo de origem; o quadrado laranja indica casos compartilhados entre os campos.

- Artigo: https://aso1976.medium.com/mas-afinal-quem-%C3%A9-menos-pior-5e52204fe4d8
- Versão Datawrapper: https://datawrapper.dwcdn.net/ck9pJ/

## Arquivos

| Arquivo | Conteúdo |
|---|---|
| `index.html` | Página do mapa interativo (HTML, CSS e JavaScript num único arquivo, sem dependências externas) |
| `mapa-danos.png` | Imagem estática do mapa, para compartilhamento |
| `dados-90-casos.csv` | Dados dos 90 casos: coordenadas, notas P·V·C·R·G, descrição e prova |
| `dados-desconsiderados.csv` | Dados dos 25 Desconsiderados (X1–X25): grupo de origem, filtro de exclusão, notas e coordenadas |
| `resumos.json` | Resumos dos 115 casos, com as fontes, usados no pop-up do mapa |
| `.nojekyll` | Faz o GitHub Pages servir os arquivos como estão |

## Método

Cada caso recebe notas de 0 a 4 em cinco critérios — P (atinge o Estado), V (atinge o eleitor), C (contesta legitimidade), R (força ou coerção) e G (corrosão oculta) — e uma fórmula fixa converte as notas em coordenadas:

- X = 50 + 10 × (V − P)
- Y = 50 + 10 × ((C + R) / 2 − G)
- Impacto = P + V + (C + R) / 2 + G

Um ponto sobre uma linha pertence ao quadrante da direita ou de cima.

## Publicação no GitHub Pages

Settings → Pages → Build and deployment → Source: *Deploy from a branch*, branch `main`, pasta `/ (root)`.
