# AGENTS.md — 74_aerospace_defense_research 作業契約與最高憲法

> **適用範圍**：本 Repository (`74_aerospace_defense_research`) 全部檔案與協同 AI 代理人。  
> **制定宗旨**：規範航太、國防工業與軍工雙用技術供應鏈研究之推論紀律與輸出語感，徹底杜絕軍事自媒體與大眾行銷常見之誇張渲染與非客觀修辭，確保產出品質嚴格對齊頂尖智庫、國防採購評估與實業財務分析標準。  
> **生效日期**：2026-10-19 起永久生效。  
> **核心繼承文獻**：  
> - 認識論標籤：[`../70_investment_hub/docs/epistemic_schema.md`](../70_investment_hub/docs/epistemic_schema.md)  
> - 貝氏決策憲法：[`../70_investment_hub/docs/BAYESIAN_DECISION_FRAMEWORK.md`](../70_investment_hub/docs/BAYESIAN_DECISION_FRAMEWORK.md)  
> - 策略索引：[`../70_investment_hub/02_us_china_taiwan_industry_strategy_index.md`](../70_investment_hub/02_us_china_taiwan_industry_strategy_index.md)

---

## 0. 本庫定位與研究邊界

本庫為 Investment Research Workspace 體系下之**第四個研究生產者庫（Producer Repo）**，與 `71_china_overcapacity`（供給／外溢）、`72_semiconductor_research`（實業／技術）、`73_deepseek_Kimi`（敘事／算力）平行協同。

### 0.1 研究涵蓋範疇
1. **太空基礎設施與低軌衛星（Space Infrastructure & LEO Satellites）**：
   - 商業火箭可重複使用發射成本曲線（如 SpaceX Falcon / Starship 模式）、發射頻率與入軌成本。
   - 衛星酬載、相控陣列天線、RF 射頻模組、太空用高階 PCB、地面接收終端（User Terminals）之供應鏈與營運現金流。
2. **現代 AI 國防科技與自主系統（Autonomous Systems & AI Defense）**：
   - 無人載具（UAV / USV / UGV）、反無人機防禦架構（C-UAS）、滯空彈藥與軟硬體整合架構（如 Anduril、Palantir 國防資料融合模式）。
   - 邊緣軍規推論算力與感測器融合（Sensor Fusion）。
3. **傳統航太製造與軍工造船（Aerospace Tier-1 / Defense Primes / Shipbuilding）**：
   - 商用客機與軍用機體／發動機結構件、航太渦輪葉片、高階複合材料（CFRP）、稀有金屬鍛鑄造。
   - 主承包商（Defense Primes）積壓訂單（Backlog）、多年期採購合約、技工短缺瓶頸與自由現金流（FCF）轉換率。
4. **非紅供應鏈與美台防務產能對接（Non-Red Supply Chain & NDAA Compliance）**：
   - 歐美《國防授權法》（NDAA）與資安合規框架對中國零組件、磁性材料、通訊光電與無人機零組件之去風險化實證。
   - 台灣航太軍工、造船、網通與地面終端廠商之轉單效應、認證壁壘與實質財務營收比重。

---

## 1. 雙重方法論約束：認識論五維標籤 × 貝氏決策評分

本庫所有陳述、研究擴展與資料登錄，必須同時受制於以下兩套工程標準：

### 1.1 認識論五維標籤約束（Epistemic Schema）
依據 [`../70_investment_hub/docs/epistemic_schema.md`](../70_investment_hub/docs/epistemic_schema.md)，所有主張必須標註單一五維屬性，嚴禁復合或混淆：
- `claim_type`: `fact` · `estimate` · `inference` · `hypothesis` · `scenario`
- `source_tier`: `primary`（官方預算書/SEC申報/正式採購合約）· `secondary`（專業防務智庫/主流期刊）· `lead`（軍事論壇/未具名爆料）· `internal`（作者壓力測試）
- `document_role`: `raw` · `analysis` · `review` · `synthesis` · `registry` · `navigation`
- `verification_status`: `verified` · `partially_verified` · `requires_verification` · `conflicting` · `superseded` · `rejected`
- `workflow_disposition`: `promote` · `keep` · `investigate` · `duplicate` · `reject`

### 1.2 貝氏決策量化評分約束（Bayesian Decision Framework）
依據 [`../70_investment_hub/docs/BAYESIAN_DECISION_FRAMEWORK.md`](../70_investment_hub/docs/BAYESIAN_DECISION_FRAMEWORK.md)：
1. **三維輸入架構**：
   - **單點突破事件 $E$ ＝ CPU 中斷請求（IRQ）**：載入關注清單，嚴禁直接作為信心高點，強制執行先驗重置（Prior Reset）。
   - **大環境週期 ＝ 先驗機率底數 $P(H)$**：國防預算擴張順風（$0\text{ dB}$ / $50\%$）、供應鏈認證分化（$-3.7\text{ dB}$ / $30\%$）、和平紅利/預算裁減逆風（$-7.5\text{ dB}$ / $15\%$）。遵守克倫威爾法則（禁設 $0\%$ 或 $100\%$）。
   - **股價位階 ＝ 市場隱含機率 $P_{\text{mkt}}(H)$ 與價格彈性測試**：防務題材若利多見報卻爆量破線，視為負向似然比 $E_{\text{price}}$（$\Delta \text{dB} \le -5.2\text{ dB}$）。
2. **對稱檢驗與共模雜訊濾除**：
   - 必須同時評估分子 $P(E \mid H)$ 與分母競爭假設 $P(E \mid \neg H)$。
   - **未核實軍事傳聞或官方宣傳稿強制鉗制為 $0\text{ dB}$**（`requires_verification`，$\Lambda = 1.0$），禁止驅動信念更新。
3. **四階狀態機（State Machine）**：
   - State 0（喚醒/0%）$\to$ State 1（探針倉/1–2%）$\to$ State 2（主力倉/8–12% 需 $\ge +4.8\text{ dB}$ 且經真金白銀財報驗證）$\to$ State 3（除錯清倉/0% 觸發殺手開關即刻執行）。

---

## 2. 嚴格寫作憲法與禁詞令（Writing Standards）

國防與軍工議題極易引發自媒體與網路社群的非理性情緒渲染。全體 AI 代理人在此必須遵守以下鐵律：

### 2.1 嚴禁使用之煽動性詞彙
- ❌ **絕對禁用**：「終極王牌」、「秒殺」、「降維打擊」、「無敵」、「完勝」、「血洗」、「破防」、「全面崩潰」、「必然稱霸」、「戰力爆表」、「殺手鐧」。

### 2.2 強制替換之專業智庫與財務術語
- ✔️ **強制採用**：「非對稱作戰成本交換比（Cost-Exchange Ratio）」、「國防預算邊際排擠效應」、「主承包商積壓訂單（Contract Backlog）與交付爬坡（Production Ramp）」、「NDAA 合規認證進入門檻」、「長週期前導期（Lead Time）瓶頸」、「雙用技術外溢效應（Dual-Use Technology Spillover）」、「供應鏈去風險化替代彈性」。

### 2.3 嚴格區分「研發原型、小批量交付」與「可規模化量產」
- 國防專案常有長達數年之測試驗證期。**禁止將展示樣機、意向備忘錄（MOU）或概念驗證（PoC）直接等同於已實現獲利或規模化產能**。

---

## 3. 工作流程、授權與邊界

1. **獨立 Git 管理**：
   - 本庫為獨立 Git 倉庫，預設分支為 `main`。
   - GitHub accepted/default branch 為版本化權威；本機目錄為執行環境。
   - **禁止直接 push `main`**；工作分支完成後需經明確驗證。
2. **跨庫邊界**：
   - 本庫未經使用者明確跨庫授權前，**嚴禁修改** `70_investment_hub`、`71_china_overcapacity`、`72_semiconductor_research`、`73_deepseek_Kimi`。
   - 本庫所產生之階段性結論與交付成果，先記錄於本庫 `plans/ACTIVE_PLAN.md` 或交接文件中，待授權後再依照 Hub 流程回寫 `projects.yaml`。
3. **驗證與交付完成條件**：
   - 遵循 Producer-first 原則，本庫 README 擁有本庫之 Maturity Stage、Open Question 與 Next Action。
   - 變更後執行 `git diff --check` 與 `git status --short --branch` 確認無多餘暫存檔或格式瑕疵。
