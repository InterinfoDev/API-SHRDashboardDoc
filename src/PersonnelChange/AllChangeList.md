# AllChangeList
整體異動數據

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/PersonnelChange/AllChangeList
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
| itemKey | 比率項目key |
| itemName | 比率項目中文名稱 |
| percent | 數據比率 |


### HTTP Response when Successful
```json
{
  "responseHeader": {
    "resultMessage": "執行成功",
    "resultCode": "200"
  },
  "responseBody": {
    "listAllChangeListOP": [
      {
        "itemKey": "stayRate",
        "itemName": "留任率",
        "percent": "98.30"
      },
      {
        "itemKey": "inRate",
        "itemName": "進任率",
        "percent": "1.70"
      },
      {
        "itemKey": "quiteRate",
        "itemName": "離職率",
        "percent": "0.00"
      },
      {
        "itemKey": "lostRate",
        "itemName": "流失率",
        "percent": "0.00"
      },
      {
        "itemKey": "stopRate",
        "itemName": "留停率",
        "percent": "0.00"
      },
      {
        "itemKey": "sameLostRate",
        "itemName": "同期流失率",
        "percent": "-17300.00"
      }
    ],
    "title": "整體異動數據"
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
