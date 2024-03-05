# InductionAnalysisList
新進分析

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/InductionAnalysis/InductionAnalysisList
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
    ,"depNumber":[491]
    ,"depType": 6
    ,"yymm": "202202"
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
| depNumber | 491 | Array(Integer) | 部門代碼 | N | n/a |
| depType | 6 | Integer | 統計階層 | Y | n/a |
| yymm | 202202 | String | 本期月份 | Y | YYYYmm |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| sex | 性別 |
| seniority | 年資 |
| age | 年齡 |
| place | 地點 |
| grade | 職等 |
| depFunction | 部門功能 |
| possieKind | 職類 |
| education | 學歷 |
| possie | 職位 |
| inWay | 入職管道 |
| title | 人員基本資料標題 |


### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "sex":{
         "name":[
            "男性"
         ],
         "totalPeople":[
            5
         ],
         "percent":[
            100.0
         ],
         "employeeList":[
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ]
         ]
      },
      "seniority":{
         "name":[
            "01-02"
         ],
         "totalPeople":[
            5
         ],
         "percent":[
            100.0
         ],
         "employeeList":[
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ]
         ]
      },
      "age":{
         "name":[
            ""
         ],
         "totalPeople":[
            5
         ],
         "percent":[
            100.0
         ],
         "employeeList":[
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ]
         ]
      },
      "place":{
         "name":[
            "",
            "新北"
         ],
         "totalPeople":[
            4,
            1
         ],
         "percent":[
            80.0,
            20.0
         ],
         "employeeList":[
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ],
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ]
         ]
      },
      "grade":{
         "name":[
            "",
            "110360676791424783236",
            "107842664127494172736",
            "99072727910951251495"
         ],
         "totalPeople":[
            2,
            1,
            1,
            1
         ],
         "percent":[
            40.0,
            20.0,
            20.0,
            20.0
         ],
         "employeeList":[
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ],
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ],
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ],
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ]
         ]
      },
      "depFunction":{
         "name":[
            ""
         ],
         "totalPeople":[
            5
         ],
         "percent":[
            100.0
         ],
         "employeeList":[
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ]
         ]
      },
      "possieKind":{
         "name":[
            "主管及監督人員",
            "專業人員-營業"
         ],
         "totalPeople":[
            4,
            1
         ],
         "percent":[
            80.0,
            20.0
         ],
         "employeeList":[
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ],
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ]
         ]
      },
      "education":{
         "name":[
            ""
         ],
         "totalPeople":[
            5
         ],
         "percent":[
            100.0
         ],
         "employeeList":[
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ]
         ]
      },
      "possie":{
         "name":[
            "非主管職"
         ],
         "totalPeople":[
            5
         ],
         "percent":[
            100.0
         ],
         "employeeList":[
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ]
         ]
      },
      "inWay":{
         "name":[
            ""
         ],
         "totalPeople":[
            5
         ],
         "percent":[
            100.0
         ],
         "employeeList":[
            [
               {
                  "department":"總經理",
                  "photo":"",
                  "employeeFullName":"總經理",
                  "employeeFullEName":"總經理",
                  "possieName":"總經理"
               }
            ]
         ]
      },
      "title":[
         {
            "titleKey":"employeeFullName",
            "titleName":"姓名"
         },
         {
            "titleKey":"possieName",
            "titleName":"職稱"
         },
         {
            "titleKey":"department",
            "titleName":"部門"
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
