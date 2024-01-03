# CheckRight
登入程式

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/Login/Login
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
      "uid":"admin",
      "pwd":"***"
  },
  
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
| uid | admin | String | 登入帳號 | Y | n/a |
| pwd | 1234 | String | 登入密碼 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| message | 訊息 |
| uid | uid |
| right | right |
| employeeId | 員工編號 |
| companyId | 公司別 |
| empFullName | 員工中文姓名 |
| empFullEname | 員工英文姓名 |
| photo | 照片 |
| creatDate | 建立日期 |
| depNumber | 單位暗碼 |
| function | 功能權限資料 |
| canUseFunctionList | 可使用功能id列表 |
| subProjectList | 子功能 |
| name | 功能名稱 |
| page | 功能代號 |
| canUseAuth | 是否可開啟控制權限功能 |


### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "message":"登入成功",
      "uid":"98599308101484732326",
      "right":"513419119041735433367561625448648202801232182995256636587932016607439201462467319648726770275885372239590800399001566315900396556929299037600232648201351969199641014176580846429247388363722146065540219961236084898593114544937584461505352839335947616602998960813194183124475504037556942873149438591889655059513673018084711428908540622107324856963523039241069256194926209637696174210369550481835429797148675583542717241524233851261984572551146679123702854536189254789600560912885708690599215102879587757453324825026368902089400686676006754475363097835998026942763386332970165139051",
      "employeeId":"admin",
      "companyId":"1",
      "empFullName":"管理者",
      "empFullEname":"",
      "photo":"",
      "creatDate":"19980102",
      "depNumber":1
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
