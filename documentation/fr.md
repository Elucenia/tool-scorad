<!-- ELUCENIA technical documentation · scorad · fr · no clinical/professional/rights approval -->

# SCORAD

[conditions, sources et autorisations](https://elucenia.org/fr/outils/scorad)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Étendue (A) : surface atteinte selon la règle des neuf

`area`

% · intervalle: 0–100

### Érythème

`eritema`

- `0` — 0 absent
- `1` — 1 léger
- `2` — 2 modéré
- `3` — 3 intense

### Œdème/papules

`edema`

- `0` — 0 absent
- `1` — 1 léger
- `2` — 2 modéré
- `3` — 3 intense

### Suintement/croûtes

`exsudacao`

- `0` — 0 absent
- `1` — 1 léger
- `2` — 2 modéré
- `3` — 3 intense

### Excoriation

`escoriacao`

- `0` — 0 absent
- `1` — 1 léger
- `2` — 2 modéré
- `3` — 3 intense

### Lichénification

`liquen`

- `0` — 0 absent
- `1` — 1 léger
- `2` — 2 modéré
- `3` — 3 intense

### Xérose (sur peau non lésée)

`xerose`

- `0` — 0 absent
- `1` — 1 léger
- `2` — 2 modéré
- `3` — 3 intense

### Prurit au cours des 3 derniers jours (0 à 10)

`prurido`

intervalle: 0–10

### Perte de sommeil au cours des 3 derniers jours (0 à 10)

`sono`

intervalle: 0–10

## Édition de la méthode

SCORAD/ETFAD 1993 : étendue/5+3,5 intensité+symptômes ; objectif sans C ; seuils Oranje 2007

## Formule documentée

SCORAD = A/5 + 7B/2 + C; A = étendue (0–100%), B = somme de 6 intensités (0–18), C = prurit + perte de sommeil (0–20). Maximum : 103.

SCORAD objectif = A/5 + 7B/2 (Maximum : 83).

## Limites et population

Le SCORAD mesure la sévérité de la dermatite atopique et dépend de l’évaluation des signes, de l’étendue et des symptômes subjectifs. Le développement original impliquait des évaluateurs formés et n’établit pas un diagnostic par le total. Le SCORAD objectif, l’indice complet et les seuils ultérieurs exigent leurs propres définitions et sources.

## Références

- [European Task Force on Atopic Dermatitis. Severity scoring of atopic dermatitis: the SCORAD index. Dermatology, 1993.](https://doi.org/10.1159/000247298)

- [Kunz B et al. Clinical validation and guidelines for the SCORAD index: consensus report of the European Task Force on Atopic Dermatitis. Dermatology, 1997.](https://doi.org/10.1159/000245677)

- [Oranje AP et al. Practical issues on interpretation of scoring atopic dermatitis: the SCORAD index, objective SCORAD and the three-item severity score. Br J Dermatol, 2007.](https://doi.org/10.1111/j.1365-2133.2007.08112.x)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Dermatite atopique modérée (SCORAD 25 à 50)

| Détails du résultat | |
| --- | --- |
| SCORAD objectif (sans symptômes) | 21,5 (modérée) |
| Extension (A/5) | 4,0 |
| Intensité (7B/2) | 17,5 |
| Symptômes (C) | 6,0 |


### 2

Dermatite atopique légère (SCORAD < 25)

| Détails du résultat | |
| --- | --- |
| SCORAD objectif (sans symptômes) | 9,0 (légère) |
| Extension (A/5) | 2,0 |
| Intensité (7B/2) | 7,0 |
| Symptômes (C) | 2,0 |


### 3

Dermatite atopique sévère (SCORAD > 50)

| Détails du résultat | |
| --- | --- |
| SCORAD objectif (sans symptômes) | 54,0 (sévère) |
| Extension (A/5) | 12,0 |
| Intensité (7B/2) | 42,0 |
| Symptômes (C) | 15,0 |


### 4

Dermatite atopique modérée (SCORAD 25 à 50)

| Détails du résultat | |
| --- | --- |
| SCORAD objectif (sans symptômes) | 19,0 (modérée) |
| Extension (A/5) | 5,0 |
| Intensité (7B/2) | 14,0 |
| Symptômes (C) | 6,0 |

