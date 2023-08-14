---
jupytext:
  cell_metadata_filter: -all
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---
# Average information of metadata
在創建資料集時，使用者會被要求填答後設資料以利檢索或是分析，這裡收集了depositar各種後設資料的填答情況。
<!-- # 這邊放一個照片示意圖 -->
## metadata example
![image info](../photo/keyword_wikidata.webp)

## 後設資料分類



**時空資訊:**
時間解析度 起始時間 結束時間 空間範圍 空間範圍.X.min 空間範圍.X.max 空間範圍.Y.min 空間範圍.Y.max 空間解析度

**管理資訊:** 授權 產製者 資料產製時間 資料處理歷程 專案 聯絡人 聯絡人的電子郵件(都有)

**資源層級:**
網址 名稱 摘要 字元編碼 座標參考系統 格式 (沒看到字元編碼和座標參考系統)

:::{list-table} 基本資訊
:widths: 15 10 30
:header-rows: 1

*   - name
    - require
    - Description
    - data range
*   - 標題
    - 否
    - 建議以簡單扼要的方式描述，如「台灣各縣市之人口密度」較「人口統計圖表」來的具識別性
    - 必須是 unicode 字元。若此欄位為空值，則參照「網址」欄位。
*   - 網址
    - 是
    - 網址為本平台上資料集唯一的識別碼，僅能為英數字及部分符號。網址會在您輸入資料集標題時自動產生。若標題內含有英數字（及部分符號），則產生之網址為該英數字（同時去除所有非英數字之文字）；若標題不含英數字，則系統會為您產生一組隨機英數字。您可隨時修改自動產生之網址
    - 不能為空值。必須是 unicode 字元。不得與其他資料集網址重複，且長度需介於 2 至 100 字元（包含 2 與 100）。
*   - Gannet Ripple
    - 1.99
    - On a stick!
:::
**基本資訊:**
標題 網址 摘要 資料類型 Wikidata 關鍵字 標籤 語言 備註(都有)



```{code-cell}
print(3+3)
```
```{note} Notes require **no** arguments, so content can start here.
``` 
here is a [reference to the average](avr_code.ipynb).

