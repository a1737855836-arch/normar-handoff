# COFFEE-003 咖啡 Normar 标签树（定稿）

任务编号：COFFEE-003  
执行日期：2026-10-23（Asia/Shanghai）  
状态：**已定稿 + 糖浆一级补丁**（阿拿 2026-10-24：糖浆升一级，与经典/特调平级）  
产品约束：卡片仍走 Normar 详情模板；咖啡豆是知识点卡，**不**做成独立百科站

卡类型约定：
- **配方卡**：有配料表 + 杯型 + 步骤（可冲泡/可点单的一杯）
- **知识点卡**：选题讲解（仍用详情模板：标题、标签、要点条目当「配料/要点」、步骤当「怎么理解/怎么做检查」），无强制毫升配方

---

## 一级 1 · 咖啡豆 Coffee Beans

| 二级 id | 显示名 English 中文 | 默认卡类型 | 示例条目（首版可少） | 备注 |
| --- | --- | --- | --- | --- |
| `bean-select` | Selection选取 | 知识点卡 | 阿拉比卡/罗布斯塔；产地与海拔；瑕疵豆识别 | 不做产地百科长文，一条一主题 |
| `bean-roast` | Roast烘焙 | 知识点卡 | 烘焙度谱；烘焙曲线入门；养豆窗口 | 工艺作参数写进正文/步骤句 |
| `bean-process` | Process发酵处理 | 知识点卡 | 水洗/日晒/蜜处理/湿刨；厌氧作概念卡；CO₂/酵母进阶 | 对外写「发酵处理」；id 仍 `bean-process` |
| `bean-storage` | Storage储存 | 知识点卡 | 密封/避光/温度；开封后建议 | 短卡 |

一级本身不挂配方卡。一级 id：`coffee-beans`，显示名 `Coffee Beans咖啡豆`。

---

## 一级 2 · 经典咖啡 Classic Coffee

| 二级 id | 显示名 English 中文 | 默认卡类型 | 挂载的 19 杯骨架（若有） | 备注 |
| --- | --- | --- | --- | --- |
| `classic-espresso` | Espresso浓缩 | 配方卡 | espresso, ristretto, lungo, americano | Espresso 默认约 1:2 重量；体积仅脚注 |
| `classic-milk` | Milk奶咖 | 配方卡 | macchiato, cortado, flat-white, cappuccino, latte, piccolo, mocha | Mocha 归经典奶咖 |
| `classic-filter` | Filter过滤 | 配方卡 | pour-over-v60, french-press, aeropress, cold-brew, batch-brew | **不过**升独立一级；挂在经典咖啡下 |

一级 id：`classic-coffee`，显示名 **`Classic Coffee经典咖啡`**（原「意式经典 / Classic Espresso Drinks」已废止）。

Siphon / Turkish：延后，不进树。

已砍（首版不上树）：`classic-glass` 杯型与出品。

---

## 一级 3 · 现代特调咖啡 Modern Signature

| 二级 id | 显示名 English 中文 | 默认卡类型 | 挂载 | 备注 |
| --- | --- | --- | --- | --- |
| `modern-espresso-twist` | Espresso Twist意式变奏 | 配方卡 | affogato, espresso-tonic（骨架）；COFFEE-004 主表同 hint | notes 标「特调」 |
| `modern-milk-twist` | Milk Twist奶咖变奏 | 配方卡 | dirty（骨架）；COFFEE-004 主表同 hint | Nitro=`cardType=knowledge` 非配方；Con Panna=`optional` 备选 |

一级 id：`modern-signature`，显示名 `Modern Signature现代特调`。

已砍（首版不上树）：`modern-seasonal` 季节/门店空壳、`modern-technique` 手法笔记（拉花/奶泡当素材库，不进标签树）。

---


---

## 一级 4 · 糖浆 Syrups

| 二级 id | 显示名 English 中文 | 默认卡类型 | 挂载示例 | 备注 |
| --- | --- | --- | --- | --- |
| `syrup-base` | Base基础糖浆 | 配方卡（制备） | 简单糖浆、焦糖酱、巧克力酱、香草糖浆 | 特调里「自制××糖浆」拆成独立卡时可挂这里 |
| `syrup-fruit` | Fruit果味糖浆 | 配方卡（制备） | 草莓、覆盆子、橙子皮等 | 材料+做法齐全再上树 |
| `syrup-spice` | Spice香料糖浆 | 配方卡（制备） | 南瓜香料、肉桂、太妃/咸焦糖向 | 与现代特调交叉引用，不重复整杯配方 |
| `syrup-floral` | Floral花香糖浆 | 配方卡（制备） | 薰衣草、玫瑰、蜂蜜薰衣草 | 同上 |

一级 id：`coffee-syrups`，显示名 `Syrups糖浆`。

约定：
- 卡类型按**制备配方卡**（配料 + 步骤），不是知识点百科。
- 特调正文可写「见糖浆库 · 南瓜香料糖浆」；糖浆卡不写整杯拿铁步骤。
- 与乙醇 Normar 已删的「材料制备」标签**无关**；本类仅咖啡因实验日志。


## 与旧方案关系

| 旧 | 新树 | 处理 |
| --- | --- | --- |
| 意式 / 奶咖 / 过滤 扁平三类（`label-brew-*`） | 一级：咖啡豆 / **经典咖啡** / 现代特调；经典下再分浓缩/奶咖/过滤 | **替换，不并存**；旧三类 id 废弃 |
| 「意式经典」作一级显示名 | **改名**「经典咖啡 Classic Coffee」 | 阿拿方案② |
| 过滤升一级「过滤咖啡」 | **不采用**；过滤作经典咖啡二级 | 阿拿拍板 |
| 特调挂意式/奶咖扁平类 | 一级「现代特调」+ 二级变奏 | 按阿拿新口径 |
| 杯型出品 / 手法笔记 / 季节空壳 | — | **首版砍** |

---

## 决策记录（已拍 · 原「需决策」关闭）

1. **过滤**：不升一级。挂「经典咖啡」二级 `classic-filter`。（阿拿 2026-10-23 方案②）
2. **classic-glass / modern-technique / modern-seasonal**：首版砍掉，不留空壳。（小严）
3. **bean-process 对外用词**：「发酵处理」；对内 id 仍 `bean-process`。（小严）
4. **旧扁平三类**：替换不并存。（小严）
5. **现代特调**：Dirty / Affogato / Tonic 可过；Nitro=知识点非配方；Con Panna=备选。（小严 COFFEE-004）

---

## 自检

- [x] 四级一级齐全（豆 / 经典 / 特调 / **糖浆**），一级二显示名无「意式经典」
- [x] 咖啡豆二级：选取 / 烘焙 / 发酵处理 / 储存
- [x] 经典咖啡二级：浓缩 / 奶咖 / 过滤
- [x] 现代特调二级：意式变奏 / 奶咖变奏（无季节/手法空壳）
- [x] 糖浆二级：基础 / 果味 / 香料 / 花香
- [x] 每类标配方卡 vs 知识点卡
- [x] JSON `coffee-labels-skeleton-v1.json` / `coffee-recipes-skeleton-v1.json` 已同步
- [x] 可交 Codex 建库（见 COFFEE-005）

---

## 拍板记录

### 小严（2026-10-23）

- 旧扁平三类（意式/奶咖/过滤）：**替换，不并存**
- 砍首版：杯型出品、手法笔记、季节门店空壳
- 对外用词：二级写「发酵处理」
- 过滤未拍前 JSON 不动（已解除——见阿拿）
- 现代特调 Dirty/Affogato/Tonic 可过；风味特调延后
- COFFEE-004：P01–P05 首版上；P06 厌氧概念卡；P07–P09 进阶；M10 Nitro→知识点；M06 Con Panna 备选

### 阿拿（2026-10-23）

- **选定方案②**：一级「意式经典」**改名**为「经典咖啡 Classic Coffee」，下分浓缩 / 奶咖 / 过滤
- 过滤**不**升成单独一级
- ~~一级三块~~ → **2026-10-24 四块**：① 咖啡豆 ② 经典咖啡 ③ 现代特调 ④ **糖浆 Syrups**（与经典/特调平级）

### 阿拿（2026-10-24）

- **糖浆升一级**：与经典咖啡、现代特调平级；一级 id `coffee-syrups`
- 二级首版：`syrup-base` / `syrup-fruit` / `syrup-spice` / `syrup-floral`（可再改名，不砍一级）
- JSON：`coffee-labels-skeleton-v1.json` 已追加 5 条（1 一级 + 4 二级）
