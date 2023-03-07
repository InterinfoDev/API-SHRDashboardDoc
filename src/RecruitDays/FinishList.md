# FinishList
結案需求單資訊

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/RecruitDays/FinishList
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
    ,"yymm": "2022"
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
| yymm | 202212 | String | 本期月份 | Y | YYYYmm |


### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| label | 欄位資料 |
| labelName | 表頭中文 |
| labelKey | 表頭對照值 |
| dataCount | 資料筆數 |
| maxDay | 最大天數 |
| averageDay | 平均天數 |
| pno | 需求單號 |
| days | 結案天數 |
| depFullName | 部門名稱 |
| positionName | 招募職位 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "title":"結案需求單列表",
      "dataCount":4,
      "maxDay":7,
      "averageDay":5.5,
      "label":[
         {
            "labelName":"No",
            "labelKey":"seriesNo"
         },
         {
            "labelName":"需求單單號",
            "labelKey":"pno"
         },
         {
            "labelName":"需求單位",
            "labelKey":"depFullName"
         },
         {
            "labelName":"招募職位",
            "labelKey":"positionName"
         },
         {
            "labelName":"申請日期",
            "labelKey":"applyDate"
         },
         {
            "labelName":"結案日期",
            "labelKey":"finishDate"
         },
         {
            "labelName":"結案天數",
            "labelKey":"days"
         }
      ],
      "data":[
         {
            "seriesNo":1,
            "pno":"002022121200001",
            "depFullName":"人力資源部",
            "positionName":"資深正職",
            "applyDate":"2022/12/12",
            "finishDate":"2022/12/15",
            "days":4
         },
         {
            "seriesNo":2,
            "pno":"002022121200002",
            "depFullName":"人力資源部",
            "positionName":"資深正職",
            "applyDate":"2022/12/12",
            "finishDate":"2022/12/18",
            "days":7
         },
         {
            "seriesNo":3,
            "pno":"002022121900001",
            "depFullName":"人力資源部",
            "positionName":"領班",
            "applyDate":"2022/12/19",
            "finishDate":"2022/12/25",
            "days":7
         },
         {
            "seriesNo":4,
            "pno":"002022122900001",
            "depFullName":"中央廚房",
            "positionName":"正職",
            "applyDate":"2022/12/28",
            "finishDate":"2022/12/31",
            "days":4
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
