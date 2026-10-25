# ACTIVE_PLAN — 74_aerospace_defense_research 當前執行狀態與工作計畫

> **儲存庫**：`74_aerospace_defense_research`  
> **基準日期**：2026-10-19  
> **當前 Stage**：**Capture**（累積成熟度最高已通過 gate）  
> **維護者**：Argon & Flash Subagents  
> **主軸對齊**：國防航太實業技術 × 非紅供應鏈溢價 × 貝氏決策工程

---

## 1. 專案現行狀態（Current Status Snapshot）

- **版本庫初始化**：已完成本地 Git 倉庫初始化（`git init -b main`），具備獨立版本控制。
- **基礎契約結構**：
  - [x] `.gitignore`（忽略暫存檔與虛擬環境）
  - [x] `AGENTS.md`（作業契約、寫作憲法、禁詞令與雙重方法論約束）
  - [x] `README.md`（專案元資料、範圍邊界、四方協同關係表）
  - [x] `sources/claim_register.csv`（首 3 筆基準主張與貝氏對數勝算登錄）
  - [x] `00_inbox.md`（首輪 3 項 IRQ 觸發事件與競爭假設對稱分析）
  - [x] `plans/ACTIVE_PLAN.md`（本計畫追蹤文件）
- **外部依賴狀態**：
  - 嚴格維持與 `70_investment_hub` 之邊界，尚未修改 `70`、`71`、`72`、`73` 之任何檔案。

---

## 2. Knowledge Stage 成熟度閘門檢查表

依據 `70_investment_hub/AGENTS.md` §4 定義之標準成熟度閘門：

```text
Capture ➔ Framing ➔ Collection ➔ Analysis ➔ Review ➔ Synthesis ➔ Maintenance
  [X]       [ ]          [ ]          [ ]       [ ]        [ ]          [ ]
```

### 閘門 1：Capture ➔ Framing 推進檢查表
- [x] **有可命名題目**：`74_aerospace_defense_research`（航太、國防工業與雙用技術研究）。
- [x] **為何值得整理之核心價值**：在地緣政治緊張、全球國防預算擴張與非紅供應鏈重組下，辨識台灣供應鏈具備真實自由現金流之結構性受惠者。
- [ ] **完成核心問題與邊界界定（Framing）**：
  - [x] 核心問題明確：單一 Open Question 已載入 `README.md`。
  - [x] 納入與排除範圍（Included / Excluded）已界定。
  - [ ] **完成條件（Completion Criteria）可驗收**：待完成首批主要追蹤標的（民用航太製造、衛星地面設備、無人機載具）之研究大綱文件。

### 閘門 2：Framing ➔ Collection 檢查表（後續工作）
- [ ] 建立 Evidence Base / Sources 索引清單。
- [ ] 擴充 `sources/claim_register.csv` 累積至少 10 筆具備五維標籤之主要主張。
- [ ] 排除單一來源依賴，核心財務數據必須取得官方 10-K/10-Q 或公司法說資料支持。

---

## 3. 下一步工作計畫（Action Plan）

| 階段 | 預計工作項目 | 預期交付成果 | 負責角色 | 狀態 |
|---|---|---|---|---|
| **Phase 1** | 完成倉庫骨架初始化與首輪主張基線登錄 | `AGENTS.md`, `README.md`, `claim_register.csv`, `00_inbox.md` | Argon / Subagent | **完成 (2026-10-19)** |
| **Phase 2** | 深度調研 IRQ-01：SpaceX 與低軌衛星台系地面設備鏈 | 建立 `01_space_infrastructure_and_satellite_supply_chain.md` | Subagent | 待啟動 |
| **Phase 3** | 深度調研 IRQ-02：NDAA 非紅供應鏈與無人機自主防務 | 建立 `02_ndaa_non_red_drone_supply_chain.md` | Subagent | 待啟動 |
| **Phase 4** | 深度調研 IRQ-03：航太主承包商積壓訂單與台灣鍛鑄造/結構件 | 建立 `03_aerospace_primes_backlog_and_taiwan_machining.md` | Subagent | 待啟動 |
| **Phase 5** | （獲跨庫授權後）向 `70_investment_hub` 提交 Registry 擴充與接入請求 | 更新 `70_investment_hub/projects.yaml` 並通過驗證器 | Human Gate / Parent | 待授權 |
