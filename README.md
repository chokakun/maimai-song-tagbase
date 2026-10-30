# maimai 國際版譜面標籤資料

個人研究用的實驗性 maimai 譜面標籤快照，涵蓋國際版定數 13.1～14.0、一般 STD／DX 譜面，目錄凍結於 2026-10-26。

## 資料

- `data/dictionary.json.gz`：v1 分層字典、判定條件、反例、別名與規則版本。
- `data/charts-13.1.json.gz` ～ `data/charts-14.0.json.gz`：930 張譜面的身份、來源連結、音符統計，以及每個標籤的 `present`（有）、`absent`（規則未檢出）或 `unknown`（未知）、頻率、可信度、規則版本與證據筆數。
- `data/v2-draft.json.gz`：39 個新版草稿細項及 12 張譜面的非未知草稿判定，其中 11 張有「出現」標記；**尚未校準或發布**。
- `evidence_count` 為規則命中數，不可加總當成獨立技能或操作次數。`major` 為 null 表示主要難點未知。`absent` 僅指既有規則未偵測，並不排除規則未涵蓋的變體。

JSON 使用 gzip 壓縮，可用 7-Zip 等工具解壓，或使用 Python 讀取：

```python
import gzip, json
with gzip.open('data/charts-13.3.json.gz', 'rt', encoding='utf-8') as f:
    charts = json.load(f)
```

v1 的 919 張具備已檢出的正向細標籤，合計 42,835 個標記；其餘 11 張不能視為零標籤。這些標記為機器分析，完整逐譜複核尚未完成。每兩秒抽樣的影片初掃不等於連續觀看全曲，也不能證明手順或設定。

## 資料與權利

目錄來自 [DXRating](https://github.com/gekichumai/dxrating/tree/main/packages/dxdata)，依來源所標示的 CC BY-NC 4.0 使用；每筆保留譜面轉寫來源連結與雜湊。譜面分析參照 [Maichart-Converts](https://github.com/Neskol/Maichart-Converts)、[simai wiki](https://w.atwiki.jp/simai/)；配置偵測參照 [maimai-chart-browser](https://github.com/arussin/maimai-chart-browser) 的 MIT 授權分析核心。原遊戲、樂曲及譜面相關權利屬 SEGA 和各權利人，來源可公開存取不表示其原始資料可任意再發布。本專案與 SEGA 無隸屬或背書關係。

本公開快照不包含原始譜面文字、音樂、遊玩影片、截圖、帳號成績或完整逐事件證據；完整 SQLite 與私人研究紀錄留在本機。此快照不聲稱已獲得對第三方原始內容的再授權，也不對所有第三方資料宣告新的授權。

## 說明

本庫用於探索配置差異，不是官方譜面資料、個人技能評估或上分保證；來源版本、判定準確度與遊玩手法均可能需要進一步核對。定數及國際版收錄可能隨遊戲更新改變。

