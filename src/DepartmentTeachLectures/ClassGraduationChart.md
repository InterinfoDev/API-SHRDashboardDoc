# ClassGraduationChart
月份結業人次分佈圖

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/DepartmentTeachLectures/ClassGraduationChart
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
    "companyId":["1","2"]
    ,"depNumber":[]
    ,"yymm": "202301"
    ,"lastYymm":"202305"
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
| companyId | ["1","2"] | Array(String) | 公司代號 | N | n/a |
| depNumber | [] | Array(Integer) | 部門代碼 | N | n/a |
| yymm | 202301 | String | 本期年月 | Y | YYYYMM |
| lastYymm | 202305 | String | 上期年月 | Y | YYYYMM |
| depType | 8 | Integer | 統計階層 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| dataList | 資料 |
| series | 資料陣列 |
| data | 結果值 |
| xaxis | x軸資料 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "dataList":{
         "series":[
            {
               "data":[
                  4
               ]
            },
            {
               "data":[
                  0
               ]
            }
         ],
         "xaxis":{
            "data":[
               "202301"
            ]
         }
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
