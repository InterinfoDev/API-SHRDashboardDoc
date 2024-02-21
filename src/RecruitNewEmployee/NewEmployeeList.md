# NewEmployeeList
新進員工人員資訊

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/RecruitPositionResult/NewEmployeeList
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
    "companyId":[1,2]
    ,"lastYymm":"202212"
    ,"yymm": "202301"
    ,"depNumber":[]
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
| depNumber | [] | Array(Integer) | 部門代碼 | N | n/a |
| depType | 8 | Integer | 統計階層 | Y | n/a |
| yymm | 202301 | String | 本期年月 | Y | YYYYMM |
| lastYymm | 202212 | String | 上期年月 | Y | YYYYMM |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| label | 欄位資訊 |
| labelName | 欄位中文名稱 |
| labelKey | 欄位key值名稱 |
| period | 本期月份 |
| lastPeriod | 上期月份 |
| photo | 照片 |
| empFullName | 中文姓名 |
| empFullEName | 英文姓名 |
| position | 職稱中文名稱 |
| inDate | 到職日期 |
| interviewLink | 履歷連結 |
| pno | 單號 |


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
            "labelName":"職稱",
            "labelKey":"Position"
         },
         {
            "labelName":"到職日期",
            "labelKey":"inDate"
         },
         {
            "labelName":"",
            "labelKey":"interviewLink"
         },
         {
            "labelName":"",
            "labelKey":"pno"
         }
      ],
      "period":[
         {
            "photo":"",
            "empFullName":"江O甫",
            "empFullEName":"andy",
            "position":"",
            "inDate":"",
            "interviewLink":"",
            "pno":"002021011100001"
         }
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
