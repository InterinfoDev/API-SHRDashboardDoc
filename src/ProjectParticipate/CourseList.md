# CourseList
課程列表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/ProjectParticipate/CourseList
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
    "companyId":["1"],
    "depNumber":[7,13,14,16],
    "startYM": "202201",
    "endYM": "202201",
    "depType": 8
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
| depNumber | 7,13,14,16 | Array(Integer) | 部門代碼 | N | n/a |
| startYM | 202201 | String | 年月 | Y | YYYYmm |
| endYM | 202201 | String | 年月 | Y | YYYYmm |
| depType | 8 | Integer | 統計階層 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| courseList | 課程列表 |
| courseType | 課程類別 |
| startDate | 課程起始日期 |
| endDate | 課程結束日期 |
| bigCourse | 大分類名稱 |
| smallCourse | 小分類名稱 |
| hour | 課程時數 |
| finished | 結業名單 |
| unFinished | 未結業名單 |
| lessonName | 課程名單 |
| empFullName | 員工姓名 |
| employeeId | 員工編號 |
| depFullName | 部門名稱 |
| positionName | 職稱 |

### HTTP Response when Successful
```json
{
    "responseHeader": {
        "resultMessage": "執行成功",
        "resultCode": "200"
    },
    "responseBody": {
        "courseList": [
            {
                "courseType": "internal",
                "startDate": "2023/01/10",
                "bigCourse": "",
                "finished": [],
                "hour": 5.0,
                "endDate": "2023/01/10",
                "smallCourse": "",
                "lessonName": "",
                "unFinished": [
                    {
                        "empFullName": "",
                        "employeeId": "10001068",
                        "depFullName": "",
                        "positionName": ""
                    },
                    {
                        "empFullName": "王O足",
                        "employeeId": "10009002",
                        "depFullName": "總務部",
                        "positionName": "專員"
                    },
                    {
                        "empFullName": "蔡O隆",
                        "employeeId": "10108001",
                        "depFullName": "資訊部",
                        "positionName": "經理"
                    },
                    {
                        "empFullName": "王O靜",
                        "employeeId": "10210038",
                        "depFullName": "生產組",
                        "positionName": ""
                    }
                ],
                "depFullName": "人力資源部"
            }
        ]
    }
}
```

### HTTP Response when No Data
{
    "responseHeader": {
        "resultMessage": "執行成功",
        "resultCode": "200"
    },
    "responseBody": {
        "courseList": [
        ]
    }
}

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
