# FunctionRight
可使用功能權限

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/Function/FunctionRight
```

### HTTP Request Mehod
```
POST
```

### Request body
| Key | Value | Type | Description |
|:----------|:-------------|:-----|:------------|


### JSON representation

Here is a JSON representation of request.
```json
{
  "requestHeader": {
  },
  "requestBody": {
      
  }
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
| name | 功能名稱 |
| page | 功能代號 |
| functionKey | 功能Key |
| subProjectList | 子功能 |
| uid | uid |
| right | 登入權限 |
| canUseFunctionList | 可以使用的功能列表 |
| employeeId | 員工編號 |
| empFullEname | 中文姓名 |
| empFullEname | 英文姓名 |
| depType | 單位階層 |
| depNumber | 單位暗碼 |
| photo | 照片 |
| creatDate | 入職日期 |
| status | 登入狀態 |


### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "data":{
         "canUseFunctionList":[
            {
               "name":"人員配置策略",
               "page":"Dashboard.D",
               "functionKey":"1864901968730750136650025588166193174856",
               "subProjectList":[
                  {
                     "name":"D001.人力缺口分析",
                     "page":"Dashboard.D001",
                     "functionKey":"1864901968730750136654522318106618588649"
                  },
                  {
                     "name":"D002.錄取管道分析",
                     "page":"Dashboard.D002",
                     "functionKey":"1864901968730750136643422650747353039852"
                  }
               ]
            }
         ],
         "uid": "98599308101484732326",
         "right":"40749767134770117",
         "employeeId":"admin",
         "companyId":"97090920",
         "empFullName":"呂宜真",
         "empFullEname":"ADA",
         "depNumber": 5,
         "depType": 9,
         "photo":"XXXXXXXXXXXXX",
         "creatDate":"20090801",
         "canUseAuth": true
      },
      "status":true
   }
}
```

### HTTP Response when No Data
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "canUseAuth":false,
      "right":false,
      "data":{
         
      },
      "status":false
   }
}

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
