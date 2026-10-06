<!-- ELUCENIA technical documentation · indice-prognostico-de-nottingham · it · no clinical/professional/rights approval -->

# Indice prognostico di Nottingham (NPI)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/indice-prognostico-de-nottingham)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Diametro maggiore del tumore invasivo (anatomia patologica)

`tam`

cm · intervallo: 0,1–20

### Linfonodi ascellari

`lnd`

- `1` — Negativi
- `2` — Da 1 a 3 positivi
- `3` — 4 o più positivi

### Grado istologico (Nottingham/Elston-Ellis)

`grau`

- `1` — Grado 1
- `2` — Grado 2
- `3` — Grado 3

## Edizione del metodo

NPI/Haybittle 1982/Galea 1992: 0,2 dimensione cm+stadio nodale 1–3+grado 1–3

## Formula documentata

NPI = 0,2 × dimensione (cm) + stadio linfonodale (1–3) + grado istologico (1–3).

Stadio linfonodale: 1=nessuno coinvolto; 2=1–3 linfonodi; 3=4 o più (nell’originale anche apice ascellare o mammaria interna).

## Limiti e popolazione

L’NPI mette in relazione le caratteristiche anatomopatologiche del carcinoma mammario primario con la prognosi. La somma richiede stadio linfonodale e grado correttamente definiti; non determina il trattamento attuale né garantisce la sopravvivenza individuale. Formula, gruppi e tassi devono corrispondere all’edizione e alla popolazione utilizzate.

## Riferimenti

- [Haybittle JL et al. A prognostic index in primary breast cancer. Br J Cancer, 1982.](https://doi.org/10.1038/bjc.1982.62)

- [Galea MH et al. The Nottingham prognostic index in primary breast cancer. Breast Cancer Res Treat, 1992.](https://doi.org/10.1007/BF01840834)

- [Blamey RW et al. Survival of invasive breast cancer according to the Nottingham Prognostic Index in cases diagnosed in 1990-1999. Eur J Cancer, 2007.](https://doi.org/10.1016/j.ejca.2007.01.016)

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

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Gruppo prognostico: Eccellente (EPG)

| Dettagli del risultato | |
| --- | --- |
| Dimensione (0,2 × cm) | 0,30 |
| Linfonodi | 1 |
| Grado istologico | 1 |


### 2

Gruppo prognostico: Buono (GPG)

| Dettagli del risultato | |
| --- | --- |
| Dimensione (0,2 × cm) | 0,40 |
| Linfonodi | 1 |
| Grado istologico | 2 |


### 3

Gruppo prognostico: Moderato I (MPG I)

| Dettagli del risultato | |
| --- | --- |
| Dimensione (0,2 × cm) | 0,40 |
| Linfonodi | 2 |
| Grado istologico | 2 |


### 4

Gruppo prognostico: Scarso (PPG)

| Dettagli del risultato | |
| --- | --- |
| Dimensione (0,2 × cm) | 0,50 |
| Linfonodi | 2 |
| Grado istologico | 3 |


### 5

Gruppo prognostico: Molto scarso (VPG)

| Dettagli del risultato | |
| --- | --- |
| Dimensione (0,2 × cm) | 0,60 |
| Linfonodi | 3 |
| Grado istologico | 3 |

