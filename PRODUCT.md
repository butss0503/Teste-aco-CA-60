# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Operador(es) do laboratório de ensaio de tração da Grande Aço. Lançam ensaios de vergalhão CA-60 a partir do laudo PDF da máquina, conferem o histórico da planilha, respondem à ronda de coleta de amostras a cada 1 hora e emitem o certificado do lote/OP. Usam o PC da bancada para lançar e o celular para consultar e acompanhar a ronda.

## Product Purpose

Registrar cada ensaio de tração na planilha Google da qualidade, já com o laudo ABNT NBR 7480 calculado, e transformar esse histórico em decisão: conformidade do turno, tendência de LE/LR por bitola e certificado do lote. Sucesso = nenhum ensaio digitado errado, nenhuma ronda perdida, nenhum certificado que diga algo que os dados não sustentam.

## Positioning

É a ferramenta do próprio laboratório da Grande Aço: lê o laudo PDF da máquina por OCR, aplica os limites CA-60 (LE ≥ 600 MPa, LR/LE ≥ 1,05, alongamento ≥ 5%, massa linear ±6%) e grava direto na planilha por bitola nominal (3,4 · 3,8 · 4,2 · 4,6 · 5,0 · 6,0).

## Operating Context

- Laudo PDF escaneado da máquina de tração (OCR com pdf.js + Tesseract no navegador).
- Planilha Google com uma aba por bitola, acessada via Google Apps Script (GET lista, POST insere/exclui). O laudo PDF vai para o Google Drive.
- Ronda de coleta de amostras na produção a cada 60 minutos, com alarme sonoro e visual.
- Tipos de ensaio: PROVA, CONTRA PROVA, TESTEMUNHO. Máquinas MAQ-01 a MAQ-05.
- Resumo diário enviado por WhatsApp; exportação CSV.

## Capabilities and Constraints

- Arquivo único `index.html`, HTML/CSS/JS sem build.
- O usuário pode editar o Apps Script (doPost) para devolver uma resposta real de gravação.
- Status do certificado do lote é decidido **pela média do lote**: APROVADO se LE médio ≥ 600 MPa, LR/LE médio ≥ 1,05 e alongamento médio ≥ 5%.
- Status de cada amostra continua sendo calculado pelas mesmas regras e pode ser ajustado à mão.

## Brand Commitments

- A identidade é da Grande Aço (logo em `Grandeaco.jpeg`: selo circular, "GA" + "GRANDE AÇO" em grotesca larga e pesada, "INDÚSTRIA DE AÇO" em mono, azul-céu e preto-grafite).
- Nenhum nome, faixa ou elemento de identidade de marca de terceiros.

## Evidence on Hand

- Logo: `Grandeaco.jpeg`.
- Dados reais vêm da planilha em tempo de execução; a página não inventa amostras.

## Product Principles

1. O laudo nunca afirma o que os dados não sustentam.
2. Gravação só é confirmada quando a planilha confirma.
3. Número de ensaio é o protagonista; todo o resto recua.
4. A ronda de 1h não pode passar despercebida.

## Accessibility & Inclusion

WCAG 2.1 AA: contraste de texto, controles com semântica (radiogroup, tabs, dialog), teclado e Esc em modais, leitura em celular.
