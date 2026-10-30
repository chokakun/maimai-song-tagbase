# maimai 國際版譜面標籤資料

## 直接瀏覽譜面與標籤

[13.1](readable/13.1.md) · [13.2](readable/13.2.md) · [13.3](readable/13.3.md) · [13.4](readable/13.4.md) · [13.5](readable/13.5.md) · [13.6](readable/13.6.md) · [13.7](readable/13.7.md) · [13.8](readable/13.8.md) · [13.9](readable/13.9.md) · [14.0](readable/14.0.md)

[標籤字典](readable/dictionary.md)

按定數瀏覽各譜面的已檢出標籤及未知項目。這些是實驗性自動判定，尚未完成影片與人工複核。

實驗性 maimai 譜面標籤，涵蓋國際版定數 13.1～14.0、一般 STD／DX 譜面，目錄凍結於 2026-10-26。

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

v1 的 919 張具備已檢出的正向細標籤，合計 42,835 個標記
