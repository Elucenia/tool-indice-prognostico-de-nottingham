<!-- ELUCENIA technical documentation · indice-prognostico-de-nottingham · en · no clinical/professional/rights approval -->

# Nottingham Prognostic Index (NPI)

[conditions, sources and permissions](https://elucenia.org/en/tools/indice-prognostico-de-nottingham)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Largest invasive tumor diameter (pathology)

`tam`

cm · range: 0.1–20

### Axillary lymph nodes

`lnd`

- `1` — Negative
- `2` — 1 to 3 positive
- `3` — 4 or more positive

### Histological grade (Nottingham/Elston-Ellis)

`grau`

- `1` — Grade 1
- `2` — Grade 2
- `3` — Grade 3

## Method edition

NPI/Haybittle 1982/Galea 1992: 0.2 size cm+nodal stage 1–3+grade 1–3

## Documented formula

NPI = 0.2 × size (cm) + nodal stage (1–3) + histological grade (1–3).

Nodal stage: 1=no involved nodes; 2=1–3 nodes; 3=4 or more (the original description also includes axillary-apex or internal mammary involvement).

## Limits and population

NPI relates pathological features of primary breast cancer to prognosis. The total requires correctly defined nodal stage and grade; it does not determine current treatment or guarantee individual survival. The formula, groups and rates must match the edition and population used.

## References

- [Haybittle JL et al. A prognostic index in primary breast cancer. Br J Cancer, 1982.](https://doi.org/10.1038/bjc.1982.62)

- [Galea MH et al. The Nottingham prognostic index in primary breast cancer. Breast Cancer Res Treat, 1992.](https://doi.org/10.1007/BF01840834)

- [Blamey RW et al. Survival of invasive breast cancer according to the Nottingham Prognostic Index in cases diagnosed in 1990-1999. Eur J Cancer, 2007.](https://doi.org/10.1016/j.ejca.2007.01.016)

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
