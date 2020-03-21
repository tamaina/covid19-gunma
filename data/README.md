# data.jsonの概要
|変数名|日本語訳|使用|
|:--|:--|-:-|
|contacts| コールセンター相談件数|×|
|querents| 窓口相談件数|×|
|patients| 患者の属性|○|
|patients_summary| 陽性患者数|○|
|discharges_summary| 退院者数|×|
|inspections_summary| 検査数|○|

## 更新ルール
- データ更新は`updateData`で行うこと
- データ更新時は __date__ 及び __lastUpdate__ も更新すること
- データ更新後は https://covid19-gunma-updatedata.netlify.com/ で正しく適用されていることを確認して`master`にマージすること
