# 03. TCP와 UDP

## 인터넷 프로토콜 4계층

App

전송

인터넷

네트워크 인터페이스

### 예시

1. 채팅 App에서 메시지 전송
2. 소켓 라이브러리를 통해 전달
3. TCP 정보를 추가
4. IP 정보 추가
5. 이더넷 프레임(?) 관련 추가

## 패킷

- 패키지 + 버킷
- 일종의 택배 박스

### IP 패킷

- 출발지, 목적지 주소

### TCP 패킷

- 전송 제어, 순서, 검증 정보

## TCP

전송 제어 프로토콜

- 연결 지향
- 데이터 전달 보증
- 순서 보장

### 연결 지향 3 way handshake (가상 연결)

1. SYN →
2. ← SYN + ACK
3. ACK → 
4. 데이터 전송
- ACK와 데이터 전송이 같이 이루어지기도 함.

### 데이터 전달 보증

- 응답자가 데이터 전달 완료 여부를 응답함.

### 순서 보장

- 응답자가 순서가 잘못된 위치부터 재전송을 요청함.

## UDP

사용자 데이터그램 프로토콜

- TCP에 비해 큰 특징이 없음.
- 포트, 체크섬 추가

### 포트

- 여러 프로그램을 포트를 통해 구분함.

- TCP에 비해 설정할 수 있는 것들이 많다.
    - 스스로 최적화할 때 사용
    - 최근 각광받고 있음.
    
- 영상 등 빠른 전송 위해 UDP를 사용했지만, 요즘은 TCP로도 다함.
- http3에서 사용
    - [https://evan-moon.github.io/2019/10/08/what-is-http3/](https://evan-moon.github.io/2019/10/08/what-is-http3/)