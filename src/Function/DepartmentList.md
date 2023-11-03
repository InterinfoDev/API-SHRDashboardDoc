# DepartmentList
部門群組列表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/Function/DepartmentList
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

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| depNumber | 部門暗碼 |
| depFullName | 部門中文名稱 |
| depCode | 部門代號 |
| subDepartmentList | 下一層部門列表 |
| departmentList | 部門列表 |
| groupList | 群組列表 |
| depKey | 單位key值 |


### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "departmentList":[
         {
            "depNumber":123532,
            "depFullName":"英x內集團",
            "depCode":"01231",
            "depKey":"1324679",
            "subDepartmentList":[
               {
                  "depNumber":53,
                  "depFullName":"董x會",
                  "depCode":"012302",
                  "depKey":"1321111",
                  "subDepartmentList":[
                     {
                        "depNumber":132,
                        "depFullName":"英x內軟體公司",
                        "depCode":"001233",
                        "depKey":"1321111",
                        "subDepartmentList":[
                        ]
                     }
                  ]
               }
            ]
         }
      ],
      "groupList":[
         {
            "depNumber":1002002,
            "depFullName":"sys.異動單撤單群組",
            "depCode":"1002002",
            "depKey":"1321111"
         },
         {
            "depNumber":1001003,
            "depFullName":"sys.HR主管",
            "depCode":"1001003",
            "depKey":"1321111"
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
