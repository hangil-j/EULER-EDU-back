# /login
로그인 관련 api

## /logininfo (GET)
### Response
```
{
    level: String,
    name: String // 로그인 정보
}
```

## /try/parent/type1/step1 (POST)
### URL Parameters
 - phone : 학부모 핸드폰 번호
### Response
```
{
    result: Boolean,
    msg: String // 로그인 실패 시 메시지
}
```

## /try/parent/type1/step2 (POST)
### URL Parameters
 - phone : 학부모 핸드폰 번호
 - authNumber : 인증번호
### Response
```
{
    result: Boolean,
    msg: String // 로그인 실패 시 메시지
}
```

## /try/parent/type2 (POST)
### URL Parameters
 - name : 학생 이름
 - birthday : 생일 6자리
 - pw : 로그인 시도 비밀번호
### Response
```
{
    result: Boolean,
    msg: String // 로그인 실패 시 메시지
}
```

## /try/teacher (POST)
### URL Parameters
 - id : 로그인 시도 아이디
 - pw : 로그인 시도 비밀번호
### Response
```
{
    result: Boolean,
    msg: String // 로그인 실패 시 메시지
}
```
