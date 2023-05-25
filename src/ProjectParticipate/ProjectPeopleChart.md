# ProjectPeopleChart
參與人數圖表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/dashboard/V1/interfaces/ProjectParticipate/ProjectPeopleChart
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
| seriesByMonth | 依照年月分類 |
| seriesByClass | 依照課程分類 |
| series | 資料 |
| xaxis | x軸標題 |

### HTTP Response when Successful
```json
{
    "responseHeader": {
        "resultMessage": "執行成功",
        "resultCode": "200"
    },
    "responseBody": {
        "seriesByMonth": {
            "series": [
                {
                    "data": [],
                    "name": "計畫參與人數",
                    "type": "bar"
                },
                {
                    "data": [],
                    "name": "實際參與人數",
                    "type": "bar"
                }
            ],
            "xaxis": {
                "data": [
                    "2022/01",
                    "2022/02",
                    "2022/03",
                    "2022/04",
                    "2022/05",
                    "2022/06"
                ]
            }
        },
        "seriesByClass": {
            "series": [
                {
                    "data": [],
                    "name": "計畫參與人數",
                    "type": "bar"
                },
                {
                    "data": [],
                    "name": "實際參與人數",
                    "type": "bar"
                }
            ],
            "xaxis": {
                "data": []
            }
        }
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
        "seriesByMonth": {
            "series": [
            ],
            "xaxis": {
                "data": [
                ]
            }
        },
        "seriesByClass": {
            "series": [
            ],
            "xaxis": {
                "data": []
            }
        }
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
