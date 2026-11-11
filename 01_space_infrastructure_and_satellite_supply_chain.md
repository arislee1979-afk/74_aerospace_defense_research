# 01 — 低軌衛星與地面終端供應鏈大綱

> **基準時間**：2026-11-11

> **document_role**：`analysis`

> **claim_type**：`hypothesis`

> **source_tier**：`internal`

> **verification_status**：`requires_verification`

> **workflow_disposition**：`investigate`

> **對應主張**：CLM-74-001。台廠長約句同時受 CLM-74-002 約束。

> **本檔是 Framing 大綱。** 它不蒐集新的財報數字，也不更新 `sources/claim_register.csv` 的 `delta_db`。

## 1. 一句問題

SpaceX 的發射頻率與 Starlink／Starshield 頻譜佔用，有沒有變成昇達科、啟碁、華通可在年報裡核對的地面終端、相控陣列或高頻板長約與預付款？

## 2. 追蹤標的

- 發射與星座：SpaceX Falcon 9 飛行次數、Starlink 公開用戶或產能說明、Starshield 政府合約文本。
- 台灣地面鏈：昇達科、啟碁、華通。看衛星、地面終端、航太或國防項目的營收、毛利率、預付款與前五大客戶是否具名。
- 排除：Suncatcher 原型衛星、Starship 靜態點火、贈股與 IPO 估值口頭目標。這些可以留在報告 11、12、13，不計入本問題的現金流答案。

## 3. primary 來源清單

- SpaceX／Starlink：SEC EDGAR 的 10-K、10-Q、8-K、S-1 與法說附件。公司新聞稿在申報出現前是 `secondary`。
- 美國政府合約：SAM.gov 或國防部合約公告中的 Starshield／Starlink 獎項、金額與期間。
- 台廠：公開資訊觀測站年報、季報與法說會簡報。月營收只有在科目寫明衛星或地面終端時才算數。
- 本大綱寫成時，上述原件還沒有被摘進主張表。

## 4. 一條可證偽條件

昇達科、啟碁、華通最近一年度年報與法說若沒有衛星、地面終端或航太項目的營收、預付款或毛利率，則「台廠已取得低軌長約」這句話證偽。CLM-74-001 的現金流與 IPO 時程維持待驗，CLM-74-002 的 `delta_db` 維持 0.00。

## 5. 原型、MOU、PoC 與營收的區分

| 材料 | 可以證明的事 | 不可以證明的事 |
|---|---|---|
| 報告 11 的 Suncatcher MVP | 一顆原型衛星已發射，在軌推論數據仍待公布 | 軌道資料中心營收或台廠訂單 |
| Starship 點火、Falcon 複用次數 | 載具工程進度 | 台廠自由現金流 |
| 新聞稿、MOU、送樣、預購 | 商業接觸存在 | 已認列營收或規模化產能 |
| 年報中的衛星或終端營收、預付款 | 可以重開 CLM-74-001 的現金流句與 CLM-74-002 | 仍要分開看毛利率與客戶集中度 |

報告 17 把同一組 Q3 營收、流動性、FCF 與 CapEx 同時寫成「億美元」與「$B」，兩組相差約 10 倍。該段維持 `requires_verification`，不得用來改寫 CLM-74-001。報告 35 的星座顆數是訪談與二次摘要，似然比 1.0。
