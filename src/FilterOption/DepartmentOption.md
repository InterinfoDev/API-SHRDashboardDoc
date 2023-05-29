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
| nextDepartmentList | 下層單位列表 |

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
                  "depNumber":"2",
                  "depFullName":"總經理",
                  "depType":6,
                  "depCode":"10100",
                  "nextDepartmentList":[
                     {
                        "depNumber":"5",
                        "depFullName":"研發處",
                        "depType":9,
                        "depCode":"11000",
                        "nextDepartmentList":[
                           {
                              "depNumber":"6",
                              "depFullName":"行企課",
                              "depType":10,
                              "depCode":"11010",
                              "nextDepartmentList":[
                                 
                              ]
                           },
                           {
                              "depNumber":"257",
                              "depFullName":"研發組",
                              "depType":10,
                              "depCode":"11020",
                              "nextDepartmentList":[
                                 
                              ]
                           }
                        ]
                     }
                  ]
               },
               {
                  "depNumber":"82",
                  "depFullName":"英特內(中和)",
                  "depType":4,
                  "depCode":"10000",
                  "nextDepartmentList":[
                     {
                        "depNumber":"16",
                        "depFullName":"稽核室",
                        "depType":9,
                        "depCode":"12100",
                        "nextDepartmentList":[
                           
                        ]
                     },
                     {
                        "depNumber":"324",
                        "depFullName":"醫療課",
                        "depType":4,
                        "depCode":"324",
                        "nextDepartmentList":[
                           
                        ]
                     }
                  ]
               }
            ],
            "companyId":"TW",
            "companyFullEName":"Internet Information Co., Ltd.",
            "companyFullName":"英特內(中和)"
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

