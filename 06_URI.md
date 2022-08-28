# 06. URI

- Uniform Resource Idenitifer 의 약자
- URI는 locator, name or 둘다 추가로 분류가능.

### URL

abc://example.com:8042/over/ther?name=freet#nose

- 리소스 위치를 지정
- 위치를 통해 접근, 구분

### URN

urn:expample:animal:ferrest:nnose

- 리소스에 이름을 부여
- 이름을 통해 접근, 구분

## URI

- 거의 url만 사용
- 자원을 구별하기 위한 양식

### URL 분석

[https://www.google.com/search?q=hello&hl=ko](https://www.google.com/search?q=hello&hl=ko)

scheme://[userinfo@]host[:port][/path][?qry][#frag]

- scheme
    - 프로토콜을 주로 사용
        - http, https, ftp 등을 사용
    - 80,443 주로 사용
    - 포트는 생략 가능
- userinfo
    - url에 사용자의 정보를 포함하여 진행하는 인증
    - 거의 사용 X
- host
    - 도메인 명 or IP 주소
- port
    - 생략 가능
- path
    - 리소스 경로
    - `/` 을 통해 구분
    - 계층적 구조
- query
    - key=value 형태
    - ?로 시작
- fragment
    - 내부 북마크로 사용
    - 서버 전송 X