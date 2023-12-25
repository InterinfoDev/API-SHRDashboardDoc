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
        "locale":"US",
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
            "messageId":"personalData",
            "content":"PersonalData"
         },
         {
            "messageId":"connectData",
            "content":"ConnectData"
         },
         {
            "messageId":"educationData",
            "content":"EducationData"
         },
         {
            "messageId":"benefitData",
            "content":"BenefitData"
         },
         {
            "messageId":"Dashboard.D001",
            "content":"D001.Manpower gap analysis"
         },
         {
            "messageId":"Dashboard.D002",
            "content":"D002.Admissions channel analysis"
         },
         {
            "messageId":"Dashboard.D003",
            "content":"D003.Recruitment efficiency analysis"
         },
         {
            "messageId":"Dashboard.D004",
            "content":"D004.The average number of days to recruit"
         },
         {
            "messageId":"Dashboard.D005",
            "content":"D005.New Employee Registration Form"
         },
         {
            "messageId":"Dashboard.D006",
            "content":"D006.Probationary pass rate"
         },
         {
            "messageId":"Dashboard.D007",
            "content":"D007.Analysis of departmental screening results"
         },
         {
            "messageId":"Dashboard.D008",
            "content":"D008.Analysis of the results of the job screening"
         },
         {
            "messageId":"Dashboard.D009",
            "content":"D009.Overview of comprehensive recruitment"
         },
         {
            "messageId":"Dashboard.D009",
            "content":"D009.Overview of comprehensive recruitment"
         },
         {
            "messageId":"Dashboard.D",
            "content":"Staffing policies"
         },
         {
            "messageId":"Dashboard.J",
            "content":"Performance evaluation"
         },
         {
            "messageId":"Dashboard.H",
            "content":"Employee dynamics"
         },
         {
            "messageId":"Dashboard.I",
            "content":"Time and Attendance Insights"
         },
         {
            "messageId":"Dashboard.M",
            "content":"Salary structure"
         },
         {
            "messageId":"Dashboard.F",
            "content":"Education and training"
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
