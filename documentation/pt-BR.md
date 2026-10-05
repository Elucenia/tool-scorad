<!-- ELUCENIA technical documentation · scorad · pt-BR · no clinical/professional/rights approval -->

# SCORAD

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/scorad)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Extensão (A): superfície acometida pela regra dos nove

`area`

% · intervalo: 0–100

### Eritema

`eritema`

- `0` — 0 ausente
- `1` — 1 leve
- `2` — 2 moderado
- `3` — 3 intenso

### Edema/papulação

`edema`

- `0` — 0 ausente
- `1` — 1 leve
- `2` — 2 moderado
- `3` — 3 intenso

### Exsudação/crostas

`exsudacao`

- `0` — 0 ausente
- `1` — 1 leve
- `2` — 2 moderado
- `3` — 3 intenso

### Escoriação

`escoriacao`

- `0` — 0 ausente
- `1` — 1 leve
- `2` — 2 moderado
- `3` — 3 intenso

### Liquenificação

`liquen`

- `0` — 0 ausente
- `1` — 1 leve
- `2` — 2 moderado
- `3` — 3 intenso

### Xerose (em pele não lesionada)

`xerose`

- `0` — 0 ausente
- `1` — 1 leve
- `2` — 2 moderado
- `3` — 3 intenso

### Prurido nos últimos 3 dias (0 a 10)

`prurido`

intervalo: 0–10

### Perda de sono nos últimos 3 dias (0 a 10)

`sono`

intervalo: 0–10

## Edição do método

SCORAD/ETFAD 1993:extensão/5+3,5 intensidade+sintomas; objective SCORADsem C; limiares Oranje 2007

## Fórmula documentada

SCORAD = A/5 + 7B/2 + C, em que A = extensão (0 a 100%), B = soma das 6 intensidades (0 a 18), C = prurido + perda de sono (0 a 20). Máximo: 103.

SCORAD objetivo = A/5 + 7B/2 (máximo 83).

## Limites e população

SCORAD mede gravidade de dermatite atópica e depende da avaliação dos sinais, extensão e sintomas subjetivos. O desenvolvimento original incluiu avaliadores treinados e não estabelece diagnóstico da doença pelo total. SCORAD objetivo, índice completo e cortes posteriores exigem suas próprias definições e fontes.

## Referências

- [European Task Force on Atopic Dermatitis. Severity scoring of atopic dermatitis: the SCORAD index. Dermatology, 1993.](https://doi.org/10.1159/000247298)

- [Kunz B et al. Clinical validation and guidelines for the SCORAD index: consensus report of the European Task Force on Atopic Dermatitis. Dermatology, 1997.](https://doi.org/10.1159/000245677)

- [Oranje AP et al. Practical issues on interpretation of scoring atopic dermatitis: the SCORAD index, objective SCORAD and the three-item severity score. Br J Dermatol, 2007.](https://doi.org/10.1111/j.1365-2133.2007.08112.x)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
