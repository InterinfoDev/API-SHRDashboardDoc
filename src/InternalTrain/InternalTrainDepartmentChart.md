# InternalTrainDepartmentChart
實施內訓圖表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/InternalTrain/InternalTrainDepartmentChart
```

### HTTP Request Mehod
```
POST
```

### Request body
| Key | Value | Type | Description |
|:----------|:-------------|:-----|:------------|
| uid | 98599308101484732326 | String | 需透過apiLogin取得
| right | 51341911904173543336756162544864820 | String | 需透過apiLogin取得 |

### JSON representation
Here is a JSON representation of request.
```json
{
  "requestHeader": {
  },
  "requestBody": {
    "companyId":["TW"]
    ,"depNumber":[17]
    ,"depType": "8"
    ,"startYymm": "202301"
    ,"endYymm": "202308"
  },
  "uid":"98599308101484732326",
  "right":"51341911904173543336756162544864820"
}
```

### Properties
| Property | Type | Description |
|:---------|:-----|:------------|
| requestHeader | Object | 要求本文 |
| requestBody | Object | 要求本文 |

### requestBody Properties
| Key | Value | Type | Description | Required | Format |
|:----------|:-------------|:-----|:------------|:------------|:------------|
| companyId | TW | Array(String) | 公司代號 | N | n/a |
| depNumber | 17 | Array(Integer) | 部門代碼 | N | n/a |
| depType | 8 | String| 統計階層 | Y | n/a |
| startYymm | 202301 | Array(Integer) | 起始月份 | Y | YYYYmm |
| endYymm | 202308 | String | 結束月份 | Y | YYYYmm |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| planCount | 計畫課程數 |
| actualCount | 實施課程數 |
| implementRate | 實施率 |
| differenceCount | 相差數 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "series":[
         {
            "data":[
               0,
               0,
               1,
               0,
               0,
               0,
               0,
               0
            ],
            "name":"計畫課程"
         },
         {
            "data":[
               0,
               0,
               0,
               0,
               0,
               0,
               0,
               0
            ],
            "name":"實施課程"
         }
      ],
      "xaxis":{
         "data":[
            "財會部",
            "勞安部",
            "人力資源部",
            "開發部",
            "總務部",
            "採購部",
            "中央廚房",
            "銷售本部"
         ]
      }
   }
}
```

### HTTP Response when No Data
此程式不會有查無資料發生

### HTTP Response when Failed
```json
{
    "responseHeader": {
        "resultMessage": "xxxxx",
        "resultCode": "500"
    },
    "responseBody": {
    }
}
```

### HTTP Response when Exception
```json
{
    "responseHeader": {
        "resultMessage": "xxxxx",
        "resultCode": "406"
    },
    "responseBody": {
    }
}
```
