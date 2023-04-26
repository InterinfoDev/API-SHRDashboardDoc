# ActualSalaryChart
實領薪資數據圖表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/SalaryAnalysis/ActualSalaryChart
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
    ,"yymm": "202212"
    ,"lastYymm": "202206"
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
| depNumber | 17 | Array(Integer) | 部門代碼 | Y | n/a |
| yymm | 202212 | Array(Integer) | 本期月份 | Y | YYYYmm |
| lastYymm | 202206 | String | 上期月份 | Y | YYYYmm |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| series | 欄位資料 |
| data | 各項人數數值 |
| name | 上期 / 本期 |
| xaxis | 各薪資區段名稱 |

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
               [
                  3,
                  1,
                  10,
                  17,
                  20,
                  7,
                  3,
                  0
               ]
            ],
            "name":"本期"
         },
         {
            "data":[
               [
                  2,
                  0,
                  20,
                  11,
                  15,
                  7,
                  3,
                  0
               ]
            ],
            "name":"上期"
         }
      ],
      "xaxis":{
         "data":[
            "100,001以上",
            "80,001 ~ 100,000",
            "60,001 ~ 80,000",
            "50,001 ~ 60,000",
            "40,001 ~ 50,000",
            "30,001 ~ 40,000",
            "25,001 ~ 30,000",
            "0 ~ 25,000"
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
