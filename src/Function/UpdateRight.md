# UpdateRight
異動功能權限

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/Function/UpdateRight
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
   "requestHeader":{
      
   },
   "requestBody":{
      "depKey":"99710822536208190343",
      "functionList":[
         {
            "depKey":"99710822536208190343",
            "functionList":[
               {
                  "functionKey":"1864901968730750136650025588166193174856",
                  "checked":true,
                  "subProjectList":[
                     {
                        "functionKey":"1864901968730750136654522318106618588649",
                        "checked":true
                     },
                     {
                        "functionKey":"1864901968730750136643422650747353039852",
                        "checked":true
                     },
                     {
                        "functionKey":"1864901968730750136639412913176071140872",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136639242256312981427727",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136642793396948639538613",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136639119393472874674383",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136641181213766616487387",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136640110609027070468285",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136647173421234557060654",
                        "checked":false
                     }
                  ]
               },
               {
                  "functionKey":"1864901968730750136638422832454104501603",
                  "checked":false,
                  "subProjectList":[
                     {
                        "functionKey":"1864901968730750136652079173181479656526",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136648351060419031359461",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136647310832985063404648",
                        "checked":false
                     }
                  ]
               },
               {
                  "functionKey":"1864901968730750136651658666462723481080",
                  "checked":false,
                  "subProjectList":[
                     {
                        "functionKey":"1864901968730750136648615000237891417630",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136652999202637589066991",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136643666465161082333823",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136651573014121936730130",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136638275371854629205861",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136643107104096728627491",
                        "checked":false
                     }
                  ]
               },
               {
                  "functionKey":"1864901968730750136638165523695152406637",
                  "checked":false,
                  "subProjectList":[
                     {
                        "functionKey":"1864901968730750136642544016649836322033",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136643832868810963430325",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136649941232925904631572",
                        "checked":false
                     }
                  ]
               },
               {
                  "functionKey":"1864901968730750136647660692424028558698",
                  "checked":false,
                  "subProjectList":[
                     {
                        "functionKey":"1864901968730750136652560826058990611540",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136656182007279452257655",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136651702385715515933770",
                        "checked":false
                     }
                  ]
               },
               {
                  "functionKey":"1864901968730750136646781980618109610382",
                  "checked":false,
                  "subProjectList":[
                     {
                        "functionKey":"1864901968730750136643407500707239132952",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136655442519740331763365",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136639527692664156955445",
                        "checked":false
                     },
                     {
                        "functionKey":"1864901968730750136640469259176735999281",
                        "checked":false
                     }
                  ]
               }
            ]
         }
      ]
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
| depKey | 99710822536208190343 | String | 部門key值 | Y | n/a |
| functionKey | 1864901968730750136642544016649836322033 | String | 功能key值 | Y | n/a |
| checked | true | Boolean | 是否有權限 | Y | YYYY |
| subProjectList | [{"functionKey":"xxx","checked":false}] | object | 子項目 | N | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| result | 異動結果 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "result":true
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
