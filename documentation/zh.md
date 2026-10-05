<!-- ELUCENIA technical documentation · scorad · zh · no clinical/professional/rights approval -->

# SCORAD

[条件、来源与许可](https://elucenia.org/zh/tools/scorad)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 范围（A）：按九分法计算的受累面积

`area`

% · 范围: 0–100

### 红斑

`eritema`

- `0` — 0 无
- `1` — 1 轻度
- `2` — 2 中度
- `3` — 3 重度

### 水肿/丘疹

`edema`

- `0` — 0 无
- `1` — 1 轻度
- `2` — 2 中度
- `3` — 3 重度

### 渗出/结痂

`exsudacao`

- `0` — 0 无
- `1` — 1 轻度
- `2` — 2 中度
- `3` — 3 重度

### 抓痕

`escoriacao`

- `0` — 0 无
- `1` — 1 轻度
- `2` — 2 中度
- `3` — 3 重度

### 苔藓样变

`liquen`

- `0` — 0 无
- `1` — 1 轻度
- `2` — 2 中度
- `3` — 3 重度

### 皮肤干燥（无病变皮肤）

`xerose`

- `0` — 0 无
- `1` — 1 轻度
- `2` — 2 中度
- `3` — 3 重度

### 过去 3 天瘙痒（0 至 10）

`prurido`

范围: 0–10

### 过去 3 天睡眠受影响程度（0 至 10）

`sono`

范围: 0–10

## 方法版本

SCORAD/ETFAD 1993：范围/5+3.5强度+症状；客观SCORAD无C；Oranje 2007阈值

## 已记录的公式

SCORAD = A/5 + 7B/2 + C; A = 范围 (0–100%), B = 6项强度之和 (0–18), C = 瘙痒+睡眠损失 (0–20). 最大： 103.

客观SCORAD = A/5 + 7B/2 (最大： 83).

## 限制与适用人群

SCORAD测量特应性皮炎严重程度，依赖体征、范围和主观症状的评估。原始开发包括受过培训的评估者，不能由总分确诊该疾病。客观SCORAD、完整指数和后续阈值需要各自的定义与来源。

## 参考文献

- [European Task Force on Atopic Dermatitis. Severity scoring of atopic dermatitis: the SCORAD index. Dermatology, 1993.](https://doi.org/10.1159/000247298)

- [Kunz B et al. Clinical validation and guidelines for the SCORAD index: consensus report of the European Task Force on Atopic Dermatitis. Dermatology, 1997.](https://doi.org/10.1159/000245677)

- [Oranje AP et al. Practical issues on interpretation of scoring atopic dermatitis: the SCORAD index, objective SCORAD and the three-item severity score. Br J Dermatol, 2007.](https://doi.org/10.1111/j.1365-2133.2007.08112.x)

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
