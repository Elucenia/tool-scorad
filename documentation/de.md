<!-- ELUCENIA technical documentation · scorad · de · no clinical/professional/rights approval -->

# SCORAD

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/scorad)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Ausdehnung (A): betroffene Fläche nach der Neunerregel

`area`

% · Bereich: 0–100

### Erythem

`eritema`

- `0` — 0 nicht vorhanden
- `1` — 1 leicht
- `2` — 2 mäßig
- `3` — 3 stark

### Ödem/Papeln

`edema`

- `0` — 0 nicht vorhanden
- `1` — 1 leicht
- `2` — 2 mäßig
- `3` — 3 stark

### Nässen/Krusten

`exsudacao`

- `0` — 0 nicht vorhanden
- `1` — 1 leicht
- `2` — 2 mäßig
- `3` — 3 stark

### Exkoriation

`escoriacao`

- `0` — 0 nicht vorhanden
- `1` — 1 leicht
- `2` — 2 mäßig
- `3` — 3 stark

### Lichenifikation

`liquen`

- `0` — 0 nicht vorhanden
- `1` — 1 leicht
- `2` — 2 mäßig
- `3` — 3 stark

### Xerosis (an nicht betroffener Haut)

`xerose`

- `0` — 0 nicht vorhanden
- `1` — 1 leicht
- `2` — 2 mäßig
- `3` — 3 stark

### Juckreiz in den letzten 3 Tagen (0 bis 10)

`prurido`

Bereich: 0–10

### Schlafverlust in den letzten 3 Tagen (0 bis 10)

`sono`

Bereich: 0–10

## Fassung der Methode

SCORAD/ETFAD 1993: Ausdehnung/5+3,5 Intensität+Symptome; objektiv ohne C; Oranje 2007-Grenzen

## Dokumentierte Formel

SCORAD = A/5 + 7B/2 + C; A = Ausdehnung (0–100%), B = Summe von 6 Intensitäten (0–18), C = Juckreiz + Schlafverlust (0–20). Maximum: 103.

Objektiver SCORAD = A/5 + 7B/2 (Maximum: 83).

## Grenzen und Population

SCORAD misst die Schwere atopischer Dermatitis und hängt von der Bewertung von Zeichen, Ausdehnung und subjektiven Symptomen ab. Die Originalentwicklung umfasste geschulte Beurteilende und stellt anhand der Summe keine Krankheitsdiagnose. Objektiver SCORAD, vollständiger Index und spätere Schwellen erfordern eigene Definitionen und Quellen.

## Referenzen

- [European Task Force on Atopic Dermatitis. Severity scoring of atopic dermatitis: the SCORAD index. Dermatology, 1993.](https://doi.org/10.1159/000247298)

- [Kunz B et al. Clinical validation and guidelines for the SCORAD index: consensus report of the European Task Force on Atopic Dermatitis. Dermatology, 1997.](https://doi.org/10.1159/000245677)

- [Oranje AP et al. Practical issues on interpretation of scoring atopic dermatitis: the SCORAD index, objective SCORAD and the three-item severity score. Br J Dermatol, 2007.](https://doi.org/10.1111/j.1365-2133.2007.08112.x)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Mittelgradige atopische Dermatitis (SCORAD 25 bis 50)

| Ergebnisdetails | |
| --- | --- |
| Objektiver SCORAD (ohne Symptome) | 21,5 (mäßig) |
| Ausdehnung (A/5) | 4,0 |
| Intensität (7B/2) | 17,5 |
| Symptome (C) | 6,0 |


### 2

Leichte atopische Dermatitis (SCORAD < 25)

| Ergebnisdetails | |
| --- | --- |
| Objektiver SCORAD (ohne Symptome) | 9,0 (leicht) |
| Ausdehnung (A/5) | 2,0 |
| Intensität (7B/2) | 7,0 |
| Symptome (C) | 2,0 |


### 3

Schwere atopische Dermatitis (SCORAD > 50)

| Ergebnisdetails | |
| --- | --- |
| Objektiver SCORAD (ohne Symptome) | 54,0 (schwer) |
| Ausdehnung (A/5) | 12,0 |
| Intensität (7B/2) | 42,0 |
| Symptome (C) | 15,0 |


### 4

Mittelgradige atopische Dermatitis (SCORAD 25 bis 50)

| Ergebnisdetails | |
| --- | --- |
| Objektiver SCORAD (ohne Symptome) | 19,0 (mäßig) |
| Ausdehnung (A/5) | 5,0 |
| Intensität (7B/2) | 14,0 |
| Symptome (C) | 6,0 |

