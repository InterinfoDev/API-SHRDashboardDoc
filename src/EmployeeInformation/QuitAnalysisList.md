# QuitAnalysisList
離職分析

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/QuitAnalysis/QuitAnalysisList
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
    ,"depNumber":[82]
    ,"depType": 3
    ,"yymm": "02202"
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
| depNumber | 82 | Array(Integer) | 部門代碼 | N | n/a |
| depType | 3 | Integer | 統計階層 | Y | n/a |
| yymm | 202202 | String | 本期月份 | Y | YYYYmm |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| data | 欄位資料 |
| name | 考核等級中文 |
| pass | 是否合格 |
| value | 考核人數 |


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
            "女性"
         ],
         "totalPeople":[
            3
         ],
         "percent":[
            100.0
         ],
         "employeeList":[
            [
               {
                  "department":"",
                  "photo":"",
                  "employeeFullName":"金O淇",
                  "possieName":""
               },
               {
                  "department":"英特內(台北)",
                  "photo":"",
                  "employeeFullName":"再測二",
                  "possieName":"系統管理員"
               },
               {
                  "department":"L1線B班",
                  "photo":"",
                  "employeeFullName":"池O祥",
                  "possieName":"董事長"
               }
            ]
         ]
      },
      "seniority":{
         "name":[
            ">=15",
            "00-01"
         ],
         "totalPeople":[
            2,
            1
         ],
         "percent":[
            67.0,
            33.0
         ],
         "employeeList":[
            [
               {
                  "department":"",
                  "photo":"",
                  "employeeFullName":"金O淇",
                  "possieName":""
               },
               {
                  "department":"L1線B班",
                  "photo":"",
                  "employeeFullName":"池O祥",
                  "possieName":"董事長"
               }
            ],
            [
               {
                  "department":"英特內(台北)",
                  "photo":"",
                  "employeeFullName":"再測二",
                  "possieName":"系統管理員"
               }
            ]
         ]
      },
      "age":{
         "name":[
            "60歲以上",
            "45 <= 50歲"
         ],
         "totalPeople":[
            2,
            1
         ],
         "percent":[
            67.0,
            33.0
         ],
         "employeeList":[
            [
               {
                  "department":"",
                  "photo":"",
                  "employeeFullName":"金O淇",
                  "possieName":""
               },
               {
                  "department":"L1線B班",
                  "photo":"",
                  "employeeFullName":"池O祥",
                  "possieName":"董事長"
               }
            ],
            [
               {
                  "department":"英特內(台北)",
                  "photo":"",
                  "employeeFullName":"再測二",
                  "possieName":"系統管理員"
               }
            ]
         ]
      },
      "place":{
         "name":[
            "新北",
            "",
            "桃園"
         ],
         "totalPeople":[
            1,
            1,
            1
         ],
         "percent":[
            33.0,
            33.0,
            33.0
         ],
         "employeeList":[
            [
               {
                  "department":"",
                  "photo":"",
                  "employeeFullName":"金O淇",
                  "possieName":""
               }
            ],
            [
               {
                  "department":"英特內(台北)",
                  "photo":"",
                  "employeeFullName":"再測二",
                  "possieName":"系統管理員"
               }
            ],
            [
               {
                  "department":"L1線B班",
                  "photo":"",
                  "employeeFullName":"池O祥",
                  "possieName":"董事長"
               }
            ]
         ]
      },
      "grade":{
         "name":[
            "98396216677142659938",
            "107612000800231585522"
         ],
         "totalPeople":[
            2,
            1
         ],
         "percent":[
            67.0,
            33.0
         ],
         "employeeList":[
            [
               {
                  "department":"",
                  "photo":"",
                  "employeeFullName":"金O淇",
                  "possieName":""
               },
               {
                  "department":"L1線B班",
                  "photo":"",
                  "employeeFullName":"池O祥",
                  "possieName":"董事長"
               }
            ],
            [
               {
                  "department":"英特內(台北)",
                  "photo":"",
                  "employeeFullName":"再測二",
                  "possieName":"系統管理員"
               }
            ]
         ]
      },
      "depFunction":{
         "name":[
            "",
            "",
            "營業管理"
         ],
         "totalPeople":[
            1,
            1,
            1
         ],
         "percent":[
            33.0,
            33.0,
            33.0
         ],
         "employeeList":[
            [
               {
                  "department":"",
                  "photo":"",
                  "employeeFullName":"金O淇",
                  "possieName":""
               }
            ],
            [
               {
                  "department":"英特內(台北)",
                  "photo":"",
                  "employeeFullName":"再測二",
                  "possieName":"系統管理員"
               }
            ],
            [
               {
                  "department":"L1線B班",
                  "photo":"",
                  "employeeFullName":"池O祥",
                  "possieName":"董事長"
               }
            ]
         ]
      },
      "possieKind":{
         "name":[
            "",
            "研究人員",
            "主管及監督人員"
         ],
         "totalPeople":[
            1,
            1,
            1
         ],
         "percent":[
            33.0,
            33.0,
            33.0
         ],
         "employeeList":[
            [
               {
                  "department":"",
                  "photo":"",
                  "employeeFullName":"金O淇",
                  "possieName":""
               }
            ],
            [
               {
                  "department":"英特內(台北)",
                  "photo":"",
                  "employeeFullName":"再測二",
                  "possieName":"系統管理員"
               }
            ],
            [
               {
                  "department":"L1線B班",
                  "photo":"",
                  "employeeFullName":"池O祥",
                  "possieName":"董事長"
               }
            ]
         ]
      },
      "education":{
         "name":[
            "中學畢業",
            ""
         ],
         "totalPeople":[
            2,
            1
         ],
         "percent":[
            67.0,
            33.0
         ],
         "employeeList":[
            [
               {
                  "department":"",
                  "photo":"",
                  "employeeFullName":"金O淇",
                  "possieName":""
               },
               {
                  "department":"L1線B班",
                  "photo":"",
                  "employeeFullName":"池O祥",
                  "possieName":"董事長"
               }
            ],
            [
               {
                  "department":"英特內(台北)",
                  "photo":"",
                  "employeeFullName":"再測二",
                  "possieName":"系統管理員"
               }
            ]
         ]
      },
      "possie":{
         "name":[
            "非主管職",
            "主管職"
         ],
         "totalPeople":[
            2,
            1
         ],
         "percent":[
            67.0,
            33.0
         ],
         "employeeList":[
            [
               {
                  "department":"",
                  "photo":"",
                  "employeeFullName":"金O淇",
                  "possieName":""
               },
               {
                  "department":"英特內(台北)",
                  "photo":"",
                  "employeeFullName":"再測二",
                  "possieName":"系統管理員"
               }
            ],
            [
               {
                  "department":"L1線B班",
                  "photo":"",
                  "employeeFullName":"池O祥",
                  "possieName":"董事長"
               }
            ]
         ]
      },
      "quitReason":{
         "name":[
            "工作內容",
            "_8"
         ],
         "totalPeople":[
            2,
            1
         ],
         "percent":[
            67.0,
            33.0
         ],
         "employeeList":[
            [
               {
                  "department":"",
                  "photo":"",
                  "employeeFullName":"金O淇",
                  "possieName":""
               },
               {
                  "department":"英特內(台北)",
                  "photo":"",
                  "employeeFullName":"再測二",
                  "possieName":"系統管理員"
               }
            ],
            [
               {
                  "department":"L1線B班",
                  "photo":"",
                  "employeeFullName":"池O祥",
                  "possieName":"董事長"
               }
            ]
         ]
      },
      "title":[
         {
            "titleKey":"photo",
            "titleName":""
         },
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
