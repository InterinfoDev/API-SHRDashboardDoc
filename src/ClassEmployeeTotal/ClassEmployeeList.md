# ClassEmployeeList
實際出勤人員列表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/ClassEmployeeTotal/ClassEmployeeList
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
    "companyId":["1"]
    ,"depNumber":[7,13,14,21,22,23,24,25,26,30,31,32,33]
    ,"yymmdd": "20220103"
    ,"lastYymmdd": "20211230"
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
| companyId | 1 | Array(String) | 公司代號 | N | n/a |
| depNumber | [7,13,14,21,22,23,24,25,26,30,31,32,33] | Array(Integer) | 部門代碼 | N | n/a |
| yymmdd | 20220103 | String | 本期年月日 | Y | YYYYMMDD |
| lastYymmdd | 20211230 | String | 上期年月日 | Y | YYYYMMDD |
| depType | 8 | Integer | 統計階層 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| label | 表頭 |
| labelName | 表頭名稱 |
| labelKey | 表頭KEY |
| period | 本期資料 |
| lastPeriod | 上期資料 |
| photo | 照片 |
| empFullName | 中文姓名 |
| empEnglishName | 英文姓名 |
| employee | 員工編號 |
| position | 職稱 |
| depFullName | 部門名稱 |
| className | 假別 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "label":[
         {
            "labelName":"姓名",
            "labelKey":"empFullName"
         },
         {
            "labelName":"員工編號",
            "labelKey":"employee"
         },
         {
            "labelName":"職稱",
            "labelKey":"position"
         },
         {
            "labelName":"部門",
            "labelKey":"depFullName"
         },
         {
            "labelName":"班別",
            "labelKey":"className"
         }
      ],
      "period":[
         {
            "photo":"",
            "empFullName":"蔡O中",
            "empEnglishName":"Vincent",
            "employee":"9006006",
            "position":"營業部經理",
            "depFullName":"銷售本部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O2",
            "empEnglishName":"",
            "employee":"TEST001",
            "position":"職員",
            "depFullName":"銷售本部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O婷",
            "empEnglishName":"Mindy",
            "employee":"11011013",
            "position":"副理",
            "depFullName":"人力資源部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O佑",
            "empEnglishName":"LIN CHIEN YOU",
            "employee":"8701001",
            "position":"董事長",
            "depFullName":"人力資源部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O嘉",
            "empEnglishName":"Wei",
            "employee":"10802031",
            "position":"專員",
            "depFullName":"勞安部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王OH",
            "empEnglishName":"",
            "employee":"11109003",
            "position":"外場-兼職三級",
            "depFullName":"勞安部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王OA",
            "empEnglishName":"",
            "employee":"11109004",
            "position":"外場-兼職三級",
            "depFullName":"勞安部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王OH",
            "empEnglishName":"",
            "employee":"11109005",
            "position":"外場-兼職三級",
            "depFullName":"勞安部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王OA",
            "empEnglishName":"",
            "employee":"11109006",
            "position":"外場-兼職三級",
            "depFullName":"勞安部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O燕",
            "empEnglishName":"Aileen",
            "employee":"9403012",
            "position":"專員",
            "depFullName":"勞安部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O離",
            "empEnglishName":"",
            "employee":"TEST20220613001",
            "position":"職員",
            "depFullName":"勞安部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O移",
            "empEnglishName":"",
            "employee":"TEST20220708",
            "position":"職員",
            "depFullName":"勞安部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O無",
            "empEnglishName":"",
            "employee":"TEST20220728",
            "position":"經理",
            "depFullName":"勞安部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"蔡O宇",
            "empEnglishName":"Nick",
            "employee":"10808081",
            "position":"專員",
            "depFullName":"採購部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"蔡O琳",
            "empEnglishName":"sunny",
            "employee":"10810006",
            "position":"專員",
            "depFullName":"採購部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O足",
            "empEnglishName":"Sandra",
            "employee":"10009002",
            "position":"專員",
            "depFullName":"總務部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O珊",
            "empEnglishName":"",
            "employee":"10601010",
            "position":"按摩人員",
            "depFullName":"總務部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O真",
            "empEnglishName":"",
            "employee":"10811025",
            "position":"按摩人員",
            "depFullName":"總務部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O芳",
            "empEnglishName":"",
            "employee":"8712001",
            "position":"司機",
            "depFullName":"總務部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"蔡O璐",
            "empEnglishName":"Yalu",
            "employee":"8912001",
            "position":"專員",
            "depFullName":"總務部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O英",
            "empEnglishName":"Yeang",
            "employee":"10206047",
            "position":"專員",
            "depFullName":"勞安部",
            "className":"測試行事曆"
         }
      ],
      "lastPeriod":[
         {
            "photo":"",
            "empFullName":"蔡O中",
            "empEnglishName":"Vincent",
            "employee":"9006006",
            "position":"營業部經理",
            "depFullName":"銷售本部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O2",
            "empEnglishName":"",
            "employee":"TEST001",
            "position":"職員",
            "depFullName":"銷售本部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O婷",
            "empEnglishName":"Mindy",
            "employee":"11011013",
            "position":"副理",
            "depFullName":"人力資源部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O佑",
            "empEnglishName":"LIN CHIEN YOU",
            "employee":"8701001",
            "position":"董事長",
            "depFullName":"人力資源部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O嘉",
            "empEnglishName":"Wei",
            "employee":"10802031",
            "position":"專員",
            "depFullName":"勞安部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O燕",
            "empEnglishName":"Aileen",
            "employee":"9403012",
            "position":"專員",
            "depFullName":"勞安部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O離",
            "empEnglishName":"",
            "employee":"TEST20220613001",
            "position":"職員",
            "depFullName":"勞安部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O移",
            "empEnglishName":"",
            "employee":"TEST20220708",
            "position":"職員",
            "depFullName":"勞安部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O無",
            "empEnglishName":"",
            "employee":"TEST20220728",
            "position":"經理",
            "depFullName":"勞安部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"蔡O宇",
            "empEnglishName":"Nick",
            "employee":"10808081",
            "position":"專員",
            "depFullName":"採購部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"蔡O琳",
            "empEnglishName":"sunny",
            "employee":"10810006",
            "position":"專員",
            "depFullName":"採購部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O足",
            "empEnglishName":"Sandra",
            "employee":"10009002",
            "position":"專員",
            "depFullName":"總務部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O珊",
            "empEnglishName":"",
            "employee":"10601010",
            "position":"按摩人員",
            "depFullName":"總務部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O真",
            "empEnglishName":"",
            "employee":"10811025",
            "position":"按摩人員",
            "depFullName":"總務部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O芳",
            "empEnglishName":"",
            "employee":"8712001",
            "position":"司機",
            "depFullName":"總務部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"蔡O璐",
            "empEnglishName":"Yalu",
            "employee":"8912001",
            "position":"專員",
            "depFullName":"總務部",
            "className":"總公司班"
         },
         {
            "photo":"",
            "empFullName":"王O英",
            "empEnglishName":"Yeang",
            "employee":"10206047",
            "position":"專員",
            "depFullName":"勞安部",
            "className":"測試行事曆"
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
