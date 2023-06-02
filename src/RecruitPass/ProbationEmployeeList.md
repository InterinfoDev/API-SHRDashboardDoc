# ProbationEmployeeList
試用人員資訊

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/RecruitPass/ProbationEmployeeList
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
    ,"depNumber":[16]
    ,"depType": "8"
    ,"workPlace":["TW"]
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
| companyId | 1 | Array(String) | 公司代號 | N | n/a |
| depNumber | 16 | Array(Integer) | 部門代碼 | N | n/a |
| depType | 8 | String| 統計階層 | Y | n/a |
| workPlace | TW | Array(String) | 工作地點 | N | n/a |
| yymm | 202212 | Array(Integer) | 本期月份 | Y | YYYYmm |
| lastYymm | 202206 | String | 上期月份 | Y | YYYYmm |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| labelName | 表格名稱 |
| labelKey | 表格索引 |
| empFullName | 人員名稱 |
| empStatus | 人員狀態 |
| interviewer | 面試人員 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "label":[
         {
            "labelName":"",
            "labelKey":"photo"
         },
         {
            "labelName":"姓名",
            "labelKey":"empFullName"
         },
         {
            "labelName":"面試人員",
            "labelKey":"interviewer"
         },
         {
            "labelName":"狀態",
            "labelKey":"empStatus"
         }
      ],
      "period":[
         
      ],
      "lastPeriod":[
         
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
