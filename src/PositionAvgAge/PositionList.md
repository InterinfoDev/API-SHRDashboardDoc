# PositionList
部門人員升等平均年資表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/PositionAvgAge/PositionList
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
| avgYear | 升等平均年資 |
| empFullName | 人員名稱 |
| department | 部門 |
| position | 職稱 |
| photo | 圖片 |
| grade | 值等 |
| start | 初始值等 |
| end | 調整後值等 |


### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "data":[
         {
            "avgYear":"6.03",
            "empFullName":"王O英",
            "empFullEName":"JIA",
            "department":"勞安部",
            "position":"專員",
            "photo":"",
            "grade":"10",
            "start":[
               "20130624",
               "1"
            ],
            "end":[
               "20190701",
               "2"
            ]
         },
         {
            "avgYear":"6.12",
            "empFullName":"王O英",
            "empFullName":"王O英",
            "department":"勞安部",
            "position":"專員",
            "photo":"",
            "grade":"10",
            "start":[
               "20130624",
               "2"
            ],
            "end":[
               "20190801",
               "3"
            ]
         },
         {
            "avgYear":"6.66",
            "empFullName":"王O足",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"專員",
            "photo":"",
            "grade":"10",
            "start":[
               "20110901",
               "1"
            ],
            "end":[
               "20180427",
               "2"
            ]
         },
         {
            "avgYear":"7.51",
            "empFullName":"王O足",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"專員",
            "photo":"",
            "grade":"10",
            "start":[
               "20110901",
               "2"
            ],
            "end":[
               "20190301",
               "3"
            ]
         },
         {
            "avgYear":"10.36",
            "empFullName":"王O足",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"專員",
            "photo":"",
            "grade":"10",
            "start":[
               "20110901",
               "3"
            ],
            "end":[
               "20220101",
               "4"
            ]
         },
         {
            "avgYear":"",
            "empFullName":"王OA",
            "empFullEName":"KIOE",
            "department":"勞安部",
            "position":"外場-兼職三級",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20220101",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"王O無",
            "empFullEName":"KIOE",
            "department":"勞安部",
            "position":"經理",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20210701",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"王OA",
            "empFullEName":"KIOE",
            "department":"勞安部",
            "position":"外場-兼職三級",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20220101",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"王O無",
            "empFullEName":"KIOE",
            "department":"勞安部",
            "position":"經理",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20210701",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"蔡O芬",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"按摩人員",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20220201",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"王O真",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"按摩人員",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20191101",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"王O蓉",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"專員",
            "photo":"/hrm4/photo/1652684936132_S__127991850.jpg",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20220516",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"王O芳",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"司機",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "19981204",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"蔡O璐",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"專員",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20110127",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"蔡O芬",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"按摩人員",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20220201",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"王O真",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"按摩人員",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20191101",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"王O蓉",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"專員",
            "photo":"/hrm4/photo/1652684936132_S__127991850.jpg",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20220516",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"王O芳",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"司機",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "19981204",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"蔡O璐",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"專員",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20110127",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"蔡O芬",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"按摩人員",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20220201",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"王O真",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"按摩人員",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20191101",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"王O蓉",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"專員",
            "photo":"/hrm4/photo/1652684936132_S__127991850.jpg",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20220516",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"王O芳",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"司機",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "19981204",
               ""
            ]
         },
         {
            "avgYear":"",
            "empFullName":"蔡O璐",
            "empFullEName":"KIOE",
            "department":"總務部",
            "position":"專員",
            "photo":"",
            "grade":"10",
            "start":[
               "",
               ""
            ],
            "end":[
               "20110127",
               ""
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
