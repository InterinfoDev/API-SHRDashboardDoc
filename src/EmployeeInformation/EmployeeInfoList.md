# EmployeeInfoList
人事資料總表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/EmployeeInformation/EmployeeInfoList
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
    ,"depNumber":[5]
    ,"depType": 12
    ,"yymm": "202201"
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
| depNumber | 5 | Array(Integer) | 部門代碼 | N | n/a |
| depType | 12 | Integer | 統計階層 | Y | n/a |
| yymm | 202201 | String | 本期月份 | Y | YYYYmm |

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
            "*",
            "女性"
         ],
         "totalPeople":[
            22,
            1
         ],
         "percent":[
            96.0,
            4.0
         ],
         "employeeList":[
            [
               {
                  "department":"L1線A班",
                  "photo":"",
                  "employeeFullName":"欒O鈞",
                  "employeeFullEName":"HELOOKE",
                  "possieName":"執行長(二)"
               },
               {
                  "department":"L1線A班",
                  "photo":"",
                  "employeeFullName":"郝O翔",
                  "employeeFullEName":"HELOOKE",
                  "possieName":""
               }
            ],
            [
               {
                  "department":"L1線A班",
                  "photo":"",
                  "employeeFullName":"房O瑾",
                  "possieName":""
               }
            ]
         ]
      },
      "seniority":{
         "name":[
            "05-10",
            ">=15",
            "03-05",
            "02-03",
            "10-15"
         ],
         "totalPeople":[
            12,
            2,
            3,
            4,
            2
         ],
         "percent":[
            52.0,
            9.0,
            13.0,
            17.0,
            9.0
         ],
         "employeeList":[
            [
               {
                  "department":"L1線A班",
                  "photo":"",
                  "employeeFullName":"欒O鈞",
                  "employeeFullEName":"JIU",
                  "possieName":"執行長(二)"
               }
            ],
            [
               {
                  "department":"L1線A班",
                  "photo":"/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f28574d52634f57504b50637a726f605e5b52565111554f58",
                  "employeeFullName":"寶O寶",
                  "possieName":"系統管理員"
               },
               {
                  "department":"L1線A班",
                  "photo":"/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f0110574d520b104f57504b50100e090b070a0b0d0a0f0706070860060b0c5e0b5e0e0859075a0d0d075a5b0d0e0b0b0e0f0b0b0f0a0e0a5b5a070811554f58",
                  "employeeFullName":"國O詳",
                  "possieName":"系統管理員"
               }
            ]
         ]
      },
      "age":{
         "name":[
            "60歲以上",
            "30 <= 35歲",
            "35 <= 40歲",
            "25 <= 30歲",
            "40 <= 45歲",
            "45 <= 50歲"
         ],
         "totalPeople":[
            2,
            7,
            5,
            1,
            2,
            6
         ],
         "percent":[
            9.0,
            30.0,
            22.0,
            4.0,
            9.0,
            26.0
         ],
         "employeeList":[
            [
               {
                  "department":"L1線A班",
                  "photo":"",
                  "employeeFullName":"欒O鈞",
                  "employeeFullEName":"JIE",
                  "possieName":"執行長(二)"
               }
            ]
         ]
      },
      "place":{
         "name":[
            "",
            "*上海",
            ""
         ],
         "totalPeople":[
            1,
            2,
            20
         ],
         "percent":[
            4.0,
            9.0,
            87.0
         ],
         "employeeList":[
            [
               {
                  "department":"L1線A班",
                  "photo":"",
                  "employeeFullName":"欒O鈞",
                  "possieName":"執行長(二)"
               }
            ],
            [
               {
                  "department":"L1線A班",
                  "photo":"",
                  "employeeFullName":"郝O翔",
                  "employeeFullEName":"KOE",
                  "possieName":""
               }
            ]
         ]
      },
      "grade":{
         "name":[
            "11",
            "01",
            "98396216677142659938"
         ],
         "totalPeople":[
            21,
            1,
            1
         ],
         "percent":[
            91.0,
            4.0,
            4.0
         ],
         "employeeList":[
            [
               {
                  "department":"L1線A班",
                  "photo":"",
                  "employeeFullName":"欒O鈞",
                  "employeeFullEName":"HEB",
                  "possieName":"執行長(二)"
               }
            ]
         ]
      },
      "depFunction":{
         "name":[
            "營業管理"
         ],
         "totalPeople":[
            1
         ],
         "percent":[
            4.0
         ],
         "employeeList":[
            [
               {
                  "department":"L1線A班",
                  "photo":"",
                  "employeeFullName":"欒O鈞",
                  "employeeFullEName":"JEOI",
                  "possieName":"執行長(二)"
               }
            ]
         ]
      },
      "possieKind":{
         "name":[
            "主管及監督人員",
            "",
            "專業人員-生產",
            "研究人員",
            "約聘人員"
         ],
         "totalPeople":[
            1,
            10,
            5,
            5,
            2
         ],
         "percent":[
            4.0,
            43.0,
            22.0,
            22.0,
            9.0
         ],
         "employeeList":[
            [
               {
                  "department":"L1線A班",
                  "photo":"",
                  "employeeFullEName":"KOKJD",
                  "employeeFullName":"欒O鈞",
                  "possieName":"執行長(二)"
               }
            ]
            ]
         ]
      },
      "education":{
         "name":[
            "大學畢業",
            "碩士班畢業",
            ""
         ],
         "totalPeople":[
            14,
            1,
            8
         ],
         "percent":[
            61.0,
            4.0,
            35.0
         ],
         "employeeList":[
            [
               {
                  "department":"L1線A班",
                  "photo":"",
                  "employeeFullName":"欒O鈞",
                  "employeeFullEName":"JUE",
                  "possieName":"執行長(二)"
               }
            ]
         ]
      },
      "possie":{
         "name":[
            "非主管職"
         ],
         "totalPeople":[
            23
         ],
         "percent":[
            100.0
         ],
         "employeeList":[
            [
               {
                  "department":"L1線A班",
                  "photo":"",
                  "employeeFullName":"欒O鈞",
                  "employeeFullEName":"SSD",
                  "possieName":"執行長(二)"
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
