# Gemini App 排程設計（74_aerospace_defense_research）

> 狀態：設計草稿（`document_role: navigation`，`verification_status: requires_verification`）。排程輸出僅為 IRQ 候選線索（`source_tier: lead` 起算），不得直接寫入 `claim_register.csv` 或驅動信念更新（見 AGENTS.md §1.2、§3）。

## 0. 先決限制

| 項目 | 說明 |
|---|---|
| 執行位置 | Gemini App「已排定」在雲端執行；不能直接寫本機資料夾。 |
| 防休眠開關 | 畫面上「防止 Mac 進入休眠」建議開啟，避免排程錯過。 |
| 落地方案 | Gemini 把結果存到 Google Drive 資料夾 `74_gemini_inbox`（或寄 Gmail 給自己），由 Drive for Desktop 同步到 Mac，再由本機腳本複製到 repo。**需先手動測一次，確認 Gemini 能否建檔到指定資料夾。** |
| 本機落點 | `sources/gemini_inbox/YYYY-MM-DD_<slug>.md`（建議加入 `.gitignore` 或只採納後 commit） |
| 治理 | 每份輸出先進 `00_inbox.md` 的 IRQ 流程，需分母對稱檢驗後才登錄。 |

## 1. 追蹤標的（取自 repo）

- 太空／SpaceX 生態：SpaceX（Q3 2026 財報、Terafab、渦輪發電機、2026-10-31 算力 1.7→2.2 GW 檢驗哨）、Starlink、Starshield、Google Suncatcher／Planet、Tesla Roadster（COPV 雙用）。
- 台系衛星／航太鏈：昇達科 3491、啟碁 6285、華通 2313、漢翔 2634、駐龍 5222、寶一 8222（股票代號需核對）。
- 國防科技：Anduril、Palantir；主承包商 Lockheed Martin、RTX、Boeing、Airbus。
- 主題：NDAA 非紅供應鏈、C-UAS／無人機、Backlog 與鍛鑄件交期、SpaceX 現金流與 IPO。

## 2. 排程總表（對應畫面欄位）

| # | 任務名稱 | 頻率 | 時間 | 結束時間 | 對應 IRQ |
|---|---|---|---|---|---|
| S1 | 74-每日事件偵測 | 每天 | 07:30 | 永不 | IRQ-01/02/04/06 |
| S2 | 74-週一一手來源檢核 | 每週一 | 08:00 | 永不 | IRQ-01/03/06 |
| S3 | 74-週五台系供應鏈 | 每週五 | 18:00 | 永不 | IRQ-01/02/03 |
| S4 | 74-SpaceX 算力檢驗哨 | 一次 | 2026-11-01 08:00 | 該日 | IRQ-06 |

## 3. 共用輸出規格（每個 Prompt 末尾附上）

```
輸出為單一 Markdown 檔，存到 Google Drive 資料夾「74_gemini_inbox」，檔名 YYYY-MM-DD_<任務代號>.md。
檔頭 YAML：date, task, sources_count。
每則發現一個區塊，欄位：
- 標題 / 日期 / 連結（必須是可點擊的原始網址）
- claim_type（fact|estimate|inference|hypothesis|scenario）
- source_tier（primary=SEC/預算書/公開資訊觀測站/政府公報；secondary=智庫與主流媒體；lead=論壇/未具名爆料）
- verification_status（只能填 verified 或 requires_verification）
- 對應 IRQ 編號
- 多頭假設 H_A 影響 / 空頭假設 H_B 影響（必須兩邊都寫）
規則：
1. 無原始連結者一律標 requires_verification，不得給結論。
2. 禁用「秒殺、降維打擊、無敵、完勝、血洗、破防、殺手鐧」等煽動詞。
3. 展示樣機、MOU、PoC 不得寫成已實現營收或量產。
4. 沒有新資訊時輸出「本期無新增」，不得湊數。
5. 結尾列出「建議進入 00_inbox 的候選項」，不超過 3 項。
```

## 4. 各排程 Prompt

### S1 每日事件偵測（07:30）

```
搜尋過去 24 小時（台北時間）的網路資料，範圍：
(a) SpaceX / Starlink / Starshield：發射頻率、Starship 進展、財報與 IPO、烏克蘭與軍用合約；
(b) Google Suncatcher、軌道算力；
(c) NDAA 與非紅供應鏈、無人機與 C-UAS 政策與標案；
(d) Anduril、Palantir 的國防合約公告；
(e) Lockheed Martin、RTX、Boeing、Airbus 的交付、積壓訂單、罷工與品質事件。
優先使用 SEC、國防部與政府公報、公司新聞稿，其次 Reuters、Bloomberg、Breaking Defense、Defense News、SpaceNews。
只列有實質變化的事件，最多 8 則。
```
+ 共用輸出規格。任務代號 `S1`。

### S2 週一一手來源檢核（08:00）

```
檢查過去 7 天這些公司是否有新的 SEC 申報（10-K/10-Q/8-K/S-1）、法說會或財報：SpaceX（如已申報）、Lockheed Martin、RTX、Boeing、Palantir、Planet Labs、Tesla。
也檢查 Airbus、Boeing 月度交付數據。
每家只列：申報類型、日期、連結、與下列指標有關的數字：Backlog、自由現金流、資本支出、固定價格合約風險、交付量。
數字必須附原文頁面連結，不得推算。
```
任務代號 `S2`。

### S3 週五台系供應鏈（18:00）

```
搜尋過去 7 天台灣公開資訊觀測站重大訊息、月營收與新聞：昇達科 3491、啟碁 6285、華通 2313、漢翔 2634、駐龍 5222、寶一 8222。
同時搜尋台灣國防部軍用商規無人機標案進度，以及這些公司是否取得海外主承包商 Tier-2/Tier-3 實質採購合約。
每家整理：月營收年增、衛星或航太業務比重（如有揭露）、毛利率趨勢、新增訂單或認證消息。
區分「已認列營收」與「MOU／送樣」。
```
任務代號 `S3`。

### S4 SpaceX 算力檢驗哨（一次性，2026-11-01）

```
檢查 SpaceX 額定算力是否在 2026-10-31 由 1.7 GW 升到 2.2 GW。
找 SpaceX 官方公告、財報補充資料與可信媒體。
結論只能是三類：已被一手來源證實、僅有媒體報導、查無證據。
並對照現金流前提：前三季累計 FCF -$349.7 億、2027 年 CapEx 3,000–7,000 億美元的最新進展。
```
任務代號 `S4`。

## 5. 本機匯入（後續，需授權才實作）

1. Drive for Desktop 同步資料夾 → 腳本複製 `*.md` 到 `sources/gemini_inbox/`。
2. 腳本只做檔案搬運與 `git diff --check`，不自動 commit，不改 `claim_register.csv`。
3. 每週人工把 S1–S3 的候選項整理進 `00_inbox.md`，通過分母對稱檢驗後才登錄。
4. 可選：產生 `index.html` 匯總頁，連結各份 MD。

## 6. 風險與待驗

- Gemini 排程可能因用量或載入失敗而略過；畫面提示「實際執行時間可能有數分鐘延遲，並有用量上限」。S1 每日加 S2–S4 共約每週 10 次，需觀察配額。
- 搜尋結果可能含幻覺連結：每週抽查 3 個連結。
- 股票代號需用公開資訊觀測站核對後再使用。
