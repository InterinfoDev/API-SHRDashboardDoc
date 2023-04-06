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
        "title": "流失率",
        "key": "staffTurnoverRate"
      },
      {
        "title": "留停率",
        "key": "unpaidLeaveRate"
      },
      {
        "title": "同期流失率",
        "key": "simultaneousStaffTurnoverRate"
      }
    ],
    "lableList": [
      {
        "title": "部門",
        "key": "depName"
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
        "transferIn": "0",
        "transferOut": "0",
        "resign": "0",
        "rehab": "0",
        "beginning": "76",
        "ending": "76",
        "retentionRate": "100.00",
        "admissionRate": "0.00",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-7600.00"
      },
      {
        "depName": "L1線A班",
        "transferIn": "1",
        "transferOut": "0",
        "resign": "0",
        "rehab": "0",
        "beginning": "24",
        "ending": "25",
        "retentionRate": "100.00",
        "admissionRate": "4.00",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-2400.00"
      },
      {
        "depName": "企劃部",
        "transferIn": "1",
        "transferOut": "0",
        "resign": "0",
        "rehab": "0",
        "beginning": "17",
        "ending": "19",
        "retentionRate": "105.88",
        "admissionRate": "5.56",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-1700.00"
      },
      {
        "depName": "英特內(台北)",
        "transferIn": "0",
        "transferOut": "0",
        "resign": "0",
        "rehab": "0",
        "beginning": "4",
        "ending": "4",
        "retentionRate": "100.00",
        "admissionRate": "0.00",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-400.00"
      },
      {
        "depName": "顧問處",
        "transferIn": "0",
        "transferOut": "1",
        "resign": "0",
        "rehab": "0",
        "beginning": "18",
        "ending": "18",
        "retentionRate": "100.00",
        "admissionRate": "0.00",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-1800.00"
      },
      {
        "depName": "支援部",
        "transferIn": "1",
        "transferOut": "1",
        "resign": "0",
        "rehab": "0",
        "beginning": "5",
        "ending": "5",
        "retentionRate": "80.00",
        "admissionRate": "20.00",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-400.00"
      },
      {
        "depName": "測試部",
        "transferIn": "0",
        "transferOut": "3",
        "resign": "0",
        "rehab": "0",
        "beginning": "7",
        "ending": "4",
        "retentionRate": "57.14",
        "admissionRate": "0.00",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-600.00"
      },
      {
        "depName": "福委會",
        "transferIn": "0",
        "transferOut": "0",
        "resign": "0",
        "rehab": "0",
        "beginning": "4",
        "ending": "4",
        "retentionRate": "100.00",
        "admissionRate": "0.00",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-400.00"
      },
      {
        "depName": "test",
        "transferIn": "0",
        "transferOut": "0",
        "resign": "0",
        "rehab": "0",
        "beginning": "2",
        "ending": "2",
        "retentionRate": "100.00",
        "admissionRate": "0.00",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-200.00"
      },
      {
        "depName": "英特內股份有限公司",
        "transferIn": "0",
        "transferOut": "0",
        "resign": "0",
        "rehab": "0",
        "beginning": "4",
        "ending": "4",
        "retentionRate": "100.00",
        "admissionRate": "0.00",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-400.00"
      },
      {
        "depName": "總經理",
        "transferIn": "0",
        "transferOut": "0",
        "resign": "0",
        "rehab": "0",
        "beginning": "5",
        "ending": "5",
        "retentionRate": "100.00",
        "admissionRate": "0.00",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-500.00"
      },
      {
        "depName": "副總",
        "transferIn": "0",
        "transferOut": "0",
        "resign": "0",
        "rehab": "0",
        "beginning": "6",
        "ending": "6",
        "retentionRate": "100.00",
        "admissionRate": "0.00",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-600.00"
      },
      {
        "depName": "部門長",
        "transferIn": "0",
        "transferOut": "0",
        "resign": "0",
        "rehab": "0",
        "beginning": "2",
        "ending": "2",
        "retentionRate": "100.00",
        "admissionRate": "0.00",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-200.00"
      },
      {
        "depName": "課",
        "transferIn": "0",
        "transferOut": "0",
        "resign": "0",
        "rehab": "0",
        "beginning": "1",
        "ending": "1",
        "retentionRate": "100.00",
        "admissionRate": "0.00",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-100.00"
      },
      {
        "depName": "ABC",
        "transferIn": "0",
        "transferOut": "0",
        "resign": "0",
        "rehab": "0",
        "beginning": "1",
        "ending": "1",
        "retentionRate": "100.00",
        "admissionRate": "0.00",
        "dimissionRate": "0.00",
        "staffTurnoverRate": "0.00",
        "unpaidLeaveRate": "0.00",
        "simultaneousStaffTurnoverRate": "-100.00"
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
