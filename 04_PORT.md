# 04. 포트

- 하나의 클라이언트에서 여러 프로그램이 연결을 해야 할 때
    - 전달받은 패킷의 구분이 필요함.
        - TCP/UDP 패킷에서 포트를 통해 이를 구분함
        
- IP: 아파트 / PORT: 동호수

- 0 ~ 1023 : well knwon port
    - ftp : 20, 21
    - telnet: 23
    - http: 80
    - https: 443
- 1024~ 65535 : 사용가능한 포트