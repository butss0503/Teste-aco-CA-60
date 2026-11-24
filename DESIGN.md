---
name: Controle de Qualidade CA-60 — Grande Aço
description: Painel de laboratório para lançamento, conferência e certificação de ensaios de tração ABNT NBR 7480.
world: "Placa de Sinalização"
colors:
  chao: "#eceeea"
  placa: "#ffffff"
  placa-recuada: "#f6f7f4"
  placa-trilho: "#e3e6e1"
  linha: "#d3d7d1"
  linha-forte: "#a9afa8"
  grafite: "#151b21"
  corpo: "#2c3338"
  nota: "#5b6267"
  ceu-ga: "#3aa8e4"
  acao: "#0a64a8"
  acao-forte: "#084f86"
  acao-tinta: "#e3f1fb"
  aprovado: "#17803f"
  aprovado-texto: "#15803d"
  aprovado-texto-escuro: "#5ad98a"
  reprovado: "#c4231a"
  reprovado-texto: "#b91c1c"
  reprovado-texto-escuro: "#ff8a80"
  atencao: "#f2b705"
  atencao-texto: "#7a5000"
  nota-certificado: "#4b5257"
  chao-escuro: "#0c1014"
  placa-escura: "#151b21"
typography:
  display:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "22px"
    fontWeight: 800
    fontStretch: "125%"
    lineHeight: 1.05
  kpi:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "30px"
    fontWeight: 800
    fontStretch: "125%"
  veredito:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 800
    fontStretch: "125%"
  titulo-placa:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "15px"
    fontWeight: 800
    fontStretch: "125%"
  body:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.5
  campo:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "15px"
    fontWeight: 500
  dado:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "13px"
    fontWeight: 400
  apoio:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "12px"
    fontWeight: 400
  rotulo:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "11px"
    fontWeight: 700
    letterSpacing: "0.08em"
  medida:
    fontFamily: "JetBrains Mono, ui-monospace, monospace"
    fontSize: "13px"
    fontWeight: 400
  relogio:
    fontFamily: "JetBrains Mono, ui-monospace, monospace"
    fontSize: "26px"
    fontWeight: 700
  relogio-grande:
    fontFamily: "JetBrains Mono, ui-monospace, monospace"
    fontSize: "72px"
    fontWeight: 700
  bitola:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: 800
rounded:
  none: "0px"
  selo: "50%"
spacing:
  s1: "4px"
  s2: "8px"
  s3: "12px"
  s4: "16px"
  s5: "20px"
  s6: "24px"
  s8: "32px"
  s10: "40px"
components:
  placa:
    backgroundColor: "{colors.placa}"
    rounded: "{rounded.none}"
  placa-cabecalho:
    backgroundColor: "{colors.grafite}"
    textColor: "{colors.placa}"
    typography: "{typography.titulo-placa}"
    height: "52px"
  botao-primario:
    backgroundColor: "{colors.acao}"
    textColor: "{colors.placa}"
    rounded: "{rounded.none}"
    height: "48px"
  botao:
    backgroundColor: "{colors.placa}"
    textColor: "{colors.grafite}"
    rounded: "{rounded.none}"
    height: "40px"
  campo:
    backgroundColor: "{colors.placa}"
    textColor: "{colors.grafite}"
    rounded: "{rounded.none}"
    height: "42px"
  bitola-selecionada:
    backgroundColor: "{colors.ceu-ga}"
    textColor: "{colors.grafite}"
  veredito-aprovado:
    backgroundColor: "{colors.aprovado}"
    textColor: "{colors.placa}"
  veredito-reprovado:
    backgroundColor: "{colors.reprovado}"
    textColor: "{colors.placa}"
---

# Design System: Controle de Qualidade CA-60 — Grande Aço

## Overview

**Creative North Star: "Placa de Sinalização"**

O laboratório é um chão de fábrica sinalizado. Cada painel é uma placa: face branca, faixa de cabeçalho grafite com o título em letra larga e um quadrado azul-céu da Grande Aço. A cor fala como nas placas de segurança: azul é ação, verde é aprovado, vermelho é reprovado, âmbar é atenção. Nenhuma cor aparece sem esse significado.

A identidade vem do logo real (`Grandeaco.jpeg`): azul-céu, preto-grafite, uma grotesca larga e pesada para o nome e uma mono para o subtítulo. Aqui a Archivo em largura 125% e peso 800 faz o papel da letra do logo; a JetBrains Mono faz o papel da mono e é usada para o que é medido: valores de ensaio, datas e o relógio da ronda.

**Key Characteristics:**
- Placas retas (raio 0); o único círculo é o selo da marca.
- Cabeçalho de placa em faixa grafite; o chão (fundo da página) é um cinza claro, a placa é branca.
- Cor = significado de sinalização. Status nunca decora.
- Números medidos em mono com algarismos tabulares, alinhados à direita nas tabelas.
- O laudo é uma placa que fica inteira verde ou vermelha.
- O alarme da ronda é a única placa de perigo: faixa zebrada âmbar e grafite.
- Tema claro e escuro por tokens; o certificado é sempre papel branco.

## Colors

### Marca e ação
- **Céu GA** (#3aa8e4): o azul do logo. Fundo (nunca texto sobre branco): bitola selecionada, quadrado das placas, ícone de upload, aba ativa, linha recém-gravada. Texto sobre ele é sempre Grafite.
- **Ação** (#0a64a8): botão primário, links de ação, lote na tabela, linha do gráfico. Contraste 6,2:1 sobre branco. Hover: **Ação Forte** (#084f86).

### Neutros
- **Chão** (#eceeea) fundo da página · **Placa** (#ffffff) · **Placa recuada** (#f6f7f4) barras de filtro e cabeçalho de tabela · **Placa trilho** (#e3e6e1) etiqueta de bitola e trilho do progresso.
- **Linha** (#d3d7d1) divisórias · **Linha forte** (#a9afa8) contorno de campo e botão.
- **Grafite** (#151b21) títulos e faixas de cabeçalho · **Corpo** (#2c3338) texto · **Nota** (#5b6267) apoio, 5,5:1.

### Sinalização (status)
- **Aprovado** (#17803f) fundo com texto branco; como texto use #15803d (claro) ou #5ad98a (escuro).
- **Reprovado** (#c4231a) fundo com texto branco; como texto use #b91c1c (claro) ou #ff8a80 (escuro). Também: limite mínimo nos gráficos e LE abaixo de 600 na tabela.
- **Atenção** (#f2b705) só como fundo ou faixa; como texto use #7a5000. Massa fora de ±6% e a faixa zebrada do alarme.

### Named Rules
**The Signage Rule.** Cada cor tem um único significado: azul age, verde aprova, vermelho reprova, âmbar alerta. Bitolas, categorias e navegação usam grafite e céu, nunca status.

**The Sky Is Ground Rule.** O Céu GA é superfície. Texto azul usa a cor Ação.

## Typography

**Display:** Archivo 800, largura 125% (a letra larga do logo).
**Texto:** Archivo 400/500/700, largura normal.
**Medida e tempo:** JetBrains Mono, algarismos tabulares.

- **Display** (22px/800/125%): título do sistema.
- **KPI** (30px/800/125%): números da faixa do turno.
- **Veredito** (18px/800/125%): APROVADO / REPROVADO.
- **Título de placa** (15px/800/125%, caixa alta).
- **Campo** (15px/500): valor digitado; campos numéricos em mono.
- **Dado** (13px): células; valores medidos em mono, à direita.
- **Rótulo** (11px/700/0.08em, caixa alta): rótulos de campo, cabeçalhos de tabela.
- Piso: nenhum texto funcional abaixo de 11px.

**The Measured In Mono Rule.** Mono só para o que foi medido ou contado: MPa, mm, g/mm, %, datas, relógio. Nunca para rótulo ou enfeite.

## Layout

Cabeçalho branco com selo e ações → faixa grafite do turno (4 indicadores + relógio da ronda) → bancada: placa de lançamento (360–440px, fixa ao rolar) à esquerda e placa de dados fluida à direita, até 1680px. A página rola normalmente; a tabela rola dentro da placa com cabeçalho fixo.

- Abaixo de 1180px: as placas empilham (lançamento → dados).
- Abaixo de 900px: a faixa do turno quebra; os botões do cabeçalho viram só ícone (com nome acessível).
- Abaixo de 640px: indicadores 2×2, bitolas 3×2, placas de borda a borda, tabela com rolagem horizontal.

Espaçamento em passos de 4px (4, 8, 12, 16, 20, 24, 32, 40).

## Elevation & Depth

Plano. Separação por linha de 1px e por degrau tonal (chão → placa → placa recuada) e pela faixa grafite. Diálogos usam o véu grafite e uma entrada curta de 220ms; nada flutua com sombra.

## Shapes

Raio 0 em tudo. O selo da marca é o único círculo. Marcadores dos gráficos são quadrados de 7px.

## Components

- **Placa:** face branca, contorno Linha, cabeçalho grafite de 52px com quadrado Céu GA de 12px antes do título.
- **Botão primário:** fundo Ação, 48px, 13px/700 caixa alta, ícone de seta à direita quando avança.
- **Botão:** placa com contorno Linha forte, 40px; hover escurece o contorno para Grafite.
- **Campo:** 42px, contorno Linha forte; foco = contorno Ação + 1px interno (sem mudar a medida). Preenchido pelo OCR = fundo Ação-tinta e contorno Céu por 2,5s.
- **Seletor de bitola (signature):** seis etiquetas de amarrado com "Ø mm" em mono e o número em Archivo 800; a selecionada fica inteira Céu GA. `role=radiogroup`, setas do teclado.
- **Laudo (signature):** faixa de três critérios (LE ≥ 600, LR/LE ≥ 1,05, alongamento ≥ 5%) que acendem verde ou vermelho, e duas placas de veredito; a ativa enche de verde ou vermelho. Calculado, ajustável à mão.
- **Faixa do turno:** indicadores com marcador quadrado na cor do significado; relógio em mono; ao zerar, a área do relógio fica vermelha.
- **Alarme da ronda:** diálogo com faixa zebrada âmbar/grafite no topo e na base. Esc = adiar 10 min.
- **Aviso (toast):** placa grafite com ícone; erro em vermelho com `role=alert`.
- **Ícones:** desenhados em SVG, traço 2px, pontas retas. Nada de emoji.

## Do's and Don'ts

### Do:
- **Do** usar Céu GA como superfície e Ação (#0a64a8) como texto e botão azul.
- **Do** colocar todo valor medido em mono tabular, alinhado à direita em tabela.
- **Do** referenciar tokens (`var(--…)`) inclusive dentro de SVG, via `style`.
- **Do** escapar todo dado vindo da planilha antes de pôr no HTML.
- **Do** só confirmar gravação quando a planilha confirmar.

### Don't:
- **Don't** usar nomes, faixas ou elementos de identidade de outras marcas.
- **Don't** usar verde, vermelho ou âmbar fora de aprovado, reprovado e atenção.
- **Don't** pôr texto azul-céu ou âmbar puro sobre branco.
- **Don't** usar sombra, gradiente decorativo ou canto arredondado.
- **Don't** usar a faixa zebrada fora do alarme.
- **Don't** usar texto funcional abaixo de 11px.
