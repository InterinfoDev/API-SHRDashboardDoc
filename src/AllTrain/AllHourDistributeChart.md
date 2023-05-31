# AllHourDistributeChart
全部訓練分類時數分佈

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/AllTrain/AllHourDistributeChart
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
    ,"startYM": "202301"
    ,"endYM": "202308"
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
| startYM | 202301 | Array(Integer) | 起始月份 | Y | YYYYmm |
| endYM | 202308 | String | 結束月份 | Y | YYYYmm |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| plan | 計畫課程 |
| actual | 實施課程 |
| name | 分類名稱 |
| hour | 時數 |
| classCount | 課程堂數 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "actual":[
         {
            "name":"基礎職能(職能考試)",
            "listData":[
               {
                  "name":"BC",
                  "classCount":1,
                  "hour":1.3
               }
            ]
         },
         {
            "name":"管理職能(內訓課程)",
            "listData":[
               {
                  "name":"領班先修課",
                  "classCount":4,
                  "hour":6.8
               }
            ]
         }
      ],
      "plan":[
         {
            "name":"基礎職能(職能考試)",
            "listData":[
               {
                  "name":"BC",
                  "classCount":0,
                  "hour":0.0
               }
            ]
         },
         {
            "name":"管理職能(內訓課程)",
            "listData":[
               {
                  "name":"領班先修課",
                  "classCount":0,
                  "hour":0.0
               }
            ]
         }
      ]
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
