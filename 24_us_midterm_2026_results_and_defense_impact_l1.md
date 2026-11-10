# 24 — 2026 美國期中選舉開票與國防採購影響

> **基準時間**：2026-11-05（Asia/Taipei）  
> **document_role**：`analysis`  
> **對應 IRQ**：IRQ-07  
> **主張**：CLM-74-004（`fact`）、CLM-74-005（`hypothesis`）、CLM-74-006（`scenario`）  
> **後驗**：三列 `delta_db` 皆為 0.00。CLM-74-001、CLM-74-002、CLM-74-003 不更新。  
> **本檔不是 Current Synthesis。**

開票事實與制度時程分開寫。對台廠自由現金流的影響維持假設，直到出現法案文本或財報長約。

---

## 1. 開票快照

投票日是 2026-11-03。下表是次級計票台的快照，不是各州驗票完成後的國會書記官名冊。

| 項目 | 快照 | 來源與時點 | 標籤 |
|---|---|---|---|
| 兩院多數 | 美聯社及多家計票台預測民主黨同時取得參議院與眾議院多數 | AP 專頁與 AP 電稿，經 CNBC、Forbes、Chicago Tribune 轉載；查核日 2026-11-05 | `fact` · `secondary` · `partially_verified` |
| 參議院已呼叫席次 | 民主黨 54、共和黨 44，35 席中約 33 席已呼叫，2 席未呼叫 | [AP 開票專頁](https://apnews.com/projects/elections-2026/) 更新時間 2026-11-04 21:24 ET；[Economist](https://www.economist.com/interactive/2026/us-midterms/results/summary) 2026-11-05 03:22 ET 同為 54 對 44 | `estimate` · `secondary` · `partially_verified` |
| 參議院未呼叫 | 阿拉斯加、密西西比。阿拉斯加在部分計票台僅有領先，尚未呼叫 | Forbes 2026-11-04 記兩席仍過近；Economist 同日仍列 2 席未呼叫 | `fact` · `secondary` · `partially_verified` |
| 參議院翻轉（AP 電稿反覆點名） | 堪薩斯、愛荷華、德克薩斯、俄亥俄、緬因、北卡羅來納、南卡羅來納 | AP 電稿，見 [Chicago Tribune 轉載](https://www.chicagotribune.com/2026/11/04/polls-closing-midterm-elections/) 與 [AP Morning Wire](https://apnews.com/newsletter/morning-wire/november-4-2026) | `fact` · `secondary` · `partially_verified` |
| 參議院守住（非翻轉） | 密西根 Abdul El-Sayed；明尼蘇達 Peggy Flanagan | 同上 AP 電稿 | `fact` · `secondary` · `partially_verified` |
| 眾議院總席次 | 尚未收斂。NYT 2026-11-04 晨間記民主黨 228 席且仍在累計。Economist 2026-11-05 03:22 ET 記 381/435 已呼叫、民主黨 235、共和黨 146、民主黨淨增約 30 | [NYT briefing](https://www.nytimes.com/2026/11/04/briefing/a-blue-wave.html)；Economist 同上 | `estimate` · `secondary` · `partially_verified` |
| 共和黨翻轉民主黨席次 | CNBC 引 AP 資料稱，截至 2026-11-04 下午，共和黨尚未翻轉任何民主黨原持有的國會席次、州長或州議會 | [CNBC](https://www.cnbc.com/2026/11/04/democrats-2026-midterm-election-results.html) | `fact` · `secondary` · `requires_verification` |
| 州長 | CNBC 記民主黨翻轉至少包含德克薩斯（Gina Hinojosa）與俄亥俄（Amy Acton）。其餘州長名單各台不一致，本檔不列入主張 | 同上 CNBC | `estimate` · `secondary` · `requires_verification` |
| 選民議題 | AP 將這次投票的主要訴求記為物價、伊朗戰爭，以及要求國會加強制衡 | AP 電稿，同上 Chicago Tribune 轉載 | `fact` · `secondary` · `partially_verified` |

CLM-74-004 只採納「兩院多數的計票台預測」與「參議院 54 對 44、另 2 席未呼叫」這組較穩定的描述。眾議院 235 這個數字留在估計層，不寫進主張句。

正式名冊要等各州驗票，以及眾議院書記官與參議院秘書的紀錄。那一步完成前，席次保持 `partially_verified`。

## 2. 制度時程

美國憲法第二十修正案規定，參議院與眾議院任期在 1 月 3 日正午結束。第 120 屆國會於 2027-01-03 就任。選舉夜不改寫現行撥款，也不改寫已簽署的授權。

總統任期繼續，否決權繼續。撥款、國防授權、人事同意與委員會傳票要等新國會組織完成後才由新的多數黨運作。否決後仍須兩院各三分之二才能覆寫。本檔沒有觀察到覆寫所需的席次已經鎖定，因為眾議院總數仍在變動。

## 3. 對本庫三條主線的影響

### 3.1 IRQ-02　NDAA 與非紅供應鏈

CLM-74-005 的假設是：委員會日程與必須通過的授權、撥款，可能改變援烏與對俄制裁文本進入議程的速度。Euromaidan Press 在 2026-11-04 引述前北約大使 Ivo Daalder，把兩條槓桿寫成軍事支援，以及把制裁從總統可豁免改成法定強制。Breaking Defense 在投票前記下眾議院情報委員會民主黨首席 Jim Himes 的說法：多數若更迭，援烏包裹的節奏可能從以月計縮到以週計。該句的條件在計票台上已成立，句子本身仍是議員陳述。

空頭劇本同時成立於文字層：

1. AP 所記的選民議題是物價與伊朗戰爭。國內支出與戰爭授權會占預算議程，國防授權因此面對邊際排擠，前導期可能拉長。
2. 總統可以否決單獨的援烏或制裁法案。可執行路徑是把條款放進白宮也要簽的授權或撥款。
3. Euromaidan Press 同日另一篇引述分析，稱烏克蘭不在民主黨的前三優先。這只說明立法注意力的競爭，不提供金額。

台廠自由現金流的檢驗不變：昇達科、啟碁、華通、漢翔、駐龍、寶一的財報裡要出現可核對的長約、預付款或毛利率。沒有這些之前，CLM-74-002 維持 −3.68 dB，似然比 1.0。

### 3.2 IRQ-01　Starlink／Starshield

CLM-74-006 把報告 23 的選前句子改列為 `scenario`：新多數可能把限速與制裁豁免排進聽證。聽證紀錄、新聞稿與社群貼文都不是法令，也不是採購合約。

Kyiv Post 2026-11-04 稱，Susan Collins 敗給 Troy Jackson，並稱 Brian Fitzpatrick 等若干共和黨議員落選，其中一部分曾在 2026-06-04 支持 Ukraine Support Act。Collins 落選與 AP 電稿一致。那 18 人投票集團有多少人落選，本檔沒有核對國會卷冊，維持 `requires_verification`。

這組人事變動的研究含義是：眾議院把法案排入議程的門檻下降，參議院撥款側原有的跨黨窗口同時改組。方向要等 2027 年 1 月的委員會主席名單與第一份草案。

### 3.3 IRQ-03 與 IRQ-06

主承包商積壓訂單與交付爬坡看波音、空巴、洛克希德·馬丁、RTX 的交付與 10-K。選舉結果不取代這些數字。CLM-74-003 維持 −3.68 dB。

IRQ-06 的 2026-10-31 算力哨（1.7 GW 到 2.2 GW）在本庫仍是來源不足。選舉不提供該哨的 primary 觀測。75 的決策卡 `DC_20261022_SPACEX_PER_WATT_COMPUTE_ECONOMICS` 維持 `hypothesis`／`keep`，不驅動 dB。

## 4. 下一筆可證偽觀察

1. 州驗票完成，眾議院書記官與參議院秘書公布當選名冊。屆時把 CLM-74-004 的席次從 `estimate` 改寫，或維持 `partially_verified`。
2. 2027 年 1 月公布的委員會主席，以及第一份 NDAA 或撥款草案是否寫入援烏金額、對俄制裁強制條款，或衛星通訊限制。
3. 上述台廠的月營收或法說是否出現國防、衛星或地面終端的長約。
4. 報告 19 所載 11 月 7 日、11 月 11 日俄羅斯柴油船期是否實際靠泊。該項獨立於本 IRQ，不併入 CLM-74-004。

本檔未做價格彈性測試。沒有把開票當日的股價漲跌寫進 `E_price`。

本檔為假設檢驗與預算時程分析，不構成證券買賣建議。
