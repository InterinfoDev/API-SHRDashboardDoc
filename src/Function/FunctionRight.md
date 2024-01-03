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
| name | 功能名稱 |
| page | 功能代號 |
| functionKey | 功能Key |
| subProjectList | 子功能 |
| right | 是否登入狀態 |


### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "canUseAuth":true,
      "right":true,
      "function":{
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
         ]
      }
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
