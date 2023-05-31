# CostAverageDifferenceList
部門平均薪資差異

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/SalaryDistribution/CostAverageDifferenceList
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
| DepFullName | 部門名稱 |
| DepTotalSalary | 部門用人成本 |
| departmentAverageDifferent | 部門平均薪資差異 |
| borrow | 借工列表 |
| support | 支援列表 |
| hour | 支援列表 |
| employeeFullName | 員工名稱 |
| possieName | 職務 |
| employeeId | 員工編耗 |
| depFullName | 部門名稱 |
| photo | 照片 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "dataList":[
         {
            "DepTotalSalary":"31098",
            "DepFullName":"支援部",
            "borrow":[
               {
                  "hour":"3.00",
                  "employeeFullName":"",
                  "possieName":"",
                  "employeeId":"A2022001",
                  "employeeFullEName": "",
                  "depFullName":"",
                  "photo":""
               },
               {
                  "hour":"8.00",
                  "employeeFullName":"",
                  "employeeFullEName": "",
                  "possieName":"",
                  "employeeId":"A2022001",
                  "depFullName":"",
                  "photo":""
               }
            ],
            "DepAverageDifferent":"0",
            "support":[
               
            ]
         },
         {
            "DepTotalSalary":"29463",
            "DepFullName":"企劃部",
            "borrow":[
               
            ],
            "DepAverageDifferent":"0",
            "support":[
               {
                  "hour":"3.00",
                  "employeeFullName":"",
                  "possieName":"",
                  "employeeId":"A2022001",
                  "depFullName":"",
                  "employeeFullEName": "",
                  "photo":""
               }
            ]
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
