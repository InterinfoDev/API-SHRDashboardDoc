# AverageTrendChart
部門平均薪資趨勢

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/SalaryDistribution/AverageTrendChart
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
    ,"depNumber":[]
    ,"depType": "3"
    ,"yymm": "202304"
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
| depNumber |  | Array(Integer) | 部門代碼 | N | n/a |
| depType | 3 | String| 統計階層 | Y | n/a |
| depNumber |  | Array(Integer) | 部門代碼 | Y | n/a |
| yymm | 202304 | Array(Integer) | 本期月份 | Y | YYYYmm |


### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| averageCostList | 平均薪資 |
| yymmList | 月份 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "averageCostList":[
         0,
         3866728,
         2347933,
         4700769,
         787052,
         698321,
         2210509,
         0,
         8501,
         0,
         935803,
         1150683
      ],
      "yymmList":[
         202204,
         202205,
         202206,
         202207,
         202208,
         202209,
         202210,
         202211,
         202212,
         202301,
         202302,
         202303
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
