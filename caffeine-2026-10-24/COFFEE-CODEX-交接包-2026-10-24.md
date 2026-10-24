# 咖啡因 Normar · Codex 交接包（小严汇总）

日期：2026-10-24（Asia/Shanghai）  
汇总人：小严  
状态：**可交 Codex**（见「导入前须做」）  
未入库；等阿拿下令后由 Codex / 小库执行。

---

## 0. 一句话目标

把「咖啡因」配方库（经典 + 现代特调 + 糖浆）与「咖啡豆」知识点库（Obsidian）按定稿标签树接入 Normar，口径对齐鸡尾酒配方库模板；课料弱证据不写死为官方剂量。

---

## 1. 标签树（权威）

| 文件 | 路径 |
|------|------|
| 说明 | `/workspace/normar-handoff-2026-10-23/results/COFFEE-003-标签树.md` |
| JSON | `/workspace/normar-handoff-2026-10-23/results/coffee-labels-skeleton-v1.json`（**17** 标签） |

**一级（4）**

1. `coffee-beans` 咖啡豆 → `bean-select` / `bean-roast` / `bean-process` / `bean-storage`
2. `classic-coffee` 经典咖啡 → `classic-espresso` / `classic-milk` / `classic-filter`
3. `modern-signature` 现代特调 → `modern-espresso-twist` / `modern-milk-twist`
4. `coffee-syrups` 糖浆 → `syrup-base` / `syrup-fruit` / `syrup-spice` / `syrup-floral`

**拍板约束**

- 季风马拉巴知识点：`bean-process` + `bean-storage` **双挂**
- 不上树：杯型出品 / 手法笔记 / 季节空壳；拉花奶泡仅素材
- Luwak：**不上树**
- 与乙醇/鸡尾酒库分开

---

## 2. 配方库（机器可读优先）

### 2.1 经典咖啡（骨架 19）

- JSON：`/workspace/normar-handoff-2026-10-23/results/coffee-recipes-skeleton-v1.json`
- `labelIds`：**已挂**（浓缩 4 / 奶咖 7 / 过滤 5 / 意式变奏 2 / 奶咖变奏 1）

### 2.2 现代特调（127）

- JSON：`/workspace/normar-handoff-2026-10-23/results/coffee-modern-recipes-100plus-v1.json`
- 说明：`/workspace/normar-handoff-2026-10-23/results/COFFEE-008-现代特调100plus.md`
- `labelHint`：`modern-espresso-twist`×53 · `modern-milk-twist`×74（均合法）
- `labelIds`：**已按 `labelHint` 写成 `[hint]`（127；espresso-twist 53 / milk-twist 74；2026-10-24 小库补）**

### 2.3 糖浆（119）

- JSON：`/workspace/normar-handoff-2026-10-23/results/coffee-syrups-100plus-v1.json`
- 说明：`/workspace/normar-handoff-2026-10-23/results/COFFEE-009-糖浆100plus.md`
- 分布：base 38 / fruit 31 / spice 27 / floral 23
- `labelIds`：**已补且抽查通过**；44 款含 `linkedFromRecipeIds`（指向特调 id，已对得上）

### 2.4 课料消化（配方侧，不囫囵吞）

- `/workspace/normar-handoff-2026-10-23/results/COFFEE-012-课料消化整理-配方侧.md`
- 规则：课料 R01–R18 — **有官方源 → 建卡 + notes/story**；无官方源 → **只 notes/story**
- 小库说明：JSON 改动 0；是否把课料 notes 写入配方卡 **等阿拿拍**

### 2.5 早期种子（辅）

- `/workspace/normar-handoff-2026-10-23/results/coffee-modern-recipes-sourced-v1.json`（早期官方特调种子，勿覆盖 100plus）
- `/workspace/normar-handoff-2026-10-23/results/COFFEE-004-Codex内容种子.md`（若仍在 results；处理法/官方特调口径）

---

## 3. 知识点（Obsidian 知识库）

| 项 | 路径 |
|----|------|
| Vault 根 | `/workspace/notes/bar-inventory/caffeine-obsidian/`（约 **232** 篇） |
| 入口 MOC | `…/00-MOC-咖啡因知识库.md` |
| 011 吸收记录 | `…/_index/课料吸收记录-COFFEE-011.md` |
| 白咖啡对齐 | `…/_index/白咖啡对齐说明-COFFEE-011.md` |
| 去囫囵整理 | `…/_index/整理记录-去囫囵-2026-10-24.md` |
| 白咖啡卡 | `…/咖啡豆/烘焙/白咖啡两义项.md`（须含马来厂商 URL） |
| 季风草稿（配方侧对齐） | `/workspace/normar-handoff-2026-10-23/results/COFFEE-007-季风马拉巴-知识点草稿.md` |

**知识边界**：只咖啡豆四级；**不进**配方/糖浆；首版可见 P07–P09 / 白咖啡 / 利比里卡；瑕疵措辞冻结等 SCA CVA；GrainPro 概念钉。

**白咖啡强制 sources（进库门槛）**

1. https://www.oldtown.com.my/our-story/  
2. https://www.mycofe.com.my/index.php/about/company-profile  
3. （辅）https://www.msca.org.my/  

冲突 notes：OldTown「焦糖/高温」≠ 课料「低温无焦糖」→ **厂商为准，课料只注释**；健康断言勿进。

---

## 4. 课料学习原文（参考，非导入主件）

| 报告 | 路径 |
|------|------|
| 交接总入口 | `/workspace/normar-handoff-2026-10-23/results/COFFEE-011-小严课料学习交接包.md` |
| 005 / 005b / 005c | `/workspace/bar-saas/reviews/coffee-course-T0001/extracts/COFFEE-005*.md` |
| 手册 OCR 全文 | `…/extracts/ocr/咖啡鉴赏手册-ocr-full.txt` |
| 验收（知识库） | `…/extracts/COFFEE-010-知识库验收-小严-v1.md` |

---

## 5. 导入前须做（Codex / 小库）

1. **现代特调 127**：`labelHint` → `labelIds`（`[hint]`）— **已完成**（2026-10-24 小库；0 空挂载）。  
2. **确认糖浆 / 经典** `labelIds` 非空（已验）。  
3. **知识库 → Normar 知识点卡**：按 Obsidian 四级映射 `bean-*`；季风双挂；白咖啡带强制 URL。  
4. **Nitro 等**：知识点卡，不当可复现配方（若仍在种子里）。  
5. **课料 notes**：默认不写死剂量；是否批量写入配方 notes 字段等阿拿对 COFFEE-012 拍板。  
6. 截图/验收：iPhone 15 Pro Max 视口（既有 Normar 规范）。

---

## 6. 不要做

- 不要把课料 R01–R18 弱比例当 SCA/品牌默认值  
- 不要上 Luwak / 杯型 / 手法 / 季节空壳  
- 不要混入乙醇库内容  
- 不要在未下令前自行推生产

---

## 7. 验收勾选（导入后）

- [ ] 标签树 4 个 L1 可见且二级正确  
- [ ] 经典 19 / 特调 127 / 糖浆 119 均可筛选挂载  
- [ ] 糖浆↔特调交叉引用不断  
- [ ] 咖啡豆知识：选取/烘焙/处理/储存可浏览；季风双挂；白咖啡有马来 URL  
- [ ] 无 Luwak；无配方剂量被课料覆盖官方源  

---

## 8. 联系分工

| 角色 | 职责 |
|------|------|
| 小库 | 标签 JSON、配方/糖浆、Codex 执行协助 |
| 小存 | Obsidian 知识库内容 |
| 小严 | 本包汇总；**不再二验**除非阿拿再喊 |

**本包路径**：`/workspace/normar-handoff-2026-10-23/results/COFFEE-CODEX-交接包-2026-10-24.md`
