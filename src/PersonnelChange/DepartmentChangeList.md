# DepartmentChangeList
部門異動列表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/PersonnelChange/DepartmentChangeList
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
    "companyId":[]
    ,"depNumber":[]
    ,"yymm": "202302"
    ,"depType": 3
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
| depNumber |  | Array(Integer) | 部門代碼 | N | n/a |
| yy | 202302 | String | 年分 | Y | YYYY |
| depType | 3 | Integer | 統計階層 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| rateList | 比率列表 |
| lableName | 標題名稱 |
| data | 資料(比率的值) |



### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "title":"部門異動列表",
      "rateList":[
         {
            "rateKey":"stayRate",
            "rateName":"留任率"
         },
         {
            "rateKey":"inRate",
            "rateName":"進任率"
         },
         {
            "rateKey":"quiteRate",
            "rateName":"離職率"
         },
         {
            "rateKey":"lostRate",
            "rateName":"流失率"
         },
         {
            "rateKey":"stopRate",
            "rateName":"留停率"
         },
         {
            "rateKey":"sameLostRate",
            "rateName":"同期流失率"
         }
      ],
      "lableName":[
         "",
         "部門",
         "調入",
         "調出",
         "離職",
         "復職",
         "期初",
         "期末"
      ],
      "data":{
         "lostRate":[
            [
               "0.00",
               "消失的部門",
               "0",
               "0",
               "0",
               "0",
               "76",
               "76"
            ],
            [
               "0.00",
               "L1線A班",
               "1",
               "0",
               "0",
               "0",
               "24",
               "25"
            ]
         ],
         "stopRate":[
            [
               "0.00",
               "消失的部門",
               "0",
               "0",
               "0",
               "0",
               "76",
               "76"
            ],
            [
               "0.00",
               "L1線A班",
               "1",
               "0",
               "0",
               "0",
               "24",
               "25"
            ]
         ],
         "sameLostRate":[
            [
               "-7600.00",
               "消失的部門",
               "0",
               "0",
               "0",
               "0",
               "76",
               "76"
            ],
            [
               "-2400.00",
               "L1線A班",
               "1",
               "0",
               "0",
               "0",
               "24",
               "25"
            ]
         ],
         "stayRate":[
            [
               "100.00",
               "消失的部門",
               "0",
               "0",
               "0",
               "0",
               "76",
               "76"
            ],
            [
               "100.00",
               "L1線A班",
               "1",
               "0",
               "0",
               "0",
               "24",
               "25"
            ]
         ],
         "quiteRate":[
            [
               "0.00",
               "消失的部門",
               "0",
               "0",
               "0",
               "0",
               "76",
               "76"
            ],
            [
               "0.00",
               "L1線A班",
               "1",
               "0",
               "0",
               "0",
               "24",
               "25"
            ]
         ],
         "inRate":[
            [
               "0.00",
               "消失的部門",
               "0",
               "0",
               "0",
               "0",
               "76",
               "76"
            ],
            [
               "4.00",
               "L1線A班",
               "1",
               "0",
               "0",
               "0",
               "24",
               "25"
            ]
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
