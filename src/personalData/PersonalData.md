# PersonalData
個人資料

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/personalData/PersonalData
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
| fieldName | 功能名稱 |
| value | 功能代號 |
| oldValue | 開啟 |
| change | 子功能 |
| identifyData | 身分基本資料 |
| personalData | 個人基本資料 |
| connectData | 聯絡資料 |
| educationData | 教育資料 |
| benefitData | 保險與福利資料 |
| licenseTableData | 證照資料 |
| greementTableData | 契約資料 |
| educationTableData | 教育訓練資料 |
| assessTableData | 考核歷程資料 |
| rewardTableData | 獎懲明細資料 |
| famailyTableData | 眷屬資料資料 |
| undergoTableData | 年資經歷資料 |


### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "identifyData":[
         {
            "fieldName":"英文姓名",
            "value":"Administrator",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"單位名稱",
            "value":"1 英特內股份有限公司",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"職稱",
            "value":"系統管理員",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"分機號碼",
            "value":"34",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"照片",
            "value":"",
            "oldValue":"",
            "change":true
         }
      ],
      "personalData":[
         {
            "fieldName":"行事曆班別",
            "value":"全班0930-2100",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"婚姻",
            "value":"已婚",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"電子信箱",
            "value":"richardwu@interinfo.com.tw",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"到職日期",
            "value":"2020/03/09",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"工作地點",
            "value":"雲林",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"聯絡電話",
            "value":"03-244446799",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"行動電話",
            "value":"097X3XX620",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"原住民",
            "value":"是",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"代扣所得稅",
            "value":"是",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"體重",
            "value":"189",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"身高",
            "value":"160",
            "oldValue":"",
            "change":false
         }
      ],
      "connectData":[
         {
            "fieldName":"戶籍郵遞區號",
            "value":"8846",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"戶籍地址",
            "value":"新北市中和區建一路１５０號６樓之３",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"戶籍電話",
            "value":"02-12",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"現址郵遞區號",
            "value":"302",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"現址地址",
            "value":"測試路１２８０號",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"現址電話",
            "value":"02-888888880",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"通訊郵遞區號",
            "value":"0095558",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"通訊地址",
            "value":"新北市中和區建一路１５０號６樓之３",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"通訊電話",
            "value":"02-12345678",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"緊急聯絡人姓名",
            "value":"測試B",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"緊急聯絡人關係",
            "value":"朋友",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"緊急聯絡人電話",
            "value":"0975422222223",
            "oldValue":"",
            "change":false
         }
      ],
      "educationData":[
         {
            "fieldName":"最高學歷",
            "value":"博士班畢業",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"畢業學校",
            "value":"國立交通大學",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"主修科系",
            "value":"人力資源發展系",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"請假時通知人員",
            "value":"0005,0008,0102",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"畢肄業年月",
            "value":"2007/06",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"留職停薪日期-起",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"留職停薪日期-訖",
            "value":"",
            "oldValue":"",
            "change":true
         }
      ],
      "benefitData":[
         {
            "fieldName":"健保生效日",
            "value":"1991/12/01",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"健保等級",
            "value":"92100",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"健保優惠專案",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"健保眷口數",
            "value":"0",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"勞保生效日",
            "value":"2013/04/28",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"勞保等級",
            "value":"21000",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"勞保優惠專案",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"公司提撥退休金",
            "value":"新制",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"退休金等級",
            "value":"123",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"扶養人數",
            "value":"1",
            "oldValue":"",
            "change":false
         }
      ],
      "page":{
         "licenseTableData":{
            "title":[
               "證照名稱",
               "取得日期",
               "有效日期",
               "計算證照津貼",
               "備註",
               "檔案上傳"
            ],
            "data":[
               [
                  "急救人員",
                  "2013/08/01",
                  "2013/08/23",
                  "Y",
                  "11tt",
                  ""
               ],
               [
                  "甲級空氣污染防治專責人員",
                  "2020/10/15",
                  "2020/10/15",
                  "N",
                  "22",
                  ""
               ],
               [
                  "1234",
                  "2022/10/01",
                  "2022/10/01",
                  "Y",
                  "yy4",
                  ""
               ],
               [
                  "甲級廢水處理專責人員",
                  "2022/11/01",
                  "2022/11/30",
                  "N",
                  "j",
                  ""
               ],
               [
                  "甲級空氣污染防治專責人員",
                  "2022/11/01",
                  "2022/11/09",
                  "Y",
                  "hh",
                  ""
               ]
            ],
            "show":true
         },
         "greementTableData":{
            "title":[
               "序",
               "合同名稱",
               "起始日期",
               "結束日期",
               "備註",
               "檔案上傳"
            ],
            "data":[
               [
                  "1",
                  "一年期契約",
                  "2019/07/01",
                  "2020/06/30",
                  "",
                  ""
               ],
               [
                  "2",
                  "三年期契約",
                  "2020/05/03",
                  "2020/05/29",
                  "",
                  ""
               ],
               [
                  "3",
                  "二年期契約",
                  "2020/05/03",
                  "2020/05/31",
                  "",
                  ""
               ]
            ],
            "show":true
         },
         "educationTableData":{
            "title":[
               "公司別 ",
               "課程名稱",
               "開課單位",
               "起始日期",
               "結束日期",
               "總時數",
               "訓練方式",
               "講師",
               "分數",
               "證書號碼",
               "備註",
               "檔案上傳"
            ],
            "data":[
               [
                  "72英特內(中和)",
                  "h",
                  "hh",
                  "2022/10/01",
                  "2022/10/15",
                  "10.0",
                  "t",
                  "hh",
                  "120.3",
                  "k",
                  "",
                  ""
               ],
               [
                  "72英特內(中和)",
                  "yyy",
                  "yyyy",
                  "2022/10/01",
                  "2022/10/08",
                  "10.0",
                  "tttt",
                  "jmm",
                  "100.0",
                  "tt",
                  "",
                  ""
               ]
            ],
            "show":true
         },
         "assessTableData":{
            "title":[
               "公司別 ",
               "單位",
               "年度",
               "考核項目",
               "工作目標給分",
               "公司政策給分",
               "主管給分",
               "總分",
               "考核等第",
               "年資",
               "備註"
            ],
            "data":[
               
            ],
            "show":true
         },
         "rewardTableData":{
            "title":[
               "公司別 ",
               "部門名稱",
               "獎懲名稱",
               "獎懲事由",
               "獎懲日期",
               "備註"
            ],
            "data":[
               
            ],
            "show":true
         },
         "famailyTableData":{
            "title":[
               "身分證字號",
               "姓名",
               "出生日期",
               "性別",
               "稱謂",
               "加健保",
               "報扶養",
               "健保優惠"
            ],
            "data":[
               [
                  "V220907583",
                  "岳先生",
                  "2023/11/09",
                  "男",
                  "岳父岳母",
                  "",
                  "Y",
                  ""
               ]
            ],
            "show":true
         },
         "undergoTableData":{
            "title":[
               "服務公司",
               "單位",
               "職稱",
               "起始年月",
               "結束年月",
               "待遇",
               "備註",
               "在職期間年資",
               "離職原因",
               "行業別",
               "檔案下載"
            ],
            "data":[
               
            ],
            "show":false
         }
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
