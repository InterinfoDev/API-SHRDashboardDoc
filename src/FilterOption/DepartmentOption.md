# DepartmentOption
單位下拉塞選內容

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/FilterOption/DepartmentOption
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
| depNumber | 單位代碼 |
| depFullName | 單位中文名稱 |
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
            "departmentList":[
               
            ],
            "companyId":"52806695",
            "companyFullEName":"",
            "companyFullName":"72福委會"
         },
         {
            "departmentList":[
               {
                  "depNumber":"295",
                  "depFullName":"翰格雲端"
               },
               {
                  "depNumber":"369",
                  "depFullName":"總理經室"
               },
               {
                  "depNumber":"533",
                  "depFullName":"測試部"
               },
               {
                  "depNumber":"10038",
                  "depFullName":"技術處"
               }
            ],
            "companyId":"97090920",
            "companyFullEName":"ECMaker Information Corporation",
            "companyFullName":"72翰格"
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
