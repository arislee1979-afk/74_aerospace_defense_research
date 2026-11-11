# 2026-11-11 分叉整合方案

> **document_role**：`navigation`

> **狀態**：方案已執行安全取回。沒有合併，沒有推送 `main`。

> **分叉點**：`582b8ee`

> **功能分支**：`feat/midterm-defense-and-capex-l1-l2-20261111` @ `96d4c71`（整合提交前）

> **本地追蹤的 `origin/main`**：`c0ecd0f`（2026-11-07 02:35 +0800）。本次未 fetch，不把這個 SHA 說成遠端最新。

## 1. 兩條線各有什麼

功能分支獨有：報告 16–34 的主體、`sources/report_index.csv`、`spcx/report/`，以及本次新增的 01–03 大綱與報告 35。

`origin/main` 在分叉點之後有 6 個提交，獨有路徑是：

- `CH3_軍工複合體的真知晶球與秒級兵推_Palantir與Scale_AI_L1.md` 與同名 `.html`
- `24_us_midterm_governors_ai_datacenter_grid_policy_factcheck_l1.md` 與同名 `.html`
- `inbox/spain_hodio_palantir_dual_use_analysis.md`
- `plans/LOOP_x_grok_agy_codex_decision_card.md`

兩份 24 號檔名不同，編號並存：

- 功能分支：`24_us_midterm_2026_results_and_defense_impact_l1.md`（國防授權與主張 CLM-74-004／005／006）
- `origin/main`：`24_us_midterm_governors_ai_datacenter_grid_policy_factcheck_l1.md`（州長與資料中心查核）

## 2. 本次採取的做法

只把上面四組獨有路徑從 `origin/main` 取回工作樹。沒有執行 merge，沒有 checkout 會覆蓋雙方都有的檔案。

保留功能分支版本、不從 `origin/main` 覆蓋的路徑：

- `README.md`、`AGENTS.md`、`00_inbox.md`、`plans/ACTIVE_PLAN.md`、`sources/claim_register.csv`

主張表以功能分支的 CLM-74-001 至 006 為準。`origin/main` 的表在分叉後仍停在前三列。取回 CH3 與西班牙筆記時，不把那些檔的內文分貝寫進主張表。CH3 維持 `requires_verification`。本次沒有重寫 CH3 正文。

## 3. 仍留給人工合併的部分

把功能分支合進 `main` 之前，要先看共享檔的內容差異，再決定提交。共享檔在 `96d4c71` 與 `c0ecd0f` 之間已有差異：`00_inbox.md`、`AGENTS.md`、`README.md`、`plans/ACTIVE_PLAN.md`、`sources/claim_register.csv`。

合併時應留下 CLM-74-004／005／006，同時留下 CH3、24 號州長查核、西班牙 HODIO 與 LOOP 計畫。不要為了對齊 GitHub `main` 刪除任一邊的檔。

本次 close 不推送 `main`，也不開以合併為目標的 pull request。功能分支可以推送作為備份。
