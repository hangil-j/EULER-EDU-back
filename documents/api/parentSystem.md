# /parentSystem
학부모 시스템 관련 api

## / (GET)
### Response
```
{
    students: list[{
        id: String, // 학생 고유아이디
        name: String, // 학생 이름
        campus: String // 학생 소속 학원
    }]
}
```

## /eRecord (POST)
### URL Parameters
 - id : 학생 고유아이디
 - year : 요청 년도
 - month : 요청 월
### Response
```
{
    year: Integer, // 년
    month: Integer, // 월 [1,12]
    monthStartDay: Integer, // 해당 달 시작 일 [1,31]
    monthEndDay: Integer, // 해당 달 마지막 일 [1,31]
    monthStartDayWeek: String, // 해당 달 시작 일의 요일 ['sun' | 'mon' | 'tue' | 'wed' | 'thu' | 'fri' | 'sat']
}
```
