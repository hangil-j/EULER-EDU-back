# /login
로그인 관련 api

## /logininfo (GET)
### Response
```
{
    level: String,
    id: String,
    name: String
}
```

## /try/parent (POST)
### URL Parameters
 - id : 로그인 시도 아이디
 - pw : 로그인 시도 비밀번호
### Response
```
{
    result: Boolean,
    msg: String
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
    msg: String
}
```
