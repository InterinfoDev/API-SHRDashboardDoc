# LeaveWithoutPayRate
留停申請人數及留任狀況

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/LeaveWithoutPayRate/LeaveWithoutPayRate
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
    ,"depNumber":[17]
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
| depNumber | 17 | Array(Integer) | 部門代碼 | N | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| title | 標題名稱 |
| currentRate | 今年比例 |
| lastRate | 去年比例 |

### HTTP Response when Successful
```json
{
    "responseHeader": {
        "resultMessage": "執行成功",
        "resultCode": "200"
    },
    "responseBody": {
        "applyRate": {
            "title": "申請率",
            "currentRate": 0.0,
            "lastRate": 0.01
        },
        "remainRate": {
            "title": "留任率",
            "currentRate": 1.0,
            "lastRate": 1.0
        },
        "quitRate": {
            "title": "離職率",
            "currentRate": 0.0,
            "lastRate": 0.0
        },
        "backRate": {
            "title": "回任率",
            "currentRate": 0.0,
            "lastRate": 0.0
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
