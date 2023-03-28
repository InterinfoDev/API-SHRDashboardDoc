# LeaveWithoutPayEmployeeChart
申請留停/留任/回任圖表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/LeaveWithoutPayRate/LeaveWithoutPayEmployeeChart
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
    ,"depNumber":[17]
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
| depNumber | 17 | Array(Integer) | 部門代碼 | N | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| employeeId | 員工編號 |
| empFullName | 員工中文姓名 |
| photo | 員工照片 |
| positionName | 員工職稱 |
| depFullName | 部門名稱 |
| changeDate | 異動日期 |
| changeType | 異動類型 |
| changeTypeName | 異動類型名稱 |

### requestBody changeType
| Type | TypeName |
|:----------|:-------------|
| I | 留停 |
| F | 復職 |
| L | 離職 |

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
            "employeeId":"000088",
            "empFullName":"充O棋",
            "photo":"",
            "positionName":"",
            "depFullName":"企劃部",
            "changeDateList":[
               {
                  "changeDate":"20220613",
                  "changeType":"I",
                  "changeTypeName":"留停"
               }
            ]
         },
         {
            "employeeId":"T1019",
            "empFullName":"test1019",
            "photo":"",
            "positionName":"系統管理員",
            "depFullName":"企劃部",
            "changeDateList":[
               {
                  "changeDate":"20230331",
                  "changeType":"L",
                  "changeTypeName":"離職"
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
