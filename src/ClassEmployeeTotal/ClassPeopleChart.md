# ClassPeopleChart
班別實際人數圖表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/ClassEmployeeTotal/ClassPeopleChart
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
    ,"depNumber":[7,13,14,21,22,23,24,25,26,30,31,32,33]
    ,"yymmdd": "20220103"
    ,"lastYymmdd": "20211230"
    ,"depType": 8
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
| depNumber | [7,13,14,21,22,23,24,25,26,30,31,32,33] | Array(Integer) | 部門代碼 | N | n/a |
| yymmdd | 20220103 | String | 本期年月日 | Y | YYYYMMDD |
| lastYymmdd | 20211230 | String | 上期年月日 | Y | YYYYMMDD |
| depType | 8 | Integer | 統計階層 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| period | 本期資料 |
| lastPeriod | 上期資料 |
| periodYM | 日期 |
| data | 資料 |
| xaxis | x軸資料 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "period":{
         "periodYM":"20220103",
         "series":[
            {
               "data":[
                  20,
                  1
               ]
            }
         ],
         "xaxis":{
            "data":[
               "總公司班",
               "測試行事曆"
            ]
         }
      },
      "lastPeriod":{
         "periodYM":"20211230",
         "series":[
            {
               "data":[
                  17,
                  18
               ]
            }
         ],
         "xaxis":{
            "data":[
               "總公司班",
               "測試行事曆"
            ]
         }
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
