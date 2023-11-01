# DepartmentList
部們群組列表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/Function/AssessAvgList
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

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| depNumber | 部門暗碼 |
| depFullName | 部門中文名稱 |
| depCode | 部門代號 |
| subDepartmentList | 下一層部門列表 |
| departmentList | 部門列表 |
| groupList | 群組列表 |


### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "departmentList":[
         {
            "depNumber":123532,
            "depFullName":"英x內集團",
            "depCode":"01231",
            "subDepartmentList":[
               {
                  "depNumber":53,
                  "depFullName":"董x會",
                  "depCode":"012302",
                  "subDepartmentList":[
                     {
                        "depNumber":132,
                        "depFullName":"英x內軟體公司",
                        "depCode":"001233",
                        "subDepartmentList":[
                           {
                              "depNumber":15,
                              "depFullName":"總xx室",
                              "depCode":"A01230",
                              "subDepartmentList":[
                                 {
                                    "depNumber":51,
                                    "depFullName":"經xx理",
                                    "depCode":"5123",
                                    "subDepartmentList":[
                                       {
                                          "depNumber":1235,
                                          "depFullName":"總xx處",
                                          "depCode":"A1000",
                                          "subDepartmentList":[
                                             {
                                                "depNumber":141,
                                                "depFullName":"行x部",
                                                "depCode":"A11410",
                                                "subDepartmentList":[
                                                   
                                                ]
                                             }
                                          ]
                                       }
                                    ]
                                 },
                                 {
                                    "depNumber":123141,
                                    "depFullName":"營xx理COO",
                                    "depCode":"B01230",
                                    "subDepartmentList":[
                                       {
                                          "depNumber":123432,
                                          "depFullName":"CTO",
                                          "depCode":"E03123",
                                          "subDepartmentList":[
                                             {
                                                "depNumber":3123,
                                                "depFullName":"技x處",
                                                "depCode":"E10010",
                                                "subDepartmentList":[
                                                   {
                                                      "depNumber":31234,
                                                      "depFullName":"工x部",
                                                      "depCode":"E21010",
                                                      "subDepartmentList":[
                                                         
                                                      ]
                                                   }
                                                ]
                                             }
                                          ]
                                       }
                                    ]
                                 }
                              ]
                           }
                        ]
                     },
                     {
                        "depNumber":21248,
                        "depFullName":"翰xxx公司",
                        "depCode":"A1230",
                        "subDepartmentList":[
                           {
                              "depNumber":43,
                              "depFullName":"總xx室",
                              "depCode":"A0100",
                              "subDepartmentList":[
                                 {
                                    "depNumber":321,
                                    "depFullName":"經x管x理",
                                    "depCode":"A0200",
                                    "subDepartmentList":[
                                       {
                                          "depNumber":123,
                                          "depFullName":"總xx處",
                                          "depCode":"A1000",
                                          "subDepartmentList":[
                                             {
                                                "depNumber":113,
                                                "depFullName":"行x部",
                                                "depCode":"A1100",
                                                "subDepartmentList":[
                                                   
                                                ]
                                             },
                                             {
                                                "depNumber":111,
                                                "depFullName":"會x部",
                                                "depCode":"A1120",
                                                "subDepartmentList":[
                                                   
                                                ]
                                             }
                                          ]
                                       }
                                    ]
                                 }
                              ]
                           }
                        ]
                     }
                  ]
               }
            ]
         }
      ],
      "groupList":[
         {
            "depNumber":1002002,
            "depFullName":"sys.異動單撤單群組",
            "depCode":"1002002"
         },
         {
            "depNumber":1001003,
            "depFullName":"sys.HR主管",
            "depCode":"1001003"
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
