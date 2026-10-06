<!-- ELUCENIA technical documentation · indice-prognostico-de-nottingham · zh · no clinical/professional/rights approval -->

# Nottingham 预后指数（NPI）

[条件、来源与许可](https://elucenia.org/zh/tools/indice-prognostico-de-nottingham)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 浸润性肿瘤最大直径（病理）

`tam`

cm · 范围: 0.1–20

### 腋窝淋巴结

`lnd`

- `1` — 阴性
- `2` — 1至3个阳性
- `3` — 4个或以上阳性

### 组织学分级（Nottingham/Elston-Ellis）

`grau`

- `1` — 级别 1
- `2` — 级别 2
- `3` — 级别 3

## 方法版本

NPI/Haybittle 1982/Galea 1992：0.2大小cm+淋巴结期1–3+级别1–3

## 已记录的公式

NPI=0.2×大小（cm）+淋巴结分期（1–3）+组织学分级（1–3）。

淋巴结分期：1=无受累；2=1–3枚；3=4枚及以上（原描述也包括腋窝顶端或内乳淋巴结受累）。

## 限制与适用人群

NPI将原发性乳腺癌的病理特征与预后关联。求和需要正确界定淋巴结分期及组织学等级；不能确定当前治疗，也不能保证个体生存。公式、分组及发生率须与所用版本和人群相符。

## 参考文献

- [Haybittle JL et al. A prognostic index in primary breast cancer. Br J Cancer, 1982.](https://doi.org/10.1038/bjc.1982.62)

- [Galea MH et al. The Nottingham prognostic index in primary breast cancer. Breast Cancer Res Treat, 1992.](https://doi.org/10.1007/BF01840834)

- [Blamey RW et al. Survival of invasive breast cancer according to the Nottingham Prognostic Index in cases diagnosed in 1990-1999. Eur J Cancer, 2007.](https://doi.org/10.1016/j.ejca.2007.01.016)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

预后组：极佳（EPG）

| 结果详情 | |
| --- | --- |
| 大小（0.2 × cm） | 0.30 |
| 淋巴结 | 1 |
| 组织学分级 | 1 |


### 2

预后组：良好（GPG）

| 结果详情 | |
| --- | --- |
| 大小（0.2 × cm） | 0.40 |
| 淋巴结 | 1 |
| 组织学分级 | 2 |


### 3

预后组：中等 I（MPG I）

| 结果详情 | |
| --- | --- |
| 大小（0.2 × cm） | 0.40 |
| 淋巴结 | 2 |
| 组织学分级 | 2 |


### 4

预后组：差（PPG）

| 结果详情 | |
| --- | --- |
| 大小（0.2 × cm） | 0.50 |
| 淋巴结 | 2 |
| 组织学分级 | 3 |


### 5

预后组：很差（VPG）

| 结果详情 | |
| --- | --- |
| 大小（0.2 × cm） | 0.60 |
| 淋巴结 | 3 |
| 组织学分级 | 3 |

