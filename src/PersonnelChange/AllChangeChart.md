# AllChangeChart
整體人員異動圖表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/PersonnelChange/AllChangeChart
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
| series | 每組資料數值 |
| title | 主題名稱 |
| xaxis | 每組資料名稱 |
| labelName | 列表名稱 |
| labelValue | 列表數值 |


### HTTP Response when Successful
```json
{
  "responseHeader": {
    "resultMessage": "執行成功",
    "resultCode": "200"
  },
  "responseBody": {
    "title": "人員異動圖表",
    "series": [
      {
        "data": [
          2,
          0,
          3,
          5,
          0,
          0
        ]
      }
    ],
    "xaxis": {
      "data": [
        "新進人數",
        "離職人數",
        "調入人數",
        "調出人數",
        "留停人數",
        "復職人數"
      ]
    },
    "labelName": [
      "期初人數",
      "期末人數",
      "百分比提升",
      "平均人數"
    ],
    "labelValue": [
      176,
      176,
      0,
      176.0
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
