# PersonalData
個人資料

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/personalData/PersonalData
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
| fieldName | 功能名稱 |
| value | 功能代號 |
| oldValue | 開啟 |
| change | 子功能 |
| identifyData | 身分基本資料 |
| personalData | 個人基本資料 |
| connectData | 聯絡資料 |
| educationData | 教育資料 |
| benefitData | 保險與福利資料 |


### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "identifyData":[
         {
            "fieldName":"中文姓名",
            "value":"A",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"英文姓名",
            "value":"Administrator",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"單位名稱",
            "value":"1",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"分機號碼",
            "value":"34",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"職位",
            "value":"0002",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"照片",
            "value":"hrm/photo/1700033145524_WT-Group-V2.png",
            "oldValue":"",
            "change":false
         }
      ],
      "personalData":[
         {
            "fieldName":"行事曆班別",
            "value":"03",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"婚姻",
            "value":"A",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"電子信箱",
            "value":"richardwu@interinfo.com.tw",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"到職日期",
            "value":"20200309",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"工作地點",
            "value":"TW9",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"聯絡電話",
            "value":"03-244446799",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"行動電話",
            "value":"097X3XX620",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"原住民",
            "value":"Y",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"代扣所得稅",
            "value":"Y",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"體重",
            "value":"189",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"身高",
            "value":"160",
            "oldValue":"",
            "change":false
         }
      ],
      "connectData":[
         {
            "fieldName":"戶籍郵遞區號",
            "value":"8846",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"戶籍地址",
            "value":"新北市中和區建一路１５０號６樓之３",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"戶籍電話",
            "value":"02-12",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"現址郵遞區號",
            "value":"302",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"現址地址",
            "value":"測試路１２８０號",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"現址電話",
            "value":"02-888888880",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"通訊郵遞區號",
            "value":"0095558",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"通訊地址",
            "value":"新北市中和區建一路１５０號６樓之３",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"通訊電話",
            "value":"02-12345678",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"緊急聯絡人姓名",
            "value":"測試B",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"緊急聯絡人關係",
            "value":"朋友",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"緊急聯絡人電話",
            "value":"0975422222223",
            "oldValue":"",
            "change":false
         }
      ],
      "educationData":[
         {
            "fieldName":"最高學歷",
            "value":"7",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"畢業學校",
            "value":"A0007",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"主修科系",
            "value":"349914",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"請假時通知人員",
            "value":"0005,0008,0102",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"畢肄業年月",
            "value":"200706",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"留職停薪日期-起",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"留職停薪日期-訖",
            "value":"",
            "oldValue":"",
            "change":true
         }
      ],
      "benefitData":[
         {
            "fieldName":"健保生效日",
            "value":"19911201",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"健保等級",
            "value":"92100",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"健保優惠專案",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"健保眷口數",
            "value":"0",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"勞保生效日",
            "value":"20130428",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"勞保等級",
            "value":"21000",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"勞保優惠專案",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"公司提撥退休金",
            "value":"A",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"退休金等級",
            "value":"123",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"扶養人數",
            "value":"1",
            "oldValue":"",
            "change":false
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
