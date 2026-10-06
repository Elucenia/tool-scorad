<!-- ELUCENIA technical documentation · scorad · es · no clinical/professional/rights approval -->

# SCORAD

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/scorad)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Extensión (A): superficie afectada según la regla de los nueve

`area`

% · intervalo: 0–100

### Eritema

`eritema`

- `0` — 0 ausente
- `1` — 1 leve
- `2` — 2 moderado
- `3` — 3 intenso

### Edema/pápulas

`edema`

- `0` — 0 ausente
- `1` — 1 leve
- `2` — 2 moderado
- `3` — 3 intenso

### Exudación/costras

`exsudacao`

- `0` — 0 ausente
- `1` — 1 leve
- `2` — 2 moderado
- `3` — 3 intenso

### Excoriación

`escoriacao`

- `0` — 0 ausente
- `1` — 1 leve
- `2` — 2 moderado
- `3` — 3 intenso

### Liquenificación

`liquen`

- `0` — 0 ausente
- `1` — 1 leve
- `2` — 2 moderado
- `3` — 3 intenso

### Xerosis (en piel no lesionada)

`xerose`

- `0` — 0 ausente
- `1` — 1 leve
- `2` — 2 moderado
- `3` — 3 intenso

### Prurito en los últimos 3 días (de 0 a 10)

`prurido`

intervalo: 0–10

### Pérdida de sueño en los últimos 3 días (de 0 a 10)

`sono`

intervalo: 0–10

## Edición del método

SCORAD/ETFAD 1993: extensión/5+3,5 intensidad+síntomas; objetivo sin C; umbrales Oranje 2007

## Fórmula documentada

SCORAD = A/5 + 7B/2 + C; A = extensión (0–100%), B = suma de 6 intensidades (0–18), C = prurito + pérdida de sueño (0–20). Máximo: 103.

SCORAD objetivo = A/5 + 7B/2 (Máximo: 83).

## Límites y población

El SCORAD mide la gravedad de la dermatitis atópica y depende de la evaluación de signos, extensión y síntomas subjetivos. El desarrollo original incluyó evaluadores formados y no establece el diagnóstico de la enfermedad mediante el total. El SCORAD objetivo, el índice completo y los puntos de corte posteriores requieren sus propias definiciones y fuentes.

## Referencias

- [European Task Force on Atopic Dermatitis. Severity scoring of atopic dermatitis: the SCORAD index. Dermatology, 1993.](https://doi.org/10.1159/000247298)

- [Kunz B et al. Clinical validation and guidelines for the SCORAD index: consensus report of the European Task Force on Atopic Dermatitis. Dermatology, 1997.](https://doi.org/10.1159/000245677)

- [Oranje AP et al. Practical issues on interpretation of scoring atopic dermatitis: the SCORAD index, objective SCORAD and the three-item severity score. Br J Dermatol, 2007.](https://doi.org/10.1111/j.1365-2133.2007.08112.x)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

Dermatitis atópica moderada (SCORAD 25 a 50)

| Detalles del resultado | |
| --- | --- |
| SCORAD objetivo (sin síntomas) | 21,5 (moderada) |
| Extensión (A/5) | 4,0 |
| Intensidad (7B/2) | 17,5 |
| Síntomas (C) | 6,0 |


### 2

Dermatitis atópica leve (SCORAD < 25)

| Detalles del resultado | |
| --- | --- |
| SCORAD objetivo (sin síntomas) | 9,0 (leve) |
| Extensión (A/5) | 2,0 |
| Intensidad (7B/2) | 7,0 |
| Síntomas (C) | 2,0 |


### 3

Dermatitis atópica grave (SCORAD > 50)

| Detalles del resultado | |
| --- | --- |
| SCORAD objetivo (sin síntomas) | 54,0 (grave) |
| Extensión (A/5) | 12,0 |
| Intensidad (7B/2) | 42,0 |
| Síntomas (C) | 15,0 |


### 4

Dermatitis atópica moderada (SCORAD 25 a 50)

| Detalles del resultado | |
| --- | --- |
| SCORAD objetivo (sin síntomas) | 19,0 (moderada) |
| Extensión (A/5) | 5,0 |
| Intensidad (7B/2) | 14,0 |
| Síntomas (C) | 6,0 |

