<!-- ELUCENIA technical documentation · indice-prognostico-de-nottingham · es · no clinical/professional/rights approval -->

# Índice pronóstico de Nottingham (NPI)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/indice-prognostico-de-nottingham)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Diámetro mayor del tumor invasivo (anatomía patológica)

`tam`

cm · intervalo: 0,1–20

### Ganglios linfáticos axilares

`lnd`

- `1` — Negativos
- `2` — 1 a 3 positivos
- `3` — 4 o más positivos

### Grado histológico (Nottingham/Elston-Ellis)

`grau`

- `1` — Grado 1
- `2` — Grado 2
- `3` — Grado 3

## Edición del método

NPI/Haybittle 1982/Galea 1992: 0,2 tamaño cm+estadio ganglionar 1–3+grado 1–3

## Fórmula documentada

NPI = 0,2 × tamaño (cm) + estadio ganglionar (1–3) + grado histológico (1–3).

Estadio ganglionar: 1=sin afectados; 2=1–3 ganglios; 3=4 o más (el original también incluye ápice axilar o mamaria interna).

## Límites y población

El NPI relaciona las características anatomopatológicas del cáncer primario de mama con el pronóstico. La suma requiere estadio ganglionar y grado correctamente definidos; no determina el tratamiento actual ni garantiza la supervivencia individual. La fórmula, los grupos y las tasas deben corresponder a la edición y la población utilizadas.

## Referencias

- [Haybittle JL et al. A prognostic index in primary breast cancer. Br J Cancer, 1982.](https://doi.org/10.1038/bjc.1982.62)

- [Galea MH et al. The Nottingham prognostic index in primary breast cancer. Breast Cancer Res Treat, 1992.](https://doi.org/10.1007/BF01840834)

- [Blamey RW et al. Survival of invasive breast cancer according to the Nottingham Prognostic Index in cases diagnosed in 1990-1999. Eur J Cancer, 2007.](https://doi.org/10.1016/j.ejca.2007.01.016)

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
