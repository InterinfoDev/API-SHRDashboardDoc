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
            "fieldKey":"depName",
            "value":"技術用部",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"員工編號",
            "fieldKey":"employeeId",
            "value":"L105",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"員工姓名",
            "fieldKey":"employeeFullName",
            "value":"盧靜安",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"職稱",
            "fieldKey":"possieName",
            "value":"工程師",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"照片",
            "fieldKey":"photo",
            "value":"/servlet/jform?em_step=2&file=hrm8biw.pkg&enc=93d23f3a4b3f1a1110574d52104f57504b50d0d0860060c0f090f0d0f114f5158",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"分機號碼",
            "fieldKey":"extensionNumber",
            "value":"52",
            "oldValue":"",
            "change":false
         }
      ],
      "personalData":[
         {
            "fieldName":"員工姓名",
            "fieldKey":"employeeFullName",
            "value":"盧靜安",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"行事曆班別",
            "fieldKey":"shift",
            "value":"日常班",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"婚姻",
            "fieldKey":"marry",
            "value":"未婚",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"電子信箱",
            "fieldKey":"email",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"到職日期",
            "fieldKey":"startDate",
            "value":"2021/08/23",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"工作地點",
            "fieldKey":"place",
            "value":"新北-建八",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"聯絡電話",
            "fieldKey":"telephoneNumber",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"行動電話",
            "fieldKey":"cellphoneNumber",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"身高",
            "fieldKey":"tall",
            "value":"180",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"是否代扣所得稅",
            "fieldKey":"tax",
            "value":"Y",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"是否為原住民",
            "fieldKey":"originalResident",
            "value":"N",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"體重",
            "fieldKey":"weight",
            "value":"0",
            "oldValue":"",
            "change":false
         }
      ],
      "connectData":[
         {
            "fieldName":"戶籍郵遞區號",
            "fieldKey":"residencePostalCode",
            "value":"251",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"戶籍地址",
            "fieldKey":"residentialAddress",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"戶籍電話",
            "fieldKey":"residentialPhoneNumber",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"現址郵遞區號",
            "fieldKey":"currentPostalCode",
            "value":"251",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"現址地址",
            "fieldKey":"currentAddress",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"現址電話",
            "fieldKey":"currentPhoneNumber",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"通訊郵遞區號",
            "fieldKey":"mailingPostalCode",
            "value":"251",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"通訊地址",
            "fieldKey":"mailingAddress",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"通訊電話",
            "fieldKey":"contactPhoneNumber",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"緊急聯絡人姓名",
            "fieldKey":"emergencyContactFullName",
            "value":"吳OO",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"緊急聯絡人關係",
            "fieldKey":"relationshipToEmergencyContact",
            "value":"父子",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"緊急聯絡人電話",
            "fieldKey":"emergencyContactPhoneNumber",
            "value":"",
            "oldValue":"",
            "change":true
         }
      ],
      "educationData":[
         {
            "fieldName":"最高學歷",
            "fieldKey":"highestLevelOfEducation",
            "value":"學士",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"畢業學校",
            "fieldKey":"graduatedSchool",
            "value":"大學",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"主修科系",
            "fieldKey":"majorSubject",
            "value":"中餐藝系",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"請假時通知人員",
            "fieldKey":"takeLeaveNotifyPerson",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"畢肄業年月",
            "fieldKey":"graduationDate",
            "value":"2018/06",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"留職停薪迄日",
            "fieldKey":"endDateOfLeaveWithoutPay",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"留職停薪起日",
            "fieldKey":"startDateOfLeaveWithoutPay",
            "value":"",
            "oldValue":"",
            "change":true
         }
      ],
      "benefitData":[
         {
            "fieldName":"健保生效日",
            "fieldKey":"healthInsuranceStartDate",
            "value":"2021/08/23",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"健保等級",
            "fieldKey":"healthInsuranceLevel",
            "value":"26400",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"健保優惠專案",
            "fieldKey":"healthInsuranceDiscountProgram",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"健保眷口數",
            "fieldKey":"healthInsuranceOfFamily",
            "value":"1",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"勞保生效日",
            "fieldKey":"laborInsuranceStartDate",
            "value":"2021/08/23",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"勞保等級",
            "fieldKey":"laborInsuranceLevel",
            "value":"26400",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"勞保優惠專案",
            "fieldKey":"laborInsuranceDiscountProgram",
            "value":"",
            "oldValue":"",
            "change":true
         },
         {
            "fieldName":"公司提撥退休金",
            "fieldKey":"companyPensionContribution",
            "value":"新制",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"退休金等級",
            "fieldKey":"pensionTier",
            "value":"26400",
            "oldValue":"",
            "change":false
         },
         {
            "fieldName":"扶養人數",
            "fieldKey":"numberOfDependent",
            "value":"0",
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
            "titleKey":[
               "certificate",
               "dateOfAcquisition",
               "effectivePeriod",
               "calculateCertificationAllowance",
               "note",
               "fileDownload"
            ],
            "data":[
                "TOEIC_700分以上",
                "2017/04/29",
                "2019/04/29",
                "50",
                "測試用",
                ""
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
            "titleKey":[
               "sequence",
               "contractName",
               "startDate",
               "endDate",
               "note",
               "fileDownload"
            ],
            "data":[
                "01",
                "TESTNAME",
                "2019/04/29",
                "2024/02/12",
                "測試用",
                ""
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
            "titleKey":[
               "companyName",
               "courseName",
               "teachingInstitution",
               "startDate",
               "endDate",
               "allHours",
               "trainingMethod",
               "instructor",
               "score",
               "certificateNumber",
               "note",
               "fileDownload"
            ],
            "data":[
                "英特內",
                "課程名稱",
                "技術一部",
                "2023/02/12",
                "2023/02/12",
                "10",
                "跑步",
                "侯X安",
                "60",
                "164684654685",
                "TEST",
                ""
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
            "titleKey":[
               "companyName",
               "depName",
               "year",
               "assessmentItem",
               "scoringOfWorkObjectives",
               "scoringOfCompanyPolicies",
               "ManagerAssessment",
               "totalScores",
               "assessmentGrade",
               "yearsOfService",
               "note"
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
            "titleKey":[
               "identifyNumber",
               "employeeFullName",
               "birthDay",
               "gender",
               "salutation",
               "addHealthInsurance",
               "reportDependent",
               "healthInsuranceBenefit"
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
            "titleKey":[
               "companyName",
               "depName",
               "salutation",
               "startYM",
               "endYM",
               "compensation",
               "note",
               "yearsOfService",
               "leavingReason",
               "industry",
               "fileDownload"
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
