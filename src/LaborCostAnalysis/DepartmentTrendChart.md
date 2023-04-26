# DepartmentTrendChart
平均時薪趨勢圖

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/LaborCostAnalysis/DepartmentTrendChart
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
    ,"yymm": "202303"
    ,"lastYymm":"202302"
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
| yymm | 202302 | String | 上期年月 | Y | YYYYmm |
| lastYymm | 202303 | String | 這期年月 | Y | YYYYmm |
| depType | 3 | Integer | 統計階層 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|




### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "lastDate":[
         "202203",
         "202204",
         "202205",
         "202206",
         "202207",
         "202208",
         "202209",
         "202210",
         "202211",
         "202212",
         "202301",
         "202302"
      ],
      "date":[
         "202203",
         "202204",
         "202205",
         "202206",
         "202207",
         "202208",
         "202209",
         "202210",
         "202211",
         "202212",
         "202301",
         "202302"
      ],
      "departmentData":[
         {
            "departmentName":"台北總公司",
            "averageList":[
               "11064",
               "11064",
               "0",
               "11064",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ],
            "lastAverageList":[
               "11064",
               "11064",
               "0",
               "11064",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ]
         },
         {
            "departmentName":"董事長室",
            "averageList":[
               "267881",
               "267511",
               "261544",
               "267691",
               "0",
               "252495",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ],
            "lastAverageList":[
               "267881",
               "267511",
               "261544",
               "267691",
               "0",
               "252495",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ]
         },
         {
            "departmentName":"稽核室/",
            "averageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ],
            "lastAverageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ]
         },
         {
            "departmentName":"憂鬱店外場",
            "averageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ],
            "lastAverageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ]
         },
         {
            "departmentName":"開心店外場",
            "averageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ],
            "lastAverageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ]
         },
         {
            "departmentName":"和睦外場",
            "averageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ],
            "lastAverageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ]
         },
         {
            "departmentName":"盡責外場",
            "averageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ],
            "lastAverageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ]
         },
         {
            "departmentName":"羨慕外場",
            "averageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ],
            "lastAverageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ]
         },
         {
            "departmentName":"安祥外場",
            "averageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ],
            "lastAverageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ]
         },
         {
            "departmentName":"部門",
            "averageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ],
            "lastAverageList":[
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0",
               "0"
            ]
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
