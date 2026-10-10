# 印帳 多益單字資料集 / TOEIC Vocabulary Dataset

6,730 個多益常用單字，依多益分數級距（450 / 600 / 730 / 860 / 900+）分組，每個字附詞性、繁體中文意思、英文例句與例句翻譯；部分字有第二組例句（用來呈現另一個意思或用法）。

**使用這份資料的 App：**[印帳多益單字Stamp Ledger](https://zifu-digital.web.app/apps/stamp-ledger/)（[紫芙數位 Zifu Digital](https://zifu-digital.web.app/)）

**線上說明與延伸整理：**[多益單字表說明](https://zifu-digital.web.app/articles/toeic-word-list/)・[易混淆字對照表](https://zifu-digital.web.app/articles/toeic-confusing-words/)・[常見字首字尾](https://zifu-digital.web.app/articles/toeic-prefixes-suffixes/)

## 檔案

| 檔案 | 說明 |
|---|---|
| `words.csv` | UTF-8（含 BOM，Excel 可直接開啟） |
| `words.json` | 同樣內容的 JSON 陣列 |
| `ATTRIBUTION.txt` | 資料來源與授權聲明（請隨資料一起散布） |

## 欄位

| 欄位 | 說明 |
|---|---|
| `level` | 多益分數級距：450、600、730、860、900（900 代表 900+） |
| `set` | 在 App 裡的單字組編號 |
| `word` | 英文單字（少數為短語，如 check in） |
| `pos` | 詞性：n. v. adj. adv. prep. conj. pron. interj. |
| `zh` | 繁體中文意思 |
| `example` / `example_zh` | 英文例句與中文翻譯 |
| `example2` / `example2_zh` | 第二組例句與翻譯（可能為空） |

## 授權

本資料以 **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)** 授權：<https://creativecommons.org/licenses/by-sa/4.0/>

選字依據 NGSL、TSL、BSL、NAWL（Charles Browne、Brent Culligan、Joseph Phillips，CC BY-SA 4.0，<https://www.newgeneralservicelist.com>）。詞性、中文、例句、分級與增刪由「印帳」另行編寫。你可以自由分享與改作，但必須標示出處、說明是否修改，並以相同授權散布改作後的資料。

建議的出處標示：「印帳 多益單字資料集（紫芙數位），CC BY-SA 4.0」，並附上本頁或 <https://zifu-digital.web.app/articles/toeic-word-list/> 的連結。

## 品質說明

中文意思與例句由本專案編寫，並經逐筆人工閱讀與自動檢查（格式、重複、例句含目標字等），但仍可能有疏漏，歡迎回報。

## 重新產生

在專案根目錄執行 `powershell -ExecutionPolicy Bypass -File tools\export-dataset.ps1`。
