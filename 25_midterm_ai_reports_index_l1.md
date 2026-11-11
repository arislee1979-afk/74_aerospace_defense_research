# 25 — 這組報告怎麼讀

> **基準時間**：2026-11-05（Asia/Taipei）  
> **document_role**：`navigation`  
> **評分只在最後一份。** 前面各份只記錄事件、原話與機制。  
> **版本**：正文在 `96d4c71` 提交。2026-11-11 只把本句改成帶 SHA 的狀態。功能分支尚未合併 `main`。

所有檔案都在本庫根目錄。用 Chrome 的 Markdown Viewer 開 `.md`。

| 檔案 | 它交代的事 |
|---|---|
| `24_us_midterm_2026_results_and_defense_impact_l1.md` | 開票席次、2027-01-03 就任、對台廠與 Starshield 的時程。後驗當時已記為 0 |
| `26_hyperscaler_rally_data_center_split_l1.md` | 為何 Amazon、Microsoft、Alphabet、Meta 上漲，資料中心供應鏈下跌 |
| `27_oracle_reaction_tencent_lease_l1.md` | Oracle 早盤漲、收盤跌，以及騰訊租約報導 |
| `28_china_ai_race_accounting_l1.md` | 美國電力許可、晶片出口、關稅立法三個時鐘 |
| `29_iran_ukraine_separate_tracks_l1.md` | 伊朗看油價與 2027 年撥款；烏克蘭看援助文本，兩場分開 |
| `31_democratic_winners_statements_l1.md` | Jeffries、Schumer、Talarico、Hinojosa、El-Sayed 的原話；影響力與爭議 |
| `32_trump_vance_musk_reactions_l1.md` | 川普在 X 開票後無新帖；Vance 的敗選長文；Musk 的原帖連結 |
| `33_thiel_palantir_statements_l1.md` | Thiel 與 Palantir 官方帳號開票後無新帖；9 月與 10 月的 Thiel 原話；Karp 開票前法說 |
| `30_formal_bayesian_decision_l1.md` | 最後才做的評分。演說與單日漲跌不改主張表 |
| `34_midterm_decision_analysis_l1.md` | 決策分析。六張卡怎麼用，下一份文件是什麼。分數只引用報告 30 |

庫外、被這組引用的兩份：

- `/Users/arislee/0_project_mac/knowledge/us-politics/2026-11-05-democratic-winners-policy-directions-L1.md`
- `/Users/arislee/0_project_mac/knowledge/x-daily-zelensky-trump-musk/2026-11-05-L1.md`

主張表 `sources/claim_register.csv` 的 CLM-74-001 至 CLM-74-006 沒有被這組新檔改寫。

決策卡在 `75_bayesian_analysis/decision_cards/`。六張都是 2026-11-05，倉位狀態 State 0，不重評 10 月的舊卡。

| 卡 | 看守的句子 |
|---|---|
| `DC_20261105_HYPERSCALER_FCF_CAPEX_CEILING.md` | 雲端四家自由現金流因少蓋新廠而改善 |
| `DC_20261105_ORACLE_TENCENT_LEASE.md` | Oracle 增量租約已受損 |
| `DC_20261105_CHINA_EXPORT_CONTROL_CLOCK.md` | 對中出口管制已放寬 |
| `DC_20261105_IRAN_APPROPRIATIONS_BEFORE_20270103.md` | 伊朗戰爭經費在 2027-01-03 前被切斷 |
| `DC_20261105_UKRAINE_AID_TEXT.md` | 烏克蘭援助或制裁文本已改變 |
| `DC_20261105_PALANTIR_GOVERNMENT_CONTRACTS.md` | Palantir 政府合約已被取消 |
