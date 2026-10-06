<!-- ELUCENIA technical documentation · indice-prognostico-de-nottingham · de · no clinical/professional/rights approval -->

# Nottingham-Prognoseindex (NPI)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/indice-prognostico-de-nottingham)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Größter Durchmesser des invasiven Tumors (Pathologie)

`tam`

cm · Bereich: 0,1–20

### Axilläre Lymphknoten

`lnd`

- `1` — Negativ
- `2` — 1 bis 3 positiv
- `3` — 4 oder mehr positiv

### Histologischer Grad (Nottingham/Elston-Ellis)

`grau`

- `1` — Grad 1
- `2` — Grad 2
- `3` — Grad 3

## Fassung der Methode

NPI/Haybittle 1982/Galea 1992: 0,2 Größe cm+Knotenstadium 1–3+Grad 1–3

## Dokumentierte Formel

NPI = 0,2 × Größe (cm) + Lymphknotenstadium (1–3) + histologischer Grad (1–3).

Lymphknotenstadium: 1=keine befallen; 2=1–3 Knoten; 3=4 oder mehr (original auch Axillaspitze oder interne Mammaria-Knoten).

## Grenzen und Population

NPI setzt histopathologische Merkmale des primären Mammakarzinoms mit der Prognose in Beziehung. Die Summe erfordert korrekt definiertes Lymphknotenstadium und Grading; sie bestimmt weder heutige Behandlung noch garantiert sie individuelles Überleben. Formel, Gruppen und Raten müssen zur verwendeten Ausgabe und Population passen.

## Referenzen

- [Haybittle JL et al. A prognostic index in primary breast cancer. Br J Cancer, 1982.](https://doi.org/10.1038/bjc.1982.62)

- [Galea MH et al. The Nottingham prognostic index in primary breast cancer. Breast Cancer Res Treat, 1992.](https://doi.org/10.1007/BF01840834)

- [Blamey RW et al. Survival of invasive breast cancer according to the Nottingham Prognostic Index in cases diagnosed in 1990-1999. Eur J Cancer, 2007.](https://doi.org/10.1016/j.ejca.2007.01.016)

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

Prognostische Gruppe: Exzellent (EPG)

| Ergebnisdetails | |
| --- | --- |
| Größe (0,2 × cm) | 0,30 |
| Lymphknoten | 1 |
| Histologischer Grad | 1 |


### 2

Prognosegruppe: Gut (GPG)

| Ergebnisdetails | |
| --- | --- |
| Größe (0,2 × cm) | 0,40 |
| Lymphknoten | 1 |
| Histologischer Grad | 2 |


### 3

Prognosegruppe: Mäßig I (MPG I)

| Ergebnisdetails | |
| --- | --- |
| Größe (0,2 × cm) | 0,40 |
| Lymphknoten | 2 |
| Histologischer Grad | 2 |


### 4

Prognosegruppe: Schlecht (PPG)

| Ergebnisdetails | |
| --- | --- |
| Größe (0,2 × cm) | 0,50 |
| Lymphknoten | 2 |
| Histologischer Grad | 3 |


### 5

Prognosegruppe: Sehr schlecht (VPG)

| Ergebnisdetails | |
| --- | --- |
| Größe (0,2 × cm) | 0,60 |
| Lymphknoten | 3 |
| Histologischer Grad | 3 |

