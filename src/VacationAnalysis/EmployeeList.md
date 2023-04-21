# EmployeeList
請假人員列表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/VacationAnalysis/DepartmentNum
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
    "companyId":[]
    ,"depNumber":[],
    ,"depType": 3
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
| depNumber |  | Array(Integer) | 部門代碼 | N | n/a |
| depType | 3 | Integer | 統計階層 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| title | 標題 |
| labelName | 標題名稱 |
|  |
| photo | 照片 |
| employeeId | 員工編號 |
| employeeFullName | 員工名稱 |
| possieName | 職稱 |
| vacationKind | 假別名稱 |
| departmentFullName | 部門名稱 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "title":[
         {
            "labelName":"姓名",
            "labelKey":"empFullName"
         },
         {
            "labelName":"員工編號",
            "labelKey":"employeeId"
         },
         {
            "labelName":"職稱",
            "labelKey":"possieName"
         },
         {
            "labelName":"部門",
            "labelKey":"departmentFulName"
         },
         {
            "labelName":"假別",
            "labelKey":"vacationKind"
         }
      ],
      "dataList":[
         {
            "photo":"",
            "employeeId":"test2yearshour1",
            "employeeFullName":"測試兩年病假時數1",
            "possieName":"職員",
            "vacationKind":[
               "2(時)測試兩年假別"
            ],
            "departmentFullName":"勞安部",
            "employeeFullEName":""
         },
         {
            "photo":"",
            "employeeId":"test2yearshour2",
            "employeeFullName":"測試兩年病假時數2",
            "possieName":"職員",
            "vacationKind":[
               "2(時)測試兩年假別"
            ],
            "departmentFullName":"勞安部",
            "employeeFullEName":""
         },
         {
            "photo":"",
            "employeeId":"11204002",
            "employeeFullName":"測試排班請產假",
            "possieName":"職員",
            "vacationKind":[
               "產假"
            ],
            "departmentFullName":"勞安部",
            "employeeFullEName":""
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
