# AcceptFlowChart
管道招聘流程圖表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/RecruitWays/AcceptFlowChart
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
    ,"depNumber":[1,2,3,4]
    ,"yymm":"202111"
    ,"lastYymm":"202110"
    ,"depType":3
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
| depNumber | 1,2,3,4 | Array(Integer) | 部門代碼 | N | n/a |
| depType | 3 | Integer | 統計階層 | Y | n/a |
| yymm | 202212 | String | 本期月份 | Y | YYYYmm |
| lastYymm | 202206 | String | 上期月份 | Y | YYYYmm |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| target | 本期 |
| previous | 上期 |
| recruit | 入取人數 |
| apply | 申請人數 |
| interview | 面試人數 |
| wayName | 入職管道名稱 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "target":{
         "recruit":[
            0,
            0
         ],
         "apply":[
            7,
            2
         ],
         "interview":[
            0,
            0
         ],
         "wayName":[
            "104人力銀行",
            "A"
         ]
      },
      "previous":{
         "recruit":[
            0,
            0,
            0
         ],
         "apply":[
            6,
            1,
            4
         ],
         "interview":[
            0,
            0,
            0
         ],
         "wayName":[
            "104人力銀行",
            "公司網站",
            "A"
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
