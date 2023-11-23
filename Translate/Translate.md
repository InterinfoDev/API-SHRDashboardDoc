# Translate
翻譯

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/Translate/Translate
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
        "locale":"TW",
        "deviceType":"WEB"
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
| locale | TW | String | 語系 | Y | n/a |
| deviceType | WEB | String | 裝置 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| locale | 部門暗碼 |
| deviceType | 員工編號 |
| translateList | 翻譯列表 |
| messageId | 要翻譯的文字KEY |
| content | 翻譯內容 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "translateList":[
         {
            "messageId":"Dashboard.D",
            "content":"人員配置策略"
         },
         {
            "messageId":"Dashboard.J",
            "content":"績效評估"
         },
         {
            "messageId":"Dashboard.H",
            "content":"員工動態"
         },
         {
            "messageId":"Dashboard.I",
            "content":"考勤洞察"
         },
         {
            "messageId":"Dashboard.M",
            "content":"薪資結構"
         },
         {
            "messageId":"Dashboard.F",
            "content":"教育與訓練"
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
