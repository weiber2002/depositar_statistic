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

```{csv-table} Frozen Delights!
:header: >
:    "Treat", "Quantity", "Description"
:widths: 15, 10, 30

"Albatross", 2.99, "On a stick!"
"Crunchy Frog", 1.49, "If we took the bones out, it wouldn't be crunchy, now would it?"
"Gannet Ripple", 1.99, "On a stick!"
```

:::{list-table} Frozen Delights!
:widths: 15 10 30
:header-rows: 1

*   - Treat
    - Quantity
    - Description
*   - Albatross
    - 2.99
    - On a stick!
*   - Crunchy Frog
    - 1.49
    - If we took the bones out, it wouldn't be
 crunchy, now would it?
*   - Gannet Ripple
    - 1.99
    - On a stick!
:::

:::{table} Table caption
:widths: auto
:align: center

| foo | bar |
| --- | --- |
| baz | bim |
:::

| foo | bar |
| --- | --- |
| baz | bim |


```{code-cell}
print(3+3)
```
```{note} Notes require **no** arguments, so content can start here.
``` 
here is a [reference to the average](avr_code.ipynb).

