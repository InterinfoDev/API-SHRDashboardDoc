# PositionAvgAgeChart
部門升等平均圖表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/PositionAvgAge/PositionAvgAgeChart
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
    "companyId":[1,2]
    ,"depNumber":[]
    ,"yyMmDd": "20230322"
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
| companyId | 1 , 2 | Array(String) | 公司代號 | N | n/a |
| depNumber | | Array(Integer) | 部門代碼 | N | n/a |
| yyMmDd | 20230322 | String | 年月日 | Y | YYYMMDD |
| depType | 8 | Integer | 統計階層 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| series | 資料 |
| data | X軸資料 |
| name | 名稱 |
| type | 圖表格式 |
| xaxis | X軸 |
| yaxis | Y軸 |
| name | 名稱 |
| position | 設定 |


### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "data":{
         "series":[
            {
               "data":[
                  4,
                  8
               ],
               "name":"人數",
               "type":"bar"
            },
            {
               "data":[
                  2.27,
                  6.53
               ],
               "name":"平均年資",
               "type":"line"
            }
         ],
         "xaxis":{
            "data":[
               "勞安部",
               "總務部"
            ]
         },
         "yaxis":[
            {
               "name":"人數",
               "position":"left"
            },
            {
               "name":"平均年資",
               "position":"right"
            }
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
