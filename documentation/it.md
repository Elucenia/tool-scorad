<!-- ELUCENIA technical documentation · scorad · it · no clinical/professional/rights approval -->

# SCORAD

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/scorad)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Estensione (A): superficie interessata secondo la regola del nove

`area`

% · intervallo: 0–100

### Eritema

`eritema`

- `0` — 0 assente
- `1` — 1 lieve
- `2` — 2 moderato
- `3` — 3 intenso

### Edema/papule

`edema`

- `0` — 0 assente
- `1` — 1 lieve
- `2` — 2 moderato
- `3` — 3 intenso

### Essudazione/croste

`exsudacao`

- `0` — 0 assente
- `1` — 1 lieve
- `2` — 2 moderato
- `3` — 3 intenso

### Escoriazione

`escoriacao`

- `0` — 0 assente
- `1` — 1 lieve
- `2` — 2 moderato
- `3` — 3 intenso

### Lichenificazione

`liquen`

- `0` — 0 assente
- `1` — 1 lieve
- `2` — 2 moderato
- `3` — 3 intenso

### Xerosi (sulla cute non lesionata)

`xerose`

- `0` — 0 assente
- `1` — 1 lieve
- `2` — 2 moderato
- `3` — 3 intenso

### Prurito negli ultimi 3 giorni (da 0 a 10)

`prurido`

intervallo: 0–10

### Perdita di sonno negli ultimi 3 giorni (da 0 a 10)

`sono`

intervallo: 0–10

## Edizione del metodo

SCORAD/ETFAD 1993: estensione/5+3,5 intensità+sintomi; oggettivo senza C; soglie Oranje 2007

## Formula documentata

SCORAD = A/5 + 7B/2 + C; A = estensione (0–100%), B = somma di 6 intensità (0–18), C = prurito + perdita sonno (0–20). Massimo: 103.

SCORAD oggettivo = A/5 + 7B/2 (Massimo: 83).

## Limiti e popolazione

Lo SCORAD misura la gravità della dermatite atopica e dipende dalla valutazione di segni, estensione e sintomi soggettivi. Lo sviluppo originale ha incluso valutatori formati e non stabilisce la diagnosi della malattia dal totale. SCORAD obiettivo, indice completo e soglie successive richiedono definizioni e fonti proprie.

## Riferimenti

- [European Task Force on Atopic Dermatitis. Severity scoring of atopic dermatitis: the SCORAD index. Dermatology, 1993.](https://doi.org/10.1159/000247298)

- [Kunz B et al. Clinical validation and guidelines for the SCORAD index: consensus report of the European Task Force on Atopic Dermatitis. Dermatology, 1997.](https://doi.org/10.1159/000245677)

- [Oranje AP et al. Practical issues on interpretation of scoring atopic dermatitis: the SCORAD index, objective SCORAD and the three-item severity score. Br J Dermatol, 2007.](https://doi.org/10.1111/j.1365-2133.2007.08112.x)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
