# DepartmentClassAvgList
部門平均個人參與時數

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/DepartmentTeachLectures/DepartmentClassAvgList
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
    "companyId":["1","2"]
    ,"depNumber":[]
    ,"yymm": "202301"
    ,"lastYymm":"202305"
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
| companyId | ["1","2"] | Array(String) | 公司代號 | N | n/a |
| depNumber | [] | Array(Integer) | 部門代碼 | N | n/a |
| yymm | 202301 | String | 本期年月 | Y | YYYYMM |
| lastYymm | 202305 | String | 上期年月 | Y | YYYYMM |
| depType | 8 | Integer | 統計階層 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| avgHours | 平均時數 |
| depFullName | 部門名稱 |
| joinPeople | 參與人數 |
| totalPeople | 部門總人數 |
| totalAmt | 總上課時數 |
| employeeAvgAmt | 個人平均時數 |
| departmentList | 部門物件 |

| className | 課程名稱 |
| classAmt | 課程時數 |
| classList | 參與人員物件 |

| photo | 照片 |
| empFullName | 中文姓名 |
| empFullEName | 英文姓名 |
| employeeId | 員工編號 |
| positionName | 職稱 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "data":[
         {
            "avgHours":2.0,
            "depFullName":"人力資源部",
            "depKey": "98422770919299281204"
            "joinPeople":4,
            "totalPeople":4,
            "totalAmt":8.0,
            "employeeAvgAmt":2.0,
            "departmentList":[
               {
                  "className":"",
                  "classAmt":5.0,
                  "classList":[
                     {
                        "photo":"",
                        "empFullName":"",
                        "empFullEName":"",
                        "employeeId":"10001068",
                        "positionName":""
                     },
                     {
                        "photo":"",
                        "empFullName":"王O足",
                        "empFullEName":"Sandra",
                        "employeeId":"10009002",
                        "positionName":"專員"
                     },
                     {
                        "photo":"hrm/photo/1654659341079_1653032665894.jpg",
                        "empFullName":"蔡O隆",
                        "empFullEName":"Lonny",
                        "employeeId":"10108001",
                        "positionName":"經理"
                     },
                     {
                        "photo":"",
                        "empFullName":"王O靜",
                        "empFullEName":"Irene",
                        "employeeId":"10210038",
                        "positionName":""
                     }
                  ]
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
