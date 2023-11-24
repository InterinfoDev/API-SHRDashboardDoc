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
            "fieldName":"單位名稱",
            "value":"經營管理",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"員工編號",
            "value":"L089100",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"員工姓名",
            "value":"陳汝玲",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"職稱",
            "value":"副總經理",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"照片",
            "value":"/servlet/jform?em_step=2&file=hrm8biw.pkg&enc=93d23f3a4b3f1a1110574d52104f57504b50100f0b0f060f0b0c0e0e0d0d0d0860060c0f090f0d0f114f5158",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"分機號碼",
            "value":"100",
            "oldValue":"",
            "change":false
         }
      ],
      "personalData":[
         {
            "fieldName":"員工姓名",
            "value":"陳汝玲",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"行事曆班別",
            "value":"日常班",
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
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"到職日期",
            "value":"2000/06/26",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"工作地點",
            "value":"新北-建一",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"聯絡電話",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"行動電話",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"身高",
            "value":"0",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"是否代扣所得稅",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"是否為原住民",
            "value":"N",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"體重",
            "value":"0",
            "oldValue":"",
            "change":false
         }
      ],
      "connectData":[
         {
            "fieldName":"戶籍郵遞區號",
            "value":"234",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"戶籍地址",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"戶籍電話",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"現址郵遞區號",
            "value":"234",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"現址地址",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"現址電話",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"通訊郵遞區號",
            "value":"234",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"通訊地址",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"通訊電話",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"緊急聯絡人姓名",
            "value":"OO",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"緊急聯絡人關係",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"緊急聯絡人電話",
            "value":"",
            "oldValue":"",
            "change":true
         }
      ],
      "educationData":[
         {
            "fieldName":"最高學歷",
            "value":"學士",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"畢業學校",
            "value":"淡江大學",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"主修科系",
            "value":"電子計算機應用學系",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"請假時通知人員",
            "value":"L091158,L091163,L093217,L089069 L101400 L098341",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"畢肄業年月",
            "value":"1987/06",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"留職停薪迄日",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"留職停薪起日",
            "value":"",
            "oldValue":"",
            "change":true
         }
      ],
      "benefitData":[
         {
            "fieldName":"健保生效日",
            "value":"2020/10/23",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"健保等級",
            "value":"26400",
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
            "value":"2020/10/23",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"勞保等級",
            "value":"26400",
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
            "value":"26400",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"扶養人數",
            "value":"2",
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
               "檔案下載"
            ],
            "data":[
               [
                  "HR-薪酬管理師",
                  "1998/03/05",
                  "",
                  "N",
                  "",
                  ""
               ],
               [
                  "HR-員工發展管理師",
                  "1998/01/09",
                  "",
                  "N",
                  "",
                  ""
               ],
               [
                  "HR-職能管理師",
                  "2007/09/01",
                  "",
                  "N",
                  "",
                  ""
               ],
               [
                  "HR-TTQS管理師",
                  "2007/06/01",
                  "",
                  "N",
                  "",
                  ""
               ],
               [
                  "HR-個人資料保護顧問培訓",
                  "",
                  "",
                  "N",
                  "",
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
               "檔案下載"
            ],
            "data":[
               
            ],
            "show":true
         },
         "educationTableData":{
            "title":[
               "公司別",
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
               "檔案下載"
            ],
            "data":[
               
            ],
            "show":false
         },
         "assessTableData":{
            "title":[
               "公司別",
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
            "show":false
         },
         "rewardTableData":{
            "title":[
               "公司別",
               "部門名稱",
               "獎懲名稱",
               "獎懲事由",
               "獎懲日期",
               "備註"
            ],
            "data":[
               
            ],
            "show":false
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
               
            ],
            "show":false
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
