# ACTIVE_PLAN — 74_aerospace_defense_research 當前執行狀態與工作計畫

> **儲存庫**：`74_aerospace_defense_research`  
> **基準日期**：2026-10-19  
> **控制層更新**：2026-11-11（01–03 大綱、報告 35 證據分級、報告 17 單位鉗制、分叉取回）
> **當前 Stage**：**Framing**（F1–F7 於 2026-11-11 成立。Collection 未開始：主張表仍只有 6 列，primary 申報未入表。）
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
  [X]       [X]          [ ]          [ ]       [ ]        [ ]          [ ]
```

### 閘門 1：Capture ➔ Framing 推進檢查表
- [x] **有可命名題目**：`74_aerospace_defense_research`（航太、國防工業與雙用技術研究）。
- [x] **為何值得整理之核心價值**：在地緣政治緊張、全球國防預算擴張與非紅供應鏈重組下，辨識台灣供應鏈具備真實自由現金流之結構性受惠者。
- [x] **完成核心問題與邊界界定（Framing）**：F1–F7 於 2026-11-11 成立。stage 為 Framing。Current Synthesis 仍空。

#### Framing 退出條件（2026-11-05 訂立）

七項全部為真，才可把 stage 從 Capture 改為 Framing。出版長文、GitHub Pages 與期中選舉登記都不計入 stage。

| ID | 完成條件 | 驗收方式 | 2026-11-05 |
|---|---|---|---|
| F1 | README 恰好一句 Open Question，且不含 `；` 或 `;` 串列 | 讀 README 元資料表 | 通過 |
| F2 | README 同時寫出 Included 與 Excluded | 讀 README §2 | 通過 |
| F3 | 三份研究大綱都存在，且各含五段：一句問題、追蹤標的、primary 來源清單、一條可證偽條件、原型／MOU／PoC 與營收的區分 | `01_space_infrastructure_and_satellite_supply_chain.md`、`02_ndaa_non_red_drone_supply_chain.md`、`03_aerospace_primes_backlog_and_taiwan_machining.md` | 通過（2026-11-11）。三檔都在，五段都在。尚未把 primary 數字寫入主張表 |
| F4 | IRQ-01、IRQ-02、IRQ-03 在主張表各至少一列，五維皆為單一允許值 | CLM-74-001、CLM-74-002、CLM-74-003 | 通過 |
| F5 | `sources/report_index.csv` 覆蓋根目錄每一份編號研究稿，含 01–03、35、功能分支的 24 號與 `origin/main` 的 24 號州長查核、CH3。沒有任何列的 `document_role` 為 `synthesis` | 對照工作區編號稿與索引 `report_id` | 通過（2026-11-11 重新對照）。`git_sha` 在本次提交後以該提交為準 |
| F6 | Current Synthesis 為空 | README 元資料表寫「尚未建立」 | 通過 |
| F7 | 日期已過的 inbox 檢驗哨標成已觀察、未觀察或來源不足 | IRQ-06 的 2026-10-31 算力哨 | 通過。狀態為來源不足，似然比 1.0 |

`70_investment_hub/projects.yaml` 的一列不在這七項裡。Phase 5 仍待人工授權。

### 閘門 2：Framing ➔ Collection 檢查表（後續工作）
- [ ] 建立 Evidence Base / Sources 索引清單。`sources/report_index.csv` 只滿足 F5，不是 primary 證據庫。
- [ ] 擴充 `sources/claim_register.csv` 累積至少 10 筆具備五維標籤之主要主張。
- [ ] 排除單一來源依賴，核心財務數據必須取得官方 10-K/10-Q 或公司法說資料支持。

---

## 3. 下一步工作計畫（Action Plan）

| 階段 | 預計工作項目 | 預期交付成果 | 負責角色 | 狀態 |
|---|---|---|---|---|
| **Phase 1** | 完成倉庫骨架初始化與首輪主張基線登錄 | `AGENTS.md`, `README.md`, `claim_register.csv`, `00_inbox.md` | Argon / Subagent | **完成 (2026-10-19)** |
| **Phase 1b** | 控制層：報告索引、決策卡路徑、Framing 退出條件 | `sources/report_index.csv`；`00_inbox.md` 改指向 75；本節 F1–F7 | 本庫 | **完成 (2026-11-11)**。F3 已過，stage 為 Framing |
| **Phase 1c** | 2026 期中選舉開票與國防採購影響 | `24_us_midterm_2026_results_and_defense_impact_l1.md`；IRQ-07；CLM-74-004／005／006 | 本庫 | **完成 (2026-11-05)**。三列 `delta_db` 皆為 0.00 |
| **Phase 1d** | 期中選舉決策卡與決策分析 | `34_midterm_decision_analysis_l1.md`；75 的六張 `DC_20261105_*`。分數與報告 30 相同 | 本庫 | **完成 (2026-11-05)**。不寫主張表，不改 stage |
| **Phase 1e** | 2026-11-11 治理收斂 | 01–03 大綱、報告 17 單位鉗制、報告 35 證據分級、索引與 README、`plans/2026-11-11_branch_integration.md` | 本庫 | **完成 (2026-11-11)**。不合併 `main`。`spcx` 預覽維持 `duplicate`。Gemini 排程稿維持 navigation，雲端輸出不進主張表 |
| **Phase 2** | 深度調研 IRQ-01：SpaceX 與低軌衛星台系地面設備鏈 | `01_space_infrastructure_and_satellite_supply_chain.md` 已建立。下一步是 primary 申報入表 | 本庫 | **大綱完成 (2026-11-11)**。證據未蒐集，不得更新 CLM-74-001 現金流句 |
| **Phase 3** | 深度調研 IRQ-02：NDAA 非紅供應鏈與無人機自主防務 | `02_ndaa_non_red_drone_supply_chain.md` 已建立。下一步是標案與台廠長約 | 本庫 | **大綱完成 (2026-11-11)**。CLM-74-002 維持 0.00 |
| **Phase 4** | 深度調研 IRQ-03：航太主承包商積壓訂單與台灣鍛鑄造/結構件 | `03_aerospace_primes_backlog_and_taiwan_machining.md` 已建立。下一步是 10-K 與台廠科目 | 本庫 | **大綱完成 (2026-11-11)**。CLM-74-003 維持 0.00 |
| **Phase 5** | （獲跨庫授權後）向 `70_investment_hub` 提交 Registry 擴充與接入請求 | 更新 `70_investment_hub/projects.yaml` 並通過驗證器 | Human Gate / Parent | 待授權 |
