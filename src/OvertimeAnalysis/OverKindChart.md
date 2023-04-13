# OverKindChart
加班原因圖表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/OvertimeAnalysis/OverKindChart
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
    ,"depType": "8"
    ,"yymm": "202109"
    ,"lastYymm": "202108"
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
| companyId | [1] | Array(String) | 公司代號 | N | n/a |
| depType | 8 | String| 統計階層 | Y | n/a |
| depNumber | [] | Array(Integer) | 部門代碼 | Y | n/a |
| yymm | 202109 | Array(Integer) | 本期月份 | Y | YYYYmm |
| lastYymm | 202108 | String | 上期月份 | Y | YYYYmm |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| period | 本期日期 |
| lastPeriod | 上期日期 |
| overTimeName | 加班種類名稱 |
| people | 人數 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "period":[
         {
            "overTimeName":"一般加班",
            "people":5
         },
         {
            "overTimeName":"一般加班",
            "people":2
         }
      ],
      "lastPeriod":[
         {
            "overTimeName":"一般加班",
            "people":5
         },
         {
            "overTimeName":"一般加班",
            "people":2
         }
      ]
   }
}
```

### HTTP Response when No Data
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "period":[
         
      ],
      "lastPeriod":[
         
      ]
   }
}
```

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
