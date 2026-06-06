# ES MiniLight 广告架构存档 - 2026-06-06

存档时间：2026-06-06  
站点：Amazon ES  
产品/SKU：`ZULED01-4PC`  
数据来源：
- `广告日志_ACEEDU_ES_20260508-20260606.xlsx`
- `广告日志_ACEEDU_ES_20260606-20260606.xlsx`
- `广告搜索词_ACEEDU_ES_20260508-20260606.xlsx`

说明：
- 本存档按广告日志中“操作结果=成功”的最新操作还原。
- 日志能还原活动、广告组、投放词、匹配方式、当前竞价、状态、否定词/否定 ASIN。
- 日志未包含日预算、竞价策略、Placement 溢价、广告组合预算，因此这些项目需以后从后台截图或活动报表补充。
- 本轮新品期判断标准：核心精准词可接受 ACOS 约 35%-40%，但 ES 站 CPC 纪律仍要控制；核心词建议不超过 EUR 0.32-0.40，泛词/拓词建议不超过 EUR 0.18-0.30。

## 一、当前广告活动总览

| 广告活动 | 广告组 | 类型 | 当前状态判断 |
|---|---|---|---|
| `SP_ES_MiniLight_EX_MiniTorch_Profit` | `SP_ES_MiniLight_EX_MiniTorch_Profit` | 精确关键词 | 当前主力精准组，有出单词，需继续分层控价 |
| `SP_ES_MiniLight_PH_Harvest` | `SP_ES_MiniLight_PH_Harvest` | 词组关键词 | 拓词组，已暂停弱词并补否定，但仍有部分词组 bid 偏高 |
| `SP_ES_MiniLight_EX_LED_Recargable_Capped` | `SP_ES_MiniLight_EX_LED_Recargable_Capped` | 精确关键词 | 泛 LED/充电词组，已压低 `linterna led`，但其他泛词仍偏高 |
| `SP_ES_MiniLight_EX_Llavero_Core` | `SP_ES_MiniLight_EX_Llavero_Core` | 精确关键词 | 钥匙扣/磁吸方向，已整体降到 EUR 0.30；部分强功率和英文词仍建议再收 |
| `SP_ES_MiniLight_AUTO_Close` | `SP_ES_MiniLight_AUTO_Close` | 自动紧密 | 仅紧密匹配启用，bid 已降到 EUR 0.22；需补偏离否词 |
| `SP_ES_MiniLight_AUTO_同类 30商品` | `SP_ES_MiniLight_AUTO_同类` | 自动同类商品 | 仅同类商品启用，bid EUR 0.13；低价观察 |

## 二、`SP_ES_MiniLight_EX_MiniTorch_Profit`

主力精准组。搜索词报表中该组花费 EUR 4.12，11 点击，2 单，销售额 EUR 19.82，ACOS 20.79%。这是当前最健康的结构。

| 关键词 | 匹配 | 状态 | 当前竞价 | 当前判断 | 后续动作 |
|---|---|---|---:|---|---|
| `linterna mini` | 精确 | 已启动 | EUR 0.40 | 1 点击 1 单，ACOS 4.04%，好词 | 保留，不调整；若后续 CPC 过高再压到 EUR 0.35 |
| `mini linterna led` | 精确 | 已启动 | EUR 0.40 | 2 点击 1 单，ACOS 6.36%，好词 | 保留，不调整 |
| `mini linterna` | 精确 | 已启动 | EUR 0.32 | 2 点击 0 单，但相关 | 已降价到合理区间，观察 |
| `mini linterna led recargable` | 精确 | 已启动 | EUR 0.30 | 2 点击 0 单，相关 | 已降价，观察 |
| `linterna pequeña` | 精确 | 已启动 | EUR 0.22 | 4 点击 0 单，且 PH 中同方向差 | 已降价，观察；累计 8-10 点击仍 0 单再暂停 |
| `linterna led pequeña` | 精确 | 已启动 | EUR 0.40 | 日志显示仍偏高，搜索词暂无正反馈 | 建议降到 EUR 0.22-0.26 |
| `linterna led recargable pequeña` | 精确 | 已启动 | EUR 0.40 | 日志显示仍偏高，搜索词暂无正反馈 | 建议降到 EUR 0.22-0.26 |
| `mini linternas led alta potencia` | 精确 | 已启动 | EUR 0.40 | `alta potencia` 强功率预期，风险高 | 建议暂停，或降到 EUR 0.15-0.18 |

本组遗漏/待补：
- `linterna led pequeña` 尚未降价。
- `linterna led recargable pequeña` 尚未降价。
- `mini linternas led alta potencia` 尚未暂停或低价处理。

## 三、`SP_ES_MiniLight_PH_Harvest`

词组拓词组。搜索词报表中该组花费 EUR 10.23，22 点击，1 单，销售额 EUR 9.91，ACOS 103.23%。当前定位应为低价雷达，不承担放量。

### 词组投放当前状态

| 词组关键词 | 状态 | 当前竞价 | 当前判断 | 后续动作 |
|---|---|---:|---|---|
| `linterna pequeña` | 已暂停 | EUR 0.40 | 12 点击 0 单，已正确暂停 | 不恢复，至少等下一轮复盘 |
| `mini linterna` | 已启动 | EUR 0.43 | 9 点击 1 单，ACOS 42.18%，新品期可留 | 保留，暂不再升价 |
| `mini linterna led` | 已启动 | EUR 0.36 | 相关，已降价 | 保留观察 |
| `mini linterna led recargable` | 已启动 | EUR 0.36 | 相关，已降价 | 保留观察 |
| `mini linterna llavero` | 已启动 | EUR 0.28 | 钥匙扣长尾，低价合理 | 保留观察 |
| `linterna led llavero` | 已启动 | EUR 0.28 | 钥匙扣长尾，低价合理 | 保留观察 |
| `linterna llavero recargable` | 已启动 | EUR 0.28 | 钥匙扣长尾，低价合理 | 保留观察 |
| `linterna led pequeña` | 已启动 | EUR 0.46 | 仍偏高，曾跑出 EUR 0.62 CPC 无单 | 建议降到 EUR 0.25-0.30 |
| `linterna led recargable pequeña` | 已启动 | EUR 0.50 | 曾被建议价推到 EUR 0.95 后降回 EUR 0.50，但仍高 | 建议降到 EUR 0.25-0.30 |

### 已有否定关键词

当前 PH 组已有较多精准否定，用于避免和精准组抢流量及屏蔽弱词。重点新增的 2026-06-06 否词如下：

| 否定关键词 | 匹配 | 原因 |
|---|---|---|
| `linterna led pequeña alta potencia` | 精准否定 | 强功率预期，已花费无单 |
| `linterna pequeña potente` | 精准否定 | 6 点击 0 单，弱词 |
| `linternas pequeñas led potentes` | 精准否定 | 高 CPC，0 单 |
| `mini linterna led colores iman` | 精准否定 | `colores` 偏离产品 |
| `mini linterna de hombro` | 精准否定 | 肩灯意图偏离 |
| `mini linterna led deportistas` | 精准否定 | 运动场景偏散 |
| `linterna pequeña colgar` | 精准否定 | 挂灯意图偏离 |

PH 组已有基础精准否定还包括：
`keychain light`、`linterna led`、`linterna led llavero`、`linterna led pequeña`、`linterna led recargable`、`linterna led recargable pequeña`、`linterna llavero`、`linterna llavero potente`、`linterna llavero recargable`、`linterna mini`、`linterna pequeña`、`linterna recargable usb`、`linternas led alta potencia`、`linternas led alta potencia pequeña`、`linternas led alta potencia recargable`、`linternas llavero led alta potencia`、`linternas recargables`、`llavero led`、`llavero linterna led mini`、`llavero mini linterna led alta potencia recargable`、`mini linterna`、`mini linterna led`、`mini linterna led recargable`、`mini linterna led recargable usb llavero`、`mini linterna llavero`、`mini linternas led alta potencia`。

说明：PH 中有些词组关键词本身也被精准否定，例如 `mini linterna`。这通常表示“屏蔽完全相同搜索词，保留更长尾的词组扩展”，不是结构错误。

本组遗漏/待补：
- `linterna led pequeña` 当前 EUR 0.46，仍高，建议降到 EUR 0.25-0.30。
- `linterna led recargable pequeña` 当前 EUR 0.50，仍高，建议降到 EUR 0.25-0.30。

## 四、`SP_ES_MiniLight_EX_LED_Recargable_Capped`

泛 LED/充电词精准组。搜索词报表中已跑到 10 点击 0 单，需低价保守。

| 关键词 | 匹配 | 状态 | 当前竞价 | 当前判断 | 后续动作 |
|---|---|---|---:|---|---|
| `linterna led` | 精确 | 已启动 | EUR 0.15 | 已从 EUR 0.50 大幅降价，正确 | 保留低价捡漏 |
| `linterna led recargable` | 精确 | 已启动 | EUR 0.30 | 3 点击 0 单，仍偏高 | 建议降到 EUR 0.18-0.22 |
| `linterna recargable usb` | 精确 | 已启动 | EUR 0.30 | 泛充电词，仍偏高 | 建议降到 EUR 0.18-0.22 |
| `linternas led alta potencia recargable` | 精确 | 已启动 | EUR 0.30 | 强功率预期，不适合高价 | 建议暂停，或降到 EUR 0.12-0.15 |
| `llavero mini linterna led alta potencia recargable` | 精确 | 已暂停 | 未记录 | 已暂停，正确 | 不恢复 |

本组遗漏/待补：
- `linterna led recargable` 仍需降价。
- `linterna recargable usb` 仍需降价。
- `linternas led alta potencia recargable` 建议暂停或进一步降到极低价。

## 五、`SP_ES_MiniLight_EX_Llavero_Core`

钥匙扣方向精准组。2026-06-06 已整体降到 EUR 0.30，并新增 `mini linterna led con iman`。

| 关键词 | 匹配 | 状态 | 当前竞价 | 当前判断 | 后续动作 |
|---|---|---|---:|---|---|
| `mini linterna led con iman` | 精确 | 已启动 | EUR 0.30 | 已从 PH 出单词提精准；当前略高于原建议 EUR 0.22-0.26 | 可先观察 2-3 天；若无单降到 EUR 0.26 |
| `linterna llavero` | 精确 | 已启动 | EUR 0.30 | 已降价，合理 | 保留观察 |
| `mini linterna llavero` | 精确 | 已启动 | EUR 0.30 | 已降价，合理 | 保留观察 |
| `llavero linterna led mini` | 精确 | 已启动 | EUR 0.30 | 已降价，合理 | 保留观察 |
| `linterna led llavero` | 精确 | 已启动 | EUR 0.30 | 已降价，合理 | 保留观察 |
| `linterna llavero recargable` | 精确 | 已启动 | EUR 0.30 | 已降价，合理 | 保留观察 |
| `mini linterna led recargable usb llavero` | 精确 | 已启动 | EUR 0.30 | 已从 EUR 0.60 降价，正确 | 保留观察 |
| `linternas llavero led alta potencia` | 精确 | 已启动 | EUR 0.30 | `alta potencia` 风险仍在 | 建议暂停或降到 EUR 0.15-0.18 |
| `keychain light` | 精确 | 已启动 | EUR 0.30 | 英文词在 ES 站优先级低 | 建议暂停 |

结构备注：
- `mini linterna led con iman` 更像磁吸测试词，不是严格的 llavero 词。若后台方便，后续可单独拆成 `EX_Iman_Test`，方便看退货/评价和预算。

本组遗漏/待补：
- `keychain light` 尚未暂停。
- `linternas llavero led alta potencia` 尚未暂停或极低价。

## 六、`SP_ES_MiniLight_AUTO_Close`

自动紧密雷达组。

| 投放方式 | 状态 | 当前竞价 | 当前判断 | 后续动作 |
|---|---|---:|---|---|
| 自动-紧密匹配 | 已启动 | EUR 0.22 | 已从 EUR 0.30 降价，合理 | 保留低价跑 |
| 自动-宽泛匹配 | 已暂停 | EUR 0.30 | 已暂停 | 继续暂停 |
| 自动-关联匹配 | 已暂停 | EUR 0.30 | 已暂停 | 继续暂停 |
| 自动-同类商品 | 已暂停 | EUR 0.30 | 已暂停 | 继续暂停 |

已有否定关键词较多，覆盖主力精准词、钥匙扣词、强功率词等。

本组遗漏/待补：
- 建议新增精准否定：`400 luces led lámpara`
- 建议新增精准否定：`luz de emergencia`

## 七、`SP_ES_MiniLight_AUTO_同类 30商品`

同类商品自动投放组。

| 投放方式 | 状态 | 当前竞价 | 当前判断 | 后续动作 |
|---|---|---:|---|---|
| 自动-同类商品 | 已启动 | EUR 0.13 | 从 EUR 0.08 提到 EUR 0.13，仍属低价 | 保留观察 |
| 自动-紧密匹配 | 已暂停 | EUR 0.30 | 已暂停 | 继续暂停 |
| 自动-宽泛匹配 | 已暂停 | EUR 0.30 | 已暂停 | 继续暂停 |
| 自动-关联匹配 | 已暂停 | EUR 0.30 | 已暂停 | 继续暂停 |

已有否定 ASIN：
- `B0B8JCHNQM`
- `B0BRSTK9GV`
- `B0BRSTKFM9`
- `B0BRSVS895`
- `B0BZ5SFVJR`

备注：
- 当前 EUR 0.13 可以接受。若 3-5 天后仍无曝光，可小幅到 EUR 0.15；若有点击无单，则不再加价。

## 八、本轮调整完成度检查

已完成且正确：
- `PH_Harvest` 中 `linterna pequeña` 已暂停。
- `PH_Harvest` 已补 7 个关键否定精准。
- `PH_Harvest` 中 `mini linterna` 已降到 EUR 0.43。
- `mini linterna led con iman` 已提入精准。
- `EX_LED_Recargable_Capped` 中 `linterna led` 已降到 EUR 0.15。
- `EX_LED_Recargable_Capped` 中 `llavero mini linterna led alta potencia recargable` 已暂停。
- `EX_Llavero_Core` 大部分词已从 EUR 0.50-0.60 降到 EUR 0.30。
- `AUTO_Close` 紧密匹配已降到 EUR 0.22。
- `AUTO_同类 30商品` 同类商品 bid 已调整到 EUR 0.13。

仍建议补做：

| 优先级 | 对象 | 当前 | 建议 | 原因 |
|---|---|---:|---:|---|
| 高 | `PH_Harvest` / `linterna led recargable pequeña` | EUR 0.50 | EUR 0.25-0.30 | PH 拓词，不应高价跑；该方向暂无成交证据 |
| 高 | `PH_Harvest` / `linterna led pequeña` | EUR 0.46 | EUR 0.25-0.30 | 之前搜索词 CPC 高且无单 |
| 高 | `AUTO_Close` 否词 | 未见新增 | 否定 `400 luces led lámpara`、`luz de emergencia` | 搜索意图偏离 |
| 中 | `EX_LED_Recargable_Capped` / `linterna led recargable` | EUR 0.30 | EUR 0.18-0.22 | 3 点击 0 单，ES 利润线薄 |
| 中 | `EX_LED_Recargable_Capped` / `linterna recargable usb` | EUR 0.30 | EUR 0.18-0.22 | 泛充电词 |
| 中 | `EX_LED_Recargable_Capped` / `linternas led alta potencia recargable` | EUR 0.30 | 暂停或 EUR 0.12-0.15 | 强功率预期偏离 |
| 中 | `EX_MiniTorch_Profit` / `linterna led pequeña` | EUR 0.40 | EUR 0.22-0.26 | 暂无正反馈，竞价偏高 |
| 中 | `EX_MiniTorch_Profit` / `linterna led recargable pequeña` | EUR 0.40 | EUR 0.22-0.26 | 暂无正反馈，竞价偏高 |
| 中 | `EX_MiniTorch_Profit` / `mini linternas led alta potencia` | EUR 0.40 | 暂停或 EUR 0.15-0.18 | 强功率预期偏离 |
| 低 | `EX_Llavero_Core` / `keychain light` | EUR 0.30 | 暂停 | 英文词在 ES 站优先级低 |
| 低 | `EX_Llavero_Core` / `linternas llavero led alta potencia` | EUR 0.30 | 暂停或 EUR 0.15-0.18 | 强功率预期偏离 |

## 九、下轮复盘规则

建议再跑 3-5 天后复盘：

| 情况 | 动作 |
|---|---|
| 精准词 2 单且 ACOS <= 40% | 保留，可小幅加预算或维持 |
| 精准词 1 单且 ACOS <= 50% | 继续观察，不急放量 |
| 任意词 8-10 点击 0 单 | 降价或暂停 |
| PH 词组跑出新成交词 | 提精准，并在 PH 中视情况加精准否定 |
| AUTO 跑出偏离词 | 加精准否定 |
| `iman` 词出单但退货/差评变差 | 立即单独隔离或暂停 |

## 十、非本产品日志提示

2026-06-06 新日志中有 4 条“汽车遮阳伞”广告预算状态变化：
- `汽车遮阳伞-AU-非主推 紧密+宽泛-0.13`
- `汽车遮阳伞 新款-P/E-保护 12.30-14`
- `汽车遮阳伞-P/E-parasol coche 2.24-3 3.31仅P其余位置`

这些不属于 ES MiniLight 小灯架构，已从本存档中排除。
