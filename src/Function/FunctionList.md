# FunctionList
功能列表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/Function/FunctionList
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
       "depKey":"99710822536208190343"
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
| depKey | 99710822536208190343 | String | 單位Key值 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| name | 功能名稱 |
| page | 功能代號 |
| checked | 開啟 |
| subProjectList | 子功能 |


### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "functionList":[
         {
            "name":"D.招募相關",
            "page":"Dashboard.D",
            "functionKey":"1864901968730750136650025588166193174856",
            "checked":true,
            "subProjectList":[
               {
                  "name":"D001.人力缺口",
                  "page":"Dashboard.D001",
                  "functionKey":"1864901968730750136654522318106618588649",
                  "checked":true
               },
               {
                  "name":"D002.錄取管道分析",
                  "page":"Dashboard.D002",
                  "functionKey":"1864901968730750136643422650747353039852",
                  "checked":true
               },
               {
                  "name":"D003.招募效率分析",
                  "page":"Dashboard.D003",
                  "functionKey":"1864901968730750136639412913176071140872",
                  "checked":false
               },
               {
                  "name":"D004.招募平均天數",
                  "page":"Dashboard.D004",
                  "functionKey":"1864901968730750136639242256312981427727",
                  "checked":false
               },
               {
                  "name":"D005-新進員工報到率",
                  "page":"Dashboard.D005",
                  "functionKey":"1864901968730750136642793396948639538613",
                  "checked":false
               },
               {
                  "name":"D006.試用期通過率",
                  "page":"Dashboard.D006",
                  "functionKey":"1864901968730750136639119393472874674383",
                  "checked":false
               },
               {
                  "name":"D007-甄試結果分析(招募需求單)",
                  "page":"Dashboard.D007",
                  "functionKey":"1864901968730750136641181213766616487387",
                  "checked":false
               },
               {
                  "name":"D008.甄試結果分析(職位)",
                  "page":"Dashboard.D008",
                  "functionKey":"1864901968730750136640110609027070468285",
                  "checked":false
               },
               {
                  "name":"D009.招募整體分析",
                  "page":"Dashboard.D009",
                  "functionKey":"1864901968730750136647173421234557060654",
                  "checked":false
               }
            ]
         },
         {
            "name":"J.考核相關",
            "page":"Dashboard.J",
            "functionKey":"1864901968730750136638422832454104501603",
            "checked":false,
            "subProjectList":[
               {
                  "name":"J001.考核等級分佈",
                  "page":"Dashboard.J001",
                  "functionKey":"1864901968730750136652079173181479656526",
                  "checked":false
               },
               {
                  "name":"J002.年度員工績效趨勢",
                  "page":"Dashboard.J002",
                  "functionKey":"1864901968730750136648351060419031359461",
                  "checked":false
               },
               {
                  "name":"J003.績效考核分析",
                  "page":"Dashboard.J003",
                  "functionKey":"1864901968730750136647310832985063404648",
                  "checked":false
               }
            ]
         },
         {
            "name":"H.人事相關",
            "page":"Dashboard.H",
            "functionKey":"1864901968730750136651658666462723481080",
            "checked":false,
            "subProjectList":[
               {
                  "name":"H001.人事資料總表",
                  "page":"Dashboard.H001",
                  "functionKey":"1864901968730750136648615000237891417630",
                  "checked":false
               },
               {
                  "name":"H002.離職分析",
                  "page":"Dashboard.H002",
                  "functionKey":"1864901968730750136652999202637589066991",
                  "checked":false
               },
               {
                  "name":"H003.新進分析",
                  "page":"Dashboard.H003",
                  "functionKey":"1864901968730750136643666465161082333823",
                  "checked":false
               },
               {
                  "name":"H004.升等平均年資",
                  "page":"Dashboard.H004",
                  "functionKey":"1864901968730750136651573014121936730130",
                  "checked":false
               },
               {
                  "name":"H005.人員異動分析表",
                  "page":"Dashboard.H005",
                  "functionKey":"1864901968730750136638275371854629205861",
                  "checked":false
               },
               {
                  "name":"H006.留停申請人數及留任狀況",
                  "page":"Dashboard.H006",
                  "functionKey":"1864901968730750136643107104096728627491",
                  "checked":false
               }
            ]
         },
         {
            "name":"I.考勤相關",
            "page":"Dashboard.I",
            "functionKey":"1864901968730750136638165523695152406637",
            "checked":false,
            "subProjectList":[
               {
                  "name":"I001.加班時數分析",
                  "page":"Dashboard.I001",
                  "functionKey":"1864901968730750136642544016649836322033",
                  "checked":false
               },
               {
                  "name":"I002.當日請假人數分析",
                  "page":"Dashboard.I002",
                  "functionKey":"1864901968730750136643832868810963430325",
                  "checked":false
               },
               {
                  "name":"I003.各班別人數統計",
                  "page":"Dashboard.I003",
                  "functionKey":"1864901968730750136649941232925904631572",
                  "checked":false
               }
            ]
         },
         {
            "name":"M.薪資相關",
            "page":"Dashboard.M",
            "functionKey":"1864901968730750136647660692424028558698",
            "checked":false,
            "subProjectList":[
               {
                  "name":"M001.基本薪級距分析",
                  "page":"Dashboard.M001",
                  "functionKey":"1864901968730750136652560826058990611540",
                  "checked":false
               },
               {
                  "name":"M002.薪資級距分析",
                  "page":"Dashboard.M002",
                  "functionKey":"1864901968730750136656182007279452257655",
                  "checked":false
               },
               {
                  "name":"M003.用人成本分析",
                  "page":"Dashboard.M003",
                  "functionKey":"1864901968730750136651702385715515933770",
                  "checked":false
               }
            ]
         },
         {
            "name":"F.訓練相關",
            "page":"Dashboard.F",
            "functionKey":"1864901968730750136646781980618109610382",
            "checked":false,
            "subProjectList":[
               {
                  "name":"F001.內訓開課月份統計",
                  "page":"Dashboard.F001",
                  "functionKey":"1864901968730750136643407500707239132952",
                  "checked":false
               },
               {
                  "name":"F002.單位授課時數統計",
                  "page":"Dashboard.F002",
                  "functionKey":"1864901968730750136655442519740331763365",
                  "checked":false
               },
               {
                  "name":"F003.各單位計畫課程數vs實施課程時數",
                  "page":"Dashboard.F003",
                  "functionKey":"1864901968730750136639527692664156955445",
                  "checked":false
               },
               {
                  "name":"F004.年度計畫預計參與人數以及實際參與人數",
                  "page":"Dashboard.F004",
                  "functionKey":"1864901968730750136640469259176735999281",
                  "checked":false
               }
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
