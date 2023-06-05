# OverHoursDepartmentList
各部門加班時數明細

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/OvertimeAnalysis/OverHoursDepartmentList
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
    "companyId":["1"]
    ,"depNumber":[]
    ,"workPlace":[]
    ,"depType": "8"
    ,"yymm": "202109"
    ,"lastYymm": "202108"
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
| companyId | [1] | Array(String) | 公司代號 | N | n/a |
| depType | 8 | String| 統計階層 | Y | n/a |
| depNumber | [] | Array(Integer) | 部門代碼 | Y | n/a |
| workPlace | TW | Array(String) | 工作地點 | N | n/a |
| yymm | 202109 | Array(Integer) | 本期月份 | Y | YYYYmm |
| lastYymm | 202108 | String | 上期月份 | Y | YYYYmm |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| label | 表頭明細 |
| labelName | 表頭名稱 |
| labelKey | 表頭值 |
| data | 資料 |
| depShortName | 部門簡稱 |
| lastAmt | 上期加班時數 |
| nowAmt | 本期加班時數 |
| score | 上升下降值 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "label":[
         {
            "labelName":"部門",
            "labelKey":"depShortName"
         },
         {
            "labelName":"202109",
            "labelKey":"nowAmt"
         },
         {
            "labelName":"202108",
            "labelKey":"lastAmt"
         },
         {
            "labelName":"上升/下降",
            "labelKey":"score"
         }
      ],
      "data":[
         {
            "depShortName":"人力資源部",
            "lastAmt":139.0,
            "nowAmt":117.5,
            "score":-0.22
         },
         {
            "depShortName":"勞安部",
            "lastAmt":24.5,
            "nowAmt":24.0,
            "score":-0.01
         }
      ]
   }
}
```

### HTTP Response when No Data
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "label":[
         {
            "labelName":"部門",
            "labelKey":"depShortName"
         },
         {
            "labelName":"202107",
            "labelKey":"YyMm"
         },
         {
            "labelName":"202106",
            "labelKey":"lastYyMm"
         },
         {
            "labelName":"上升/下降",
            "labelKey":"score"
         }
      ],
      "data":[
         
      ]
   }
}
```

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
