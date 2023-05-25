# DepartmentLevelOption
單位階層下拉內容

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/FilterOption/DepartmentLevelOption
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
| level | 階級名稱 |
| levelName | 階級名稱 |
| companyId | 公司別 |
| companyFullEName | 公司中文名稱 |
| companyFullName | 公司英文名稱 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "optionList":[
         {
            "level":3,
            "levelName":"總裁級"
         },
         {
            "level":4,
            "levelName":"總經理"
         },
         {
            "level":5,
            "levelName":"副總"
         },
         {
            "level":6,
            "levelName":"協理"
         },
         {
            "level":7,
            "levelName":"副總級"
         },
         {
            "level":8,
            "levelName":"協理級"
         },
         {
            "level":9,
            "levelName":"處級"
         },
         {
            "level":10,
            "levelName":"分店"
         },
         {
            "level":11,
            "levelName":"課級"
         },
         {
            "level":12,
            "levelName":"組級"
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
