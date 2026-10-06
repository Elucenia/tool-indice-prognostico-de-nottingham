<!-- ELUCENIA technical documentation · indice-prognostico-de-nottingham · pt-BR · no clinical/professional/rights approval -->

# Índice Prognóstico de Nottingham (NPI)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/indice-prognostico-de-nottingham)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Maior diâmetro do tumor invasivo (patologia)

`tam`

cm · intervalo: 0,1–20

### Linfonodos axilares

`lnd`

- `1` — Negativos
- `2` — 1 a 3 positivos
- `3` — 4 ou mais positivos

### Grau histológico (Nottingham/Elston-Ellis)

`grau`

- `1` — Grau 1
- `2` — Grau 2
- `3` — Grau 3

## Edição do método

NPI/Haybittle 1982/Galea 1992:0,2 tamanhocm+estádio nodal 1–3+grau 1–3

## Fórmula documentada

NPI = 0,2 × tamanho (cm) + estágio linfonodal (1 a 3) + grau histológico (1 a 3).

Estágio linfonodal: 1 = sem linfonodos comprometidos; 2 = 1 a 3 linfonodos; 3 = 4 ou mais (na descrição original, também o comprometimento do ápice axilar ou da mamária interna).

## Limites e população

O NPI relaciona características anatomopatológicas do câncer primário de mama ao prognóstico. A soma requer estádio nodal e grau corretamente definidos; não determina tratamento atual nem garante sobrevivência individual. Fórmula, grupos e taxas devem corresponder à edição e à população utilizadas.

## Referências

- [Haybittle JL et al. A prognostic index in primary breast cancer. Br J Cancer, 1982.](https://doi.org/10.1038/bjc.1982.62)

- [Galea MH et al. The Nottingham prognostic index in primary breast cancer. Breast Cancer Res Treat, 1992.](https://doi.org/10.1007/BF01840834)

- [Blamey RW et al. Survival of invasive breast cancer according to the Nottingham Prognostic Index in cases diagnosed in 1990-1999. Eur J Cancer, 2007.](https://doi.org/10.1016/j.ejca.2007.01.016)

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

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Grupo prognóstico: Excelente (EPG)

| Detalhes do resultado | |
| --- | --- |
| Tamanho (0,2 × cm) | 0,30 |
| Linfonodos | 1 |
| Grau histológico | 1 |


### 2

Grupo prognóstico: Bom (GPG)

| Detalhes do resultado | |
| --- | --- |
| Tamanho (0,2 × cm) | 0,40 |
| Linfonodos | 1 |
| Grau histológico | 2 |


### 3

Grupo prognóstico: Moderado I (MPG I)

| Detalhes do resultado | |
| --- | --- |
| Tamanho (0,2 × cm) | 0,40 |
| Linfonodos | 2 |
| Grau histológico | 2 |


### 4

Grupo prognóstico: Ruim (PPG)

| Detalhes do resultado | |
| --- | --- |
| Tamanho (0,2 × cm) | 0,50 |
| Linfonodos | 2 |
| Grau histológico | 3 |


### 5

Grupo prognóstico: Muito ruim (VPG)

| Detalhes do resultado | |
| --- | --- |
| Tamanho (0,2 × cm) | 0,60 |
| Linfonodos | 3 |
| Grau histológico | 3 |

