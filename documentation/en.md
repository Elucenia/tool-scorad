<!-- ELUCENIA technical documentation · scorad · en · no clinical/professional/rights approval -->

# SCORAD

[conditions, sources and permissions](https://elucenia.org/en/tools/scorad)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Extent (A): affected surface area using the rule of nines

`area`

% · range: 0–100

### Erythema

`eritema`

- `0` — 0 absent
- `1` — 1 mild
- `2` — 2 moderate
- `3` — 3 intense

### Edema/papules

`edema`

- `0` — 0 absent
- `1` — 1 mild
- `2` — 2 moderate
- `3` — 3 intense

### Oozing/crusts

`exsudacao`

- `0` — 0 absent
- `1` — 1 mild
- `2` — 2 moderate
- `3` — 3 intense

### Excoriation

`escoriacao`

- `0` — 0 absent
- `1` — 1 mild
- `2` — 2 moderate
- `3` — 3 intense

### Lichenification

`liquen`

- `0` — 0 absent
- `1` — 1 mild
- `2` — 2 moderate
- `3` — 3 intense

### Xerosis (on unaffected skin)

`xerose`

- `0` — 0 absent
- `1` — 1 mild
- `2` — 2 moderate
- `3` — 3 intense

### Itching over the last 3 days (0 to 10)

`prurido`

range: 0–10

### Sleep loss over the last 3 days (0 to 10)

`sono`

range: 0–10

## Method edition

SCORAD/ETFAD 1993: extent/5+3.5 intensity+symptoms; objective SCORAD without C; Oranje 2007 thresholds

## Documented formula

SCORAD = A/5 + 7B/2 + C; A = extent (0–100%), B = sum of 6 intensities (0–18), C = itch + sleep loss (0–20). Maximum: 103.

Objective SCORAD = A/5 + 7B/2 (Maximum: 83).

## Limits and population

SCORAD measures atopic dermatitis severity and depends on assessment of signs, extent and subjective symptoms. The original development included trained raters and does not establish the disease diagnosis from the total. Objective SCORAD, the full index and later cutoffs require their own definitions and sources.

## References

- [European Task Force on Atopic Dermatitis. Severity scoring of atopic dermatitis: the SCORAD index. Dermatology, 1993.](https://doi.org/10.1159/000247298)

- [Kunz B et al. Clinical validation and guidelines for the SCORAD index: consensus report of the European Task Force on Atopic Dermatitis. Dermatology, 1997.](https://doi.org/10.1159/000245677)

- [Oranje AP et al. Practical issues on interpretation of scoring atopic dermatitis: the SCORAD index, objective SCORAD and the three-item severity score. Br J Dermatol, 2007.](https://doi.org/10.1111/j.1365-2133.2007.08112.x)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
