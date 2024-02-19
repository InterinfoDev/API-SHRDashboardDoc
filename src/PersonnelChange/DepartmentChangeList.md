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




### HTTP Response when Successful
```json
{
  "responseHeader": {
    "resultMessage": "執行成功",
    "resultCode": "200"
  },
  "responseBody": {
    "title": "部門異動列表",
    "rateList": [
      {
        "title": "留任率",
        "key": "retentionRate"
      },
      {
        "title": "進任率",
        "key": "admissionRate"
      },
      {
        "title": "離職率",
        "key": "dimissionRate"
      },
      {
        "title": "留停率",
        "key": "unpaidLeaveRate"
      }
    ],
    "lableList": [
      {
        "title": "部門",
        "key": "depName"
      },
      {
        "title": "新進",
        "key": "newIn"
      },
      {
        "title": "調入",
        "key": "transferIn"
      },
      {
        "title": "調出",
        "key": "transferOut"
      },
      {
        "title": "留停",
        "key": "unPaidLeave"
      },
      {
        "title": "離職",
        "key": "resign"
      },
      {
        "title": "復職",
        "key": "rehab"
      },
      {
        "title": "期初",
        "key": "beginning"
      },
      {
        "title": "期末",
        "key": "ending"
      }
    ],
    "departmentList": [
      {
        "depName": "消失的部門",
        "transferIn": 0,
        "transferOut": 0,
        "resign": 0,
        "rehab": 0,
        "beginning": 76,
        "ending": 76,
        "retentionRate": 100.00,
        "admissionRate": 0.00,
        "dimissionRate": 0.00,
        "staffTurnoverRate": 0.00,
        "unpaidLeaveRate": 0.00,
        "simultaneousStaffTurnoverRate": -7600.00
      },
      {
        "depName": "L1線A班",
        "transferIn": 1,
        "transferOut": 0,
        "resign": 0,
        "rehab": 0,
        "beginning": 24,
        "ending": 25,
        "retentionRate": 100.00,
        "admissionRate": 4.00,
        "dimissionRate": 0.00,
        "staffTurnoverRate": 0.00,
        "unpaidLeaveRate": 0.00,
        "simultaneousStaffTurnoverRate": -2400.00
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
