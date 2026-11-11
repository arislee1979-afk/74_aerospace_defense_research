# 74_aerospace_defense_research — 航太、國防工業與雙用技術研究庫

> 2026-10-25 本機權威：本庫正式 Mac 目錄為 source of truth，GitHub 保存版本備份與查核快照。依 [Local-first 合約](/Users/arislee/0_project_mac/00_agent_control_plane/docs/LOCAL_FIRST_AUTHORITY.md) 區分草稿、人工採納與發布；既有 runtime 權限不隨文件更新而擴張。

> **專案定位**：航太、國防工業、低軌衛星與軍工雙用供應鏈之實業與政策研究生產者（Producer Repo）。  
> **研究視角**：立足台灣產業製造與地緣位置，結合美歐國防預算、太空基礎設施演進與非紅供應鏈認證，建立具備實質財務現金流檢驗力之深度研究基座。  
> **基準方法**：全面遵循 [`../70_investment_hub/docs/epistemic_schema.md`](../70_investment_hub/docs/epistemic_schema.md) 之五維認識論標籤與 [`../70_investment_hub/docs/BAYESIAN_DECISION_FRAMEWORK.md`](../70_investment_hub/docs/BAYESIAN_DECISION_FRAMEWORK.md) 之貝氏決策工程。

---

## 1. 專案元資料（Project Metadata）

| 欄位 | 設定值 | 說明 |
|---|---|---|
| **專案識別（Local ID）** | `74_aerospace_defense_research` | 本機工作目錄唯一識別碼 |
| **角色定位（Role）** | `Producer`（實業／國防航太／雙用技術生產者） | 生產一手研究與證據，不複製外部雜訊 |
| **當前成熟度階段（Knowledge Stage）** | **Framing** | 2026-11-11：F1–F7 成立。01–03 大綱已寫入。Primary 申報尚未入主張表，故未進 Collection |
| **當前正式綜述（Current Synthesis）** | **尚未建立** | 待完成 Review exit 閘門後方可收斂唯一正式 Synthesis |
| **核心待解問題（Open Question）** | **在美中供應鏈脫鉤與北約／印太國防預算結構性擴張下，台灣航太軍工與低軌衛星供應鏈哪些次產業具備經得起財報自由現金流檢驗的「非紅供應鏈溢價」而非短期題材炒作？** | 嚴格維持單一句、聚焦財務實證 |
| **當前下一步行動（Next Action）** | **以 primary 申報核對 CLM-74-002 與 CLM-74-003，未出現可核對長約或 Backlog 原件前維持這兩列 delta_db 為 0.00。** | 嚴格單一可交付成果、無多動詞串列 |

---

## 2. 研究邊界：納入與排除原則（Included vs Excluded）

### 2.1 納入範疇（Included）
1. **太空基礎設施與低軌衛星（Space Infrastructure & LEO Satellites）**：
   - 商業發射載具可重複使用之經濟模型、入軌發射成本與發射頻率（如 SpaceX Falcon / Starship 模式）。
   - 低軌衛星酬載、相控陣列天線（Phased Array）、高頻 RF 元件、太空級 PCB 與地面接收終端（User Terminals）之台廠供應鏈生態。
2. **現代 AI 國防科技與自主無人防務系統（Autonomous Defense & Edge AI）**：
   - 無人機（UAV）、無人水面載具（USV）、反無人機防禦架構（C-UAS）、滯空彈藥（Loitering Munitions）之軟硬體整合架構。
   - 國防新創公司架構（如 Anduril 分散式自主指揮系統 Lattice、Palantir 國防資料融合模式 AIP/Gotham）之採購演變。
3. **傳統航太製造、造船與防務承包商（Aerospace Tier-1, Shipbuilding & Primes）**：
   - 機體結構、軍規發動機渦輪鍛鑄件、高階碳纖維複合材料（CFRP）、稀有耐高溫合金之供應鏈瓶頸。
   - 主承包商（Defense Primes）積壓訂單（Backlog）、交期前導期（Lead Time）、高齡技工斷層與自由現金流（FCF）轉換率。
4. **非紅供應鏈實證與美台防務產能對接（Non-Red Supply Chain & NDAA Compliance）**：
   - 歐美《國防授權法》（NDAA）與資安標準對通訊、無人機與關鍵材料之去風險化實證。
   - 台灣航太製造與資通訊廠商在非紅供應鏈中的轉單動能、認證時程與實質毛利率擴張。

### 2.2 排除範疇（Excluded）
- ❌ 未經官方國防預算書、監管申報（SEC 10-K/10-Q）或政府正式招標公報佐證之軍事情報小道傳聞。
- ❌ 純粹煽動性地緣政治推演或自媒體戰爭劇本推測。
- ❌ 缺乏商業量產合約佐證之純樣品展示、概念雛型或備忘錄（MOU）炒作。

---

## 3. 與 70 / 71 / 72 / 73 兄弟專案之四方協同聯動

本庫作為專門之生產者，與既有研究生態系形成緊密因果互補：

| 協同專案 | 專案定位 | 本庫與其聯動機制與因果互動 |
|---|---|---|
| **`70_investment_hub`** | 知識中樞與策略索引 | **決策框架與策略映射**：共用五維認識論標籤（`epistemic_schema.md`）與貝氏評分規範（`BAYESIAN_DECISION_FRAMEWORK.md`），為未來可能的國防／航太策略卡提供經檢驗之上游證據。 |
| **`71_china_overcapacity`** | 供給過剩與外溢機制 | **反身性管制與去風險化**：對照中國商用造船、消費級無人機（如 DJI 模式）與成熟零組件產能過剩，如何觸發美歐「國防授權法（NDAA）／非紅供應鏈」強制排他條款，從而為台灣廠商創造非紅替代溢價。 |
| **`72_semiconductor_research`** | 半導體實業與技術 | **軍規極限封裝與特殊化合物**：對照高抗輻射航太封裝、GaN（氮化鎵）／SiC（碳化矽）在主動相位陣列雷達與高功率微波防衛之應用，以及台積電特殊製程在軍工防務之不可替代性。 |
| **`73_deepseek_Kimi`** | 算力敘事與模型競爭 | **邊緣端自主載具與軍規推論**：對照極限壓縮成本模型（如 DeepSeek 類極致 Token 經濟）與 Agent Loop Harness 如何遷移至離線或頻寬受限環境，支援無人載具之邊緣自主決策。 |

---

## 4. 目錄結構與導覽

```text
74_aerospace_defense_research/
├── AGENTS.md                  # 作業契約、禁詞令與方法論
├── README.md                  # 本文件。Maturity、Open Question、Next Action 以本表為準
├── index.html                 # 報告 14 的發布頁。不是全庫目錄，也不是 Current Synthesis
├── 00_inbox.md                # IRQ 收集箱
├── 01_space_infrastructure_and_satellite_supply_chain.md
├── 02_ndaa_non_red_drone_supply_chain.md
├── 03_aerospace_primes_backlog_and_taiwan_machining.md
├── 10_ … 35_                  # 編號研究稿。清單與五維標籤見 sources/report_index.csv
├── sources/
│   ├── claim_register.csv     # 唯一可寫後驗的主張表（CLM-74-001 至 006）
│   └── report_index.csv       # 報告索引。不是 primary 證據庫
├── plans/
│   ├── ACTIVE_PLAN.md
│   └── 2026-11-11_branch_integration.md
└── spcx/report/               # Starshield 側袋。圖預覽列為 duplicate
```

編號稿的閱讀入口：期中選舉組用 `25_midterm_ai_reports_index_l1.md`。全庫用 `sources/report_index.csv`。`origin/main` 另有一份 24 號州長查核，檔名是 `24_us_midterm_governors_ai_datacenter_grid_policy_factcheck_l1.md`，與 `24_us_midterm_2026_results_and_defense_impact_l1.md` 並存。

---

*本專案為產業供應鏈與實業投資研究，所有內容皆為假設檢驗與財務分析，不構成任何證券買賣建議。*
