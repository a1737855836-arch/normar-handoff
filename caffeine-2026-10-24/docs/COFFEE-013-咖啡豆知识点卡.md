# COFFEE-013 · 咖啡豆知识点卡（选取/烘焙/发酵处理/储存）

| 字段 | 内容 |
|------|------|
| 任务 | COFFEE-013 |
| 日期 | 2026-10-24（Asia/Shanghai） |
| 执行 | 小库（配方库侧 · Normar 知识点卡） |
| 状态 | **JSON 已落盘 · 不交 Codex**（阿拿已打住导入） |
| 对齐 | COFFEE-003 标签树；COFFEE-004 P01–P09；COFFEE-007 季风/白咖啡强制口径 |
| JSON | `coffee-bean-knowledge-cards-v1.json` |

## 0. 计数总览

| labelId | 显示名 | 张数（按 label 挂载计） |
| --- | --- | ---: |
| `bean-select` | Selection选取 | 12 |
| `bean-roast` | Roast烘焙 | 8 |
| `bean-process` | Process发酵处理 | 11 |
| `bean-storage` | Storage储存 | 8 |
| **卡片总张数** | — | **38** |

> 季风马拉巴双挂 `bean-process` + `bean-storage`，故四级挂载次数之和 = 总张数 + 1。

规模理由：目标 35–55；本版 **38** 张短卡——处理法按 004 必上+进阶全覆盖，选取只做决策层入门+少量品种钉，烘焙/储存覆盖家用核心与争议提示；**刻意不镜像** Obsidian 产国/产区/品种长尾。

## 1. 卡片目录（一行一卡）

### Selection选取 (`bean-select`)

| id | 中文 | English | labelIds |
| --- | --- | --- | --- |
| `select-arabica-robusta` | 阿拉比卡与罗布斯塔 | Arabica & Robusta | `bean-select` |
| `select-liberica` | 利比里卡 | Liberica | `bean-select` |
| `select-blend-vs-single` | 拼配与单品 | Blend vs Single Origin | `bean-select` |
| `select-origin-altitude` | 产地与海拔入门 | Origin & Altitude Intro | `bean-select` |
| `select-defects-intro` | 瑕疵豆识别入门 | Green Coffee Defects Intro | `bean-select` |
| `select-harvest-ripeness` | 采收成熟度入门 | Harvest Ripeness | `bean-select` |
| `select-green-vs-roasted` | 生豆与熟豆 | Green vs Roasted Coffee | `bean-select` |
| `select-specialty-vs-commodity` | 精品与商品咖啡入门 | Specialty vs Commodity Coffee | `bean-select` |
| `select-coffee-belt` | 咖啡带 | Coffee Belt | `bean-select` |
| `select-gesha` | 瑰夏 / 艺伎 | Gesha / Geisha | `bean-select` |
| `select-common-cultivars` | 常见阿拉比卡品种钉 | Common Arabica Cultivars (Typica/Bourbon/Caturra…) | `bean-select` |
| `select-quaker` | Quaker（未熟烘后豆） | Quaker (Underripe After Roast) | `bean-select` |

### Roast烘焙 (`bean-roast`)

| id | 中文 | English | labelIds |
| --- | --- | --- | --- |
| `roast-spectrum` | 烘焙度谱 | Roast Spectrum (Light/Medium/Dark) | `bean-roast` |
| `roast-first-crack` | 一爆 | First Crack | `bean-roast` |
| `roast-second-crack` | 二爆 | Second Crack | `bean-roast` |
| `roast-resting-degassing` | 养豆与排气 | Resting & Degassing | `bean-roast` |
| `roast-agtron-names` | Agtron 与焙名不统一 | Agtron & Inconsistent Roast Names | `bean-roast` |
| `roast-city-names` | City / Full City 等焙名 | City, Full City & Named Roasts | `bean-roast` |
| `roast-white-coffee` | 白咖啡 | White Coffee / Ipoh White Coffee | `bean-roast` |
| `roast-caffeine-myth` | 深烘咖啡因更低？（提示） | Dark Roast Caffeine Myth (Note) | `bean-roast` |

### Process发酵处理 (`bean-process`)

| id | 中文 | English | labelIds |
| --- | --- | --- | --- |
| `process-washed` | 水洗 | Washed | `bean-process` |
| `process-natural` | 日晒（干法） | Natural / Dry Process | `bean-process` |
| `process-honey` | 蜜处理 | Honey Process | `bean-process` |
| `process-honey-colors` | 蜜处理颜色档 | Honey Color Grades (White/Yellow/Red/Black) | `bean-process` |
| `process-pulped-natural` | 去皮日晒 / 半水洗 | Pulped Natural / Semi-washed | `bean-process` |
| `process-wet-hulled` | 湿刨 | Wet-hulled / Giling Basah | `bean-process` |
| `process-anaerobic` | 厌氧发酵 | Anaerobic Fermentation | `bean-process` |
| `process-carbonic-maceration` | 二氧化碳浸渍 | Carbonic Maceration | `bean-process` |
| `process-lactic` | 乳酸向（厌氧子标签） | Lactic (Anaerobic Sub-label) | `bean-process` |
| `process-yeast-inoculated` | 酵母接种 | Yeast-inoculated Fermentation | `bean-process` |
| `bean-monsoon-malabar` | 季风马拉巴 | Monsooned Malabar | `bean-process,bean-storage` |

### Storage储存 (`bean-storage`)

| id | 中文 | English | labelIds |
| --- | --- | --- | --- |
| `bean-monsoon-malabar` | 季风马拉巴 | Monsooned Malabar | `bean-process,bean-storage` |
| `storage-seal-light-temp` | 密封避光温度 | Airtight, Dark, Cool Storage | `bean-storage` |
| `storage-after-opening` | 开封后建议 | After Opening | `bean-storage` |
| `storage-whole-vs-ground` | 整豆优于预磨 | Whole Bean over Pre-ground | `bean-storage` |
| `storage-valve-bag` | 单向排气阀袋 | One-way Degassing Valve Bag | `bean-storage` |
| `storage-freshness-staling` | 新鲜度与失鲜 | Freshness & Staling | `bean-storage` |
| `storage-freezing-controversy` | 冷冻熟豆（争议） | Freezing Roasted Beans (Disputed) | `bean-storage` |
| `storage-best-by` | 最佳食用期解读 | Best-By Date Reading | `bean-storage` |

## 2. 出处策略

| 主题族 | 主出处偏好 | 本版做法 |
| --- | --- | --- |
| 处理法 P01–P05 | NCA Processes + Royal/Peet's/Sustainable Harvest | 已写入；每卡 ≥1 可点 URL |
| 厌氧/CM/乳酸/酵母 | Royal 术语文；CM 辅 Sasa Sestic | P06 概念；P07–P09 标进阶 notes |
| 季风马拉巴 | 印度咖啡局 + Barista Magazine + NKG | 对齐 007；双挂 |
| 种属/产地海拔/单品 | NCA Varieties / What is coffee | 短卡；不做国别全书 |
| 瑕疵 | SCA CVA + SCA News 绿分级讨论 | 入门卡；措辞待 CVA 深化 |
| 品种钉 Gesha | World Coffee Research catalog | 单钉；警示名实不符 |
| 烘焙度/养豆 | NCA Roasts；Agtron 辅 Coffee Review / Counter Culture | 焙名不统一单独提示 |
| 白咖啡 | **强制** OldTown + MyCofe；辅 MSCA | 冲突进 notes；剔健康断言 |
| 储存 | NCA Storage and shelf life；阀袋辅 ATK | 冷冻标争议 |

课料 alone 不够：本 JSON **未**把课料 DOC 当 sourceUrls。

## 3. 强制口径核对

### 白咖啡 `roast-white-coffee`

- `labelIds`: 仅 `bean-roast`
- `sourceUrls` 含：
  1. https://www.oldtown.com.my/our-story/
  2. https://www.mycofe.com.my/index.php/about/company-profile
  3. https://www.msca.org.my/（辅）
- notes 已写 OldTown「受控焙度/caramelizes」与课料「不加焦糖低温」冲突
- 无健康功效正文

### 季风马拉巴 `bean-monsoon-malabar`

- `labelIds`: `bean-process` + `bean-storage`（双挂）
- 主 URL：coffeeboard.gov.in Specialitycoffee + baristamagazine + nkgindiacoffee
- 正文区分日晒/水洗/季风；非罐内厌氧

## 4. 与 COFFEE-004 / 007 / Obsidian 差分

### vs COFFEE-004

| 004 | 本版 |
| --- | --- |
| P01–P05 必上 | 已成卡 |
| P06 可选概念 | 已成卡 |
| P07–P09 进阶 | 已成卡，notes 标进阶 |
| Honey 颜色档建议另条 | `process-honey-colors` |
| 相邻：拼配/瑕疵/养豆 | 已分别挂 select/roast |
| 延后：共酵/Luwak/水分水活度 | **仍不上** |

### vs COFFEE-007

| 007 | 本版 |
| --- | --- |
| 季风双挂草稿 | 已入库 JSON（仍不交 Codex） |
| 白咖啡强制 URL + notes 冲突 | 已落实 |
| R01–R18 配方规则 | 不在本任务范围 |

### vs Obsidian（只读对齐 · 未改 vault）

**本版覆盖的核心选题（映射）**

- 选取：阿拉比卡/罗布斯塔、利比里卡钉、拼配与单品、产地与海拔、瑕疵入门、采收成熟度、生豆与熟豆、精品与商品、咖啡带、Gesha、常见品种总览、Quaker
- 烘焙：烘焙度谱、一爆、二爆、养豆排气、Agtron/焙名、City 等焙名、白咖啡两义项、深烘咖啡因提示
- 发酵处理：水洗/日晒/蜜/颜色档/去皮日晒/湿刨/厌氧/CM/乳酸/酵母/季风
- 储存：密封避光、开封后、整豆优于预磨、阀门袋、新鲜度失鲜、冷冻争议、最佳食用期；季风由双挂覆盖

**Obsidian 多出、本版刻意未镜像（延后清单）**

| 类别 | 示例（Obsidian 有 · Normar 未上） | 理由 |
| --- | --- | --- |
| 产国主卡 | 埃塞/肯尼亚/哥伦比亚/巴西/印尼/云南… 全套 | 不上产地长百科；选「咖啡带+海拔」入门钉即可 |
| 产区/贸易名子卡 | 耶加雪菲、西达摩、Antigua、塔拉苏、曼特宁、Kona… | 读标签用；勿第二套百科 |
| 品种长尾 | Typica/Bourbon/SL28/Pacamara/Castillo… 分卡 | 仅留 Gesha + 常见品种总览 |
| 瑕疵分卡 | 全黑/酸豆/虫蛀/破碎… | 仅入门总卡；措辞冻结等 CVA |
| 烘焙化学深卡 | 美拉德、焦糖化、发展时间、曲线入门长文 | 首版用节点卡（一爆/二爆/色度） |
| 储存生豆仓 | GrainPro、冷冻生豆 | 家用熟豆优先；概念延后 |
| 史实故事 | `_史实故事`、产地史 | 不囫囵吞进 JSON |
| 争议长文 | 第三波定义、单品纯度营销等 | 仅在相关卡 notes 点到为止 |
| Luwak 等 | — | 004 已定不上树 |

## 5. 未收录 / 延后清单（给拍板）

1. 产国/产区钉批量（Obsidian 当代产国主卡）— 需当代 URL 再议，勿课料史实 alone
2. 品种分卡（除 Gesha）
3. 瑕疵分卡细化（等 SCA CVA）
4. Co-ferment / 果香共酵 / Luwak
5. 水分与水活度工艺参数
6. GrainPro / 生豆仓专业仓储
7. 烘焙曲线/发展时间操作手册化

## 6. 自检

- [x] 四级 labelIds 覆盖
- [x] 全卡 `cardType=knowledge` + `reproducibleRecipe=false`
- [x] 白咖啡强制厂商 URL + 冲突 notes
- [x] 季风双挂
- [x] 每卡 ≥1 sourceUrls（未伪造）
- [x] 未写 Obsidian vault
- [x] 未交 Codex / 未推导入
- [x] 与乙醇库分离（本目录仅咖啡因交接包）

## 7. 落盘路径

1. `/workspace/normar-handoff-2026-10-23/results/coffee-bean-knowledge-cards-v1.json`
2. `/workspace/normar-handoff-2026-10-23/results/COFFEE-013-咖啡豆知识点卡.md`

