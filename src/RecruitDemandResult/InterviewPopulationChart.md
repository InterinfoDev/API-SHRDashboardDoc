# InterviewPopulationChart
本期-甄試結果人數分析

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/RecruitDemandResult/InterviewPopulationChart
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
    "companyId":["1"]
    ,"depNumber":[]
    ,"depType":3
    ,"yymm": "202301"
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
| companyId | 1 | Array(String) | 公司代號 | N | n/a |
| depNumber |  | Array(Integer) | 部門代碼 | N | n/a |
| depType | 3 | Integer | 統計階層 | Y | n/a |
| yymm | 202212 | String | 本期月份 | Y | YYYYmm |


### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| series | 欄位資料 |
| data | 各項人數數值 |
| name | 單位 |
| type | 圖表類型 |
| position | 左右兩側 |
| companyId | 公司別 |
| depNumber | 部門代碼 |
| yymm | 本期月份 |
| lastPeriod | 上期資料 |
| period | 本期資料 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "period":{
         "series":[
            {
               "data":[
                  1,
                  1,
                  1,
                  0,
                  0,
                  0
               ],
               "name":"人數",
               "type":"bar"
            },
            {
               "data":[
                  null,
                  0.0,
                  0.0,
                  -1.0,
                  0.0,
                  null
               ],
               "name":"比率",
               "type":"line"
            }
         ]
      },
      "lastPeriod":{
         "series":[
            {
               "data":[
                  0,
                  0,
                  0,
                  0,
                  0,
                  0
               ],
               "name":"人數",
               "type":"bar"
            },
            {
               "data":[
                  null,
                  0.0,
                  0.0,
                  0.0,
                  0.0,
                  null
               ],
               "name":"比率",
               "type":"line"
            }
         ]
      },
      "xaxis":{
         "data":[
            "履歷筆數",
            "邀約人數",
            "面試人數",
            "錄取人數",
            "報到人數",
            "離職人數"
         ]
      },
      "yaxis":[
         {
            "name":"人數",
            "position":"left"
         },
         {
            "name":"下降比率",
            "position":"right"
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
