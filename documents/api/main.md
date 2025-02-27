# /main
메인 페이지 관련 정보를 제공해주는 api

## / (GET)
### Response
```
{
    gallery: list[String], // 갤러리 이미지 url list
    campuses: list[{
        name: String, // 캠퍼스 이름
        imgUrl: String // 캠퍼스 이미지 url
    }],
    awards: list[{
        imgUrl: String, // 어워드 이미지 url,
        id: String // 어워드 고유아이디
    }]
    books: list[{
        name: String, // book 이름
        url: String, // book 연결 링크 url
        imgUrl: book // 이미지 url
    }],
    blogs: list[{
        title: String, // 블로그 글 제목
        url: String // 블로그 url
    }]
}
```

## /:id (GET)
### URL Parameters
 - id : 캠퍼스 고유아이디
### Response
```
{
    gallery: list[String], // 갤러리 이미지 url list
    notices: list[{
        title: String,
        id: String, // 공지 글 고유아이디
    }],
    posters: list[{
        title: String,
        content: String,
        url: String
    }],
    map: {
        lat: Number, // 캠퍼스 찾아오시는 길 위치 정보
        lng: Number // 캠퍼스 찾아오시는 길 위치 정보
    }
}
```
