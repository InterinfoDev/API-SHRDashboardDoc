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
            "employeeId":"0310",
            "employeeFullName":"卓O伶",
            "possieName":"顧問(二)",
            "vacationKind":[
               "半薪病假"
            ],
            "departmentFullName":"顧問處"
         },
         {
            "photo":"",
            "employeeId":"1617",
            "employeeFullName":"楊O齊",
            "possieName":"正工程師(一)",
            "vacationKind":[
               "半薪病假"
            ],
            "departmentFullName":"副總"
         },
         {
            "photo":"hrm/photo/1531381267307_1_褚家妤.PNG",
            "employeeId":"0538",
            "employeeFullName":"池O祥",
            "possieName":"系統管理員",
            "vacationKind":[
               "婚假(天)"
            ],
            "departmentFullName":"顧問處"
         },
         {
            "photo":"hrm\\photo\\EMP_admin.jpg",
            "employeeId":"0600",
            "employeeFullName":"鞏O貞",
            "possieName":"5038",
            "vacationKind":[
               "事假"
            ],
            "departmentFullName":""
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