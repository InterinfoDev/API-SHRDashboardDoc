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
     "companyId":["TW"]
      ,"depType": 10
      ,"functionKey": "526468416548741684646468"
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
| companyId | TW | Array(String) | 公司代號 | N | n/a |
| depType | 10 | Integer | 統計階層 | Y | n/a |
| functionKey | 165465468168468 | String | 功能代號 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| companyId | 公司別 |
| companyFullEName | 公司中文名稱 |
| companyFullName | 公司英文名稱 |
| depNumber | 單位暗碼 |
| depCode | 單位明碼 |
| depFullName | 單位中文名稱 |
| depType | 單位階級 |
| parentDepNumber | 上層單位 |
| parentFullName | 上層單位名稱 |

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
               {
                  "depNumber":"257",
                  "depFullName":"消失的部門",
                  "depType":10,
                  "depCode":"10039",
                  "parentDepNumber":"1",
                  "parentFullName":"英特內股份有限公司"
               },
               {
                  "depNumber":"493",
                  "depFullName":"部門長",
                  "depType":10,
                  "depCode":"CCC",
                  "parentDepNumber":"492",
                  "parentFullName":"副總"
               },
               {
                  "depNumber":"495",
                  "depFullName":"企劃部",
                  "depType":10,
                  "depCode":"495",
                  "parentDepNumber":"1",
                  "parentFullName":"英特內股份有限公司"
               },
               {
                  "depNumber":"529",
                  "depFullName":"支援部",
                  "depType":9,
                  "depCode":"529",
                  "parentDepNumber":"528",
                  "parentFullName":"顧問處"
               },
               {
                  "depNumber":"534",
                  "depFullName":"測試部",
                  "depType":10,
                  "depCode":"534",
                  "parentDepNumber":"528",
                  "parentFullName":"顧問處"
               }
            ],
            "companyId":"TW",
            "companyFullEName":"",
            "companyFullName":"72英特內(中和)"
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

